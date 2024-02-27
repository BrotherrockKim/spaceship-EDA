## 프로젝트 제목 
# "Spaceship Titanic: A Machine Learning Approach to Predict Interdimensional Transport"

## 프로젝트 설명
#### 우주선 Titanic을 탄 승객들은 사고에 의해서 다른 차원으로 이동했다. 이때, 어떤 승객이 다른 차원으로 이동했는지 예측해야 한다.

## 데이터셋
- 데이터 출처 링크 Kaggle : https://www.kaggle.com/competitions/spaceship-titanic
- 데이터 칼럼 정보

| Column | Description | Data Type | Example |
| ------ | ----------- | --------- | ------- |
| PassengerId | A unique Id for each passenger. | object | 0001_01 |
| CryoSleep | Indicates if the passenger was in suspended animation during the voyage. | int64 | 0 |
| VIP | Whether the passenger has paid for special VIP service. | int64 | 0 |
| Transported | Whether the passenger was transported to another dimension (target variable). | bool | False |
| HomePlanet_Earth | The planet the passenger departed from - Earth. | float64 | 0.0 |
| HomePlanet_Europa | The planet the passenger departed from - Europa. | float64 | 1.0 |
| HomePlanet_Mars | The planet the passenger departed from - Mars. | float64 | 0.0 |
| Destination_55 Cancri e | The destination planet of the passenger - 55 Cancri e. | float64 | 0.0 |
| Destination_PSO J318.5-22 | The destination planet of the passenger - PSO J318.5-22. | float64 | 0.0 |
| Destination_TRAPPIST-1e | The destination planet of the passenger - TRAPPIST-1e. | float64 | 1.0 |
| Age | The age of the passenger. | float64 | 0.493671 |
| RoomService | Amount billed for room service. | float64 | 0.0 |
| FoodCourt | Amount billed at the food court. | float64 | 0.0 |
| ShoppingMall | Amount billed at the shopping mall. | float64 | 0.0 |
| Spa | Amount billed at the spa. | float64 | 0.0 |
| VRDeck | Amount billed at the VR deck. | float64 | 0.0 |
| Deck | Cabin deck information. | object | B |
| Num | Cabin number. | object | 0 |
| Side | Cabin side (P for Port or S for Starboard). | object | P |
| Group | Group information from PassengerId. | object | 0001 |

## 가설
***
#### a. 짐에 대한 정보는 큰 영향을 미칠 것이다.
#### b. HomePlanet이나 Destination이 큰 영향을 미칠 것이다.
#### c. 지불금액이 큰 영향을 미칠 것이다.

## 분석 및 코드
[spaceship.ipynb](./spaceship.ipynb)

## 결과 및 해석
- 가설 a. "짐에 대한 정보는 큰 영향을 미칠 것이다."
    * 정확도: 0.5978337650105957
- 가설 b. "HomePlanet이나 Destination이 큰 영향을 미칠 것이다."
    * 정확도: 0.5852985160473945
- 가설 c. "지불금액이 큰 영향을 미칠 것이다."
    * 정확도: 0.7751064074542735

### 따라서 지불금액이 큰 영향을 미친다.