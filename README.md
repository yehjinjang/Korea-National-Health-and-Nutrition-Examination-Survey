## 국민건강영양조사 자료 활용 프로젝트 모음 (2019~2022) 

## 📊 한국형 고혈압 예측 모델 

## 📝 Overview(1)
이 프로젝트는 비즈니스 통계응용 수업의 일환으로, 데이터 기반 비즈니스 모델 프로젝트를 포함합니다. 한국형 고혈압 예측 모델을 개발을 주제로 다루었습니다.

## 🚀 개인 프로젝트

### 1. 🩺 한국형 고혈압 예측 모델
#### 📌 
- **목표**: 한국인의 건강 특성을 반영하여 고혈압 발생 가능성을 예측하는 모델을 개발
- **데이터 소스**: 2019~2022년 국가건강영양조사(국건영)
- **진단 기준**: 
  - 미국 기준: 130/80mmHg
  - 유럽 기준: 140/90mmHg
- **연구 의의**: 한국인을 대상으로 한 맞춤형 고혈압 예측 모델 제공

#### Tech Stack
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) 
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) 
![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white) 
![XGBoost](https://img.shields.io/badge/XGBoost-FF4C00?style=for-the-badge&logo=xgboost&logoColor=white) 
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white) 

#### 🔑 Key Tasks
1. **데이터 전처리**:
   - 이상치 제거 (중성지방 > 500mg/dL, BMI > 40)
   - Feature Engineering: 당뇨, 비만도, 가족력 등 주요 요인 추출
2. **EDA (탐색적 데이터 분석)**:
   - 상관관계 분석(Heatmap)
   - 변수별 데이터 분포 시각화
3. **모델링 및 평가**:
   - Logistic Regression, Decision Tree, Random Forest, XGBoost 활용
   - GridSearchCV를 통한 하이퍼파라미터 튜닝
   - Accuracy, AUC Score로 성능 평가
4. **결과 해석**:
   - 특성 중요도(MDI, Permutation Importance) 및 경향성(PDP) 분석

#### 🎯 Outcomes
- **최종 모델**: XGBoost (Accuracy: 87%, AUC: 0.91)
- **주요 요인**: 나이, BMI, 가족력이 고혈압 발생에 가장 큰 영향
- **결론**: 유럽 진단 기준이 한국인의 특성에 더 적합

---

### 2. 📈 2030 위암 증가 요인 분석 *(진행 중)*
#### 📌 개요
- **목표**: 2030 세대에서 위암 발병률 증가에 영향을 미치는 주요 요인을 파악.
- **데이터 소스**: 2022년 국가건강영양조사(국건영) 및 공공 건강 데이터.
- **분석 방향**: 식습관, 생활 습관, 환경적 요인과의 연관성 분석.

#### ⚙️ 사용 기술
| 기술               | 아이콘                                                                 |
|--------------------|----------------------------------------------------------------------|
| Python            | ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) |
| Pandas            | ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) |
| Seaborn           | ![Seaborn](https://img.shields.io/badge/Seaborn-0081CB?style=for-the-badge&logo=data:image/svg+xml;base64,<svg_data>) |

#### 🔑 Key Tasks
1. **데이터 수집 및 전처리**:
   - 공공 데이터 포털에서 위암 관련 데이터 수집.
   - 결측치 처리 및 변수 생성(식습관 점수, 환경 노출 지표 등).
2. **탐색적 데이터 분석**:
   - 위암 발병률과 주요 변수 간 상관관계 확인.
3. **모델링**:
   - 다중 회귀 분석 및 변수 중요도 평가.
   - 위암 발병 위험 예측 모델 개발 진행 중.

---

### 3. 🕊️ 노인 고독사 수면 비율 분석 *(진행 중)*
#### 📌 개요
- **목표**: 고독사 위험성과 수면 패턴의 연관성을 규명.
- **데이터 소스**: 2022년 국가건강영양조사(국건영).
- **연구 의의**: 노인층의 건강 관리 및 예방 정책 수립에 기여.

#### ⚙️ 사용 기술
| 기술               | 아이콘                                                                 |
|--------------------|----------------------------------------------------------------------|
| Python            | ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) |
| Pandas            | ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) |
| Matplotlib        | ![Matplotlib](https://img.shields.io/badge/Matplotlib-0177BE?style=for-the-badge&logo=data:image/svg+xml;base64,<svg_data>) |

#### 🔑 Key Tasks
1. **데이터 전처리**:
   - 결측치 처리 및 데이터 정규화.
   - 수면 패턴 변수와 고독사 발생률 간 관계 정의.
2. **탐색적 데이터 분석**:
   - 수면 비율과 고독사 데이터 간 상관관계 분석.
   - 고독사 고위험군과 수면 패턴 시각화.

---

## 📌 프로젝트 회고
- **성공 사례**:
  - XGBoost 기반 고혈압 예측 모델에서 높은 성능 확보.
  - 공공 데이터를 활용하여 실질적이고 정책적으로 유용한 인사이트 제공.
- **한계점**:
  - 일부 연구는 데이터 제한으로 인해 추가적인 변수 포함 불가.
  - 스트레스, 나트륨 섭취량 등 주요 변수 추가 분석 필요.
