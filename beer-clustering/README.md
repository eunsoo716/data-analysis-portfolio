# Beer Profile 소비자 세그먼트 분석 (클러스터링)

맥주 3,197종의 맛 프로파일로 **자연 발생 군집을 찾고 "무엇이 고평점을 만드는가"**를 규명한 비지도학습 프로젝트입니다. (대학 STAT 437 그룹 프로젝트 — **DBSCAN 파트 담당**)

> 📄 상세 보고서: [REPORT_ko.md](./REPORT_ko.md)

## 문제정의
맛 프로파일 변수만으로 내재 군집이 존재하는지, 무엇이 고평점 맥주를 만드는지 규명.

## 데이터
- Kaggle "Beer Profile and Ratings" — 3,197개 맥주 × 25개 변수
- 출처: https://www.kaggle.com/datasets/ruthgn/beer-profile-and-ratings-data-set

## 분석 과정
1. StandardScaler 표준화
2. t-SNE로 군집가능성 선검증 (perplexity·seed 다중 비교)
3. **DBSCAN 파라미터 탐색** (k-distance plot, eps×min_samples 격자 탐색 → eps=1.8/min_samples=8)
4. HAC·K-Means와 교차검증
5. 군집 특성·평점 해석 (노이즈 16%를 니치 스타일로 해석)

## 결과
- 맥주는 뚜렷한 군집이 아닌 **연속적 맛 스펙트럼**
- 고평점을 가르는 건 강도가 아니라 **"균형·풍미 복합성"**
- DBSCAN이 팀의 최종 주력 방법으로 채택

## 사용 기술
Python, scikit-learn (DBSCAN·K-Means·계층적·t-SNE), scipy, seaborn
