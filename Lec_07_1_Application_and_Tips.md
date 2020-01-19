- Learning rate
  - Gradient
  - Learning rate
- Data preprocessing
  - Standardization
  - Normalization
  - Noisy Data
- Overfitting
  - Regularization
  - L1, L2 Norm



## Learning rate

<img src="/image/7_1.png" style="zoom:60%;" />

- 너무 크면(overshooting) : 밖으로 튕겨나가서 학습이 잘 안 되고, cost 함수가 숫자가 아닌 값이 나온다.
- 너무 작으면 : 최저점이 아닌 곳에서 멈출 수도 있다.
- 일반적인 Learning rate : 0.01



## Data preprocessing_(Feature Scaling)

<img src="/image/7_2.png" style="zoom:70%;" />

​              실제 데이터는 이 부분에 밀집되어 있다.  ==========>     0~1사이의 숫자로 표현



- Standardization ( 평균에서 얼만큼 멀어 졌나 )

​       <img src="/image/7_3.png" style="zoom:50%;" />

- Normalization ( 0 ~ 1)

  <img src="/image/7_4.png" style="zoom:50%;" /> 

  

  ## Overfitting

  > 데이터에 맞게 선(decision boundary)을 구부려서 그리는 거 => Regularization : 구부리지 말고 핀다.(weight를 최소화한다.)

  <img src="/image/7_5.png" style="zoom:70%;" />



### Overfitting 줄이는 법

- training data를 많이 가지고 한다.

- feature의 개수(ex.중복 값)를 줄인다. (or 너무 적을 경우에는 늘린다.

  => 차원 축소(PCA)

  <img src="/image/7_6.png" style="zoom:50%;" /> 

  

- Regularization (Add term to loss)
- Dropout(0.5 is common)
- Batch Normalization