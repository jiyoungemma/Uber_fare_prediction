# Uber 요금 예측 프로젝트

### 프로젝트 기획 배경
우버는 공유경제 중 하나로 계속해서 발전하여 하나의 보편적인 서비스로 자리매김한 서비스 중 하나이다. 해외에서는 모든 사람들의 스마트폰에는 우버 어플이 설치되어 있다고 해도 과언이 아닐정도로 많은 고객을 보유하고 있다. 우버 요금 예측 모델을 개발하여 미리 예측 요금을 확인하고 서비스를 이용할 것인지에 대해 판단하기 위해 프로젝트를 기획하였다.

### 가설 검증
- 출퇴근 시간에 우버 요금이 다른 시간대와 비교해 비쌀 것이다. → TRUE
- 기념일이 많은 11~12월의 우버 요금이 다른 달과 비교해 비쌀 것이다. → TRUE
- 탑승 승객이 많을수록 요금이 상승할 것이다. → FALSE
---
### 사용 기술

#### 데이터 분석 & 시각화
- pandas
- numpy
- matplotlib
- pdpbox
- shap

#### 모델링
- xgboost
- sklearn
- category_encoders
- scipy

---

### 과정 요약
- baseline model을 `linear regression`으로 설정
- 모델링에 `random forest regressor` 와 `xgbregressor` 사용
- `xgbregressor`이 더 높은 성능을 보여 채택, 테스트 데이터 학습 결과 R^2 : 0.8318 도출
