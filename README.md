# 데이터 분석 포트폴리오 — Eunsoo Kwon

통계 전공 졸업 / 데이터 분석가를 목표로 진행한 프로젝트 모음입니다. 각 프로젝트는 **문제정의 → 데이터 분석 → 인사이트 도출**의 흐름으로 정리했습니다.

## 📂 프로젝트

| 프로젝트 | 한 줄 소개 | 핵심 기술 |
|---|---|---|
| [Olist 이커머스 고객 분석](https://github.com/eunsoo716/data-analysis-portfolio/tree/main/olist-analysis) | 주문 9.6만 건을 SQL로 분석해 재구매 구조(재구매율 2.15%)를 확인하고, 통제 후에도 배송 지연이 낮은 리뷰 확률을 26.3%p 높인다는 점을 근거로 검증용 A/B 테스트 설계 | SQL(DuckDB, CTE·윈도우 함수), 로지스틱 회귀, 실험 설계 |
| [콜센터 콜량 수요예측](https://github.com/eunsoo716/data-analysis-portfolio/tree/main/call-center-forecast) | 콜센터 콜량·응대시간을 30분 단위로 예측, 구간 직접 예측으로 콜량 오차율 개선 (A 46.6% → 28.6%) | Python, LightGBM, 시계열 피처 엔지니어링 |
| [Beer 소비자 세그먼트 분석](https://github.com/eunsoo716/data-analysis-portfolio/tree/main/beer-clustering) | 맥주 3,197종을 클러스터링해 평점이 높은 군집의 특징 규명 (DBSCAN 파트 담당) | scikit-learn, DBSCAN, t-SNE |
| [학생 학업 중도이탈 예측](https://github.com/eunsoo716/data-analysis-portfolio/tree/main/student-dropout-prediction) | 학생 4,424명을 1학기 말 정보만으로 예측(ROC-AUC 약 0.91), 위험 상위 20%에 연락하면 92%가 실제 중도이탈 | Python, XGBoost·LightGBM·CatBoost, SHAP |

## 🧰 기술 스택

- 언어: Python, SQL (DuckDB)
- 분석·시각화: pandas, numpy, matplotlib, seaborn
- 통계·실험: 로지스틱 회귀(통제 변수 효과 추정), A/B 테스트 설계(표본 수 계산, SRM 점검)
- 머신러닝: 로지스틱 회귀, LightGBM, XGBoost, CatBoost, 클러스터링(DBSCAN·K-Means·계층적), SHAP
- 자격증: ADsP, SQLD

## 📌 참고

- 일부 데이터는 외부 출처(경진대회·Kaggle·UCI) 제공으로, 라이선스상 저장소에는 포함하지 않았습니다. 각 프로젝트 README의 데이터 출처를 기재해놓았습니다

