## Spotify Tracks Popularity & Musical Feature Analysis
Spotify 트랙 데이터를 활용해 아티스트, 장르, 연도별 인기 및 음악적 특성 분석

#### Skillset / Tools

SQL: 데이터베이스 설계, 테이블 생성, 데이터 탐색, 집계, 그룹화, 윈도우 함수, CTE 활용
데이터 분석: 인기 트랙/아티스트 도출, 장르별 트렌드, 연도별 변화 분석

#### Background / Objective
Spotify 데이터를 기반으로 트랙, 아티스트, 장르별 음악적 특성과 인기 트렌드를 분석했습니다.

목적:
인기 있는 아티스트·트랙과 장르별 트렌드 파악
연도별 음악적 변화 및 밸런스(valence, energy 등) 분석
특정 음악적 조합(tempo, valence)과 청취자 반응 잠재력 탐색

#### Key Analysis / Results

Top Tracks & Artists
인기 트랙 상위 10개, 아티스트 평균 인기 상위 10명 도출
트랙 수가 많으면서 인기 있는 아티스트 식별

#### Genre & Year Trends

장르별 평균 인기 점수 및 평균 템포 분석
연도별 트랙 수, 인기 트랙, 인기 아티스트 변화 확인

#### Musical Feature Insights

tempo >150 & valence <0.3 조합 트랙 탐색 → 텐션 유발 가능성 평가
아티스트별 valence·energy 변화 폭 분석 → 음악적 다양성 파악
연도별 valence 변화 최대 폭 분석 → 음악적 트렌드 변화 시각화

####  Learned / Application

배운 점:
SQL 집계, 윈도우 함수, CTE 활용으로 복합 분석 가능성을 이해
음악적 특성과 청취자 반응 간의 연관성을 데이터 기반으로 정량화

적용 가능성:
추천 시스템, 플레이리스트 큐레이션, 음악 트렌드 분석 및 마케팅 전략 수립에 활용 가능
***
## Telco Customer Churn Analysis & Prediction
통신사 고객 데이터를 기반으로 이탈 원인 분석과 ML 기반 고객 이탈 예측 모델 개발

#### Skillset / Tools
SQL: 계약 유형, 요금제, 서비스 가입 여부, 결제 방식, 연령대별 고객 이탈률 분석
Python & ML: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, Imbalanced-learn(SMOTE)
모델링: Logistic Regression, Random Forest, Gradient Boosting, XGBoost, SVM, Ensemble

#### Background / Objective
통신사 고객 데이터에서 고객 이탈 패턴과 위험 요인을 파악하고, 머신러닝 모델을 통해 조기 이탈 가능 고객을 예측하는 것이 목표였습니다.
SQL 탐색 분석으로 계약 유형·요금제·결제 방식·서비스 가입 여부별 이탈률 확인
Python 기반 ML 모델로 고객 세그멘테이션 및 예측 모델 성능 검증

#### Key Analysis / Results
SQL 기반 탐색 분석
계약 유형별 이탈률: Month-to-Month 계약 고객의 이탈률이 가장 높음
요금제·결제 방법·인터넷 서비스 유형·추가 서비스 가입 여부에 따른 이탈률 확인
조기 이탈 가능 고객(tenure ≤6개월, MonthlyCharges >70) 식별
고객 세그멘테이션: VIP 고객, 이탈 위험 고객, 업셀링 가능 고객 등 분류

#### ML 기반 예측 모델
데이터 전처리: 결측값 처리, One-Hot Encoding, StandardScaler, SMOTE 적용
모델 성능:
Logistic Regression: Accuracy 0.8055 | F1 0.6040 | AUC 0.8419
Random Forest: Accuracy 0.7779 | F1 0.5321 | AUC 0.8164
Gradient Boosting: Accuracy 0.8062 | F1 0.5895 | AUC 0.8432
XGBoost: Accuracy 0.7736 | F1 0.5384 | AUC 0.8217
SVM: Accuracy 0.7913 | F1 0.5518 | AUC 0.7905
Optimized Random Forest: 하이퍼파라미터 튜닝 후 F1 향상
Ensemble Model: VotingClassifier 기반 F1 0.5997 | AUC 0.8338
Feature Importance 분석: MonthlyCharges, tenure, Contract, 서비스 가입 여부 등 주요 변수 확인

#### Learned / Application
배운 점:
SQL로 탐색적 데이터 분석(EDA)을 통해 이탈 패턴과 비즈니스 인사이트 도출
ML 파이프라인 구축, SMOTE 활용 불균형 데이터 처리, 다양한 모델 성능 비교 경험

적용 가능성:
고객 유지 전략 설계, 마케팅 타겟팅, 조기 이탈 방지 캠페인, 추천형 요금제 제안 등 실무 적용 가능
