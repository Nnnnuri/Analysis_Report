# [분석보고서] 서울특별시 어린이 교통 사고 수와 사회적 요인의 상관 관계

### 프로젝트 기간
- 2024년 12월 30일 ~ 2025년 1월 7일

### 참여자
- 김경민, 박수빈, 은연정, 조누리

### 프로젝트 소개
서울시 공공 데이터를 기반으로 어린이 교통사고 발생과 사회적 요인 간의 관계를 분석하고, 상관관계 분석과 머신러닝 모델(Random Forest, XGBoost)을 통해 사고 건수에 영향을 미치는 주요 요인을 도출. 이를 바탕으로 사고 위험 예측 및 정책 수립에 활용 가능한 인사이트를 제시

### 폴더 구조
```
📁Analysis_Report
 ├─ .DS_Store
 ├─ .gitignore
 ├─ README.md
 ├─ report.ipynb
 └─ 📁Project
    └─📁csv
        └─ analysis_report.csv
```

<br>

## 기술 스택
1. 분석 툴: Python
2. 라이브러리: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, MinMaxScaler, RandomForestRegressor, XGBRegressor

<br>

## 데이터 소개
- 서울 열린데이터 광장, 도로교통공단, 행정안전부 외 총 11개 공공 데이터셋

<br>

## 데이터 전처리
- 정규화: MinMaxScaler 적용 (종속변수 제외)
- 왜도 보정: 지방세 데이터 log 변환
- 결측치 처리: 10% 이상 결측 컬럼 제거, 나머지는 행 삭제
- 직접적 영향 변수 제거: `어린이 인구`, `전체 사고 건수` 등은 모델에서는 제외하고 참고용 변수로만 사용

<br>

## 프로젝트 요약
- 서울시 자치구별 공공 데이터를 기반으로, 어린이 교통사고 발생에 영향을 주는 사회적 요인을 도출하고 머신러닝 모델을 통해 사고 위험을 예측. 분석 결과를 바탕으로 정책적 시사점을 제시
- 실제 행정 기획에 활용 가능한 데이터 기반 분석 프로젝트로 발전 및 정책적 해석까지 고려

<br>