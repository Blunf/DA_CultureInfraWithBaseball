# 야구장 수요 증가에 따른 주변 문화시설 연계 발전 분석 및 머신러닝 기반 향후 활성화 예측

## 📌 프로젝트 개요

본 프로젝트는 대한민국 주요 야구장의 관중 수 증가 현상을 기반으로, 야구장 인근 지역의 문화시설과의 공간적, 기능적 연계 가능성을 분석하고, 전략을 도출하는 것을 목적으로 합니다.
또한 향후 연계 발전률 예측을 통해 경제적 효과를 예측합니다.


## 🗂️ 프로젝트 구조

\`\`\`
baseball-cultural-facility-strategy/
├── data/
│   ├── raw/        # 원본 데이터 (야구장, 문화시설, 인구 등)
│   └── processed/  # 전처리된 데이터
│
├── notebooks/
│   ├── 01_eda.ipynb        # 탐색적 분석
│   ├── 02_clustering.ipynb # 지역 유형 분류 (KMeans 등)
│   └── 03_modeling.ipynb   # ML 모델로 영향 예측
│
├── src/
│   ├── data_collection.py # 데이터 수집 코드
│   ├── preprocessing.py   # 전처리 코드
│   ├── clustering.py      # 지역 분류 로직
│   ├── modeling.py        # ML 예측 모델
│   └── visualization.py   # 시각화 함수
│
├── outputs/
│   ├── figures/ # 분석 결과 시각화
│   └── tables/  # 요약 테이블
│
├── reports/
│   ├── presentation.pptx  # 발표 자료
│   └── final_report.pdf   # 최종 정책 제안 보고서
│
├── requirements.txt # 필요한 Python 패키지 목록
├── .gitignore       # Git에 포함시키지 않을 파일
└── README.md        # 이 문서
\`\`\`

## 📊 주요 데이터셋

| 출처 | 데이터 | 내용 |
|------|--------|------|
| 공공데이터포털 | `문화시설 현황`, `인구·유동인구`, `시설 위치` | 각 지역별 문화 인프라 정보 |
| KBO | `야구장별 관중 수` | 연도별 경기 관람객 수 |
| 통계청 | `지역 경제 활동`, `상권`, `생활환경` | 정책 판단을 위한 지역 지표 |



## 🛠 사용 기술

- Python (pandas, scikit-learn, geopandas, folium, matplotlib, seaborn)
- Jupyter Notebook
- 머신러닝 모델 (XGBoost, RandomForest 등)
- 공간 분석 (좌표 기반 시각화 및 클러스터링)
