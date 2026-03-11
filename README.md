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
