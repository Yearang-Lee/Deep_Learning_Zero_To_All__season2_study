다중 분류 클래스인 경우는 다음 그림과 같이 여러개의 선에 의해 데이터가 분류된다.

(A or not / B or not / C or not)

<img src="/image/6_1.png" style="zoom:70%;" />

행렬로 한 번에 합치면 다음과 같다.

<img src="/image/6_2.png" style="zoom:70%;" />

<img src="/image/6_3.png" style="zoom:70%;" />

## Softmax

<img src="/image/6_4.png" style="zoom:70%;" />

## Cost function

> cross entropy 이용

<img src="/image/6_5.png" style="zoom:70%;" />



`예측 값`과 `실제 값`의 차이를 이  `cross entropy`식을 이용해서 구한다.

<img src="/image/6_6.png" style="zoom:70%;" />

예측에 실패했기 때문에 `cross entropy`값 즉, cost function이 크게 나온다.



## [ Logistic cost ] vs [ Cross entropy ]

<img src="/image/6_7.png" style="zoom:70%;" />

## Cost function

<img src="/image/6_8.png" style="zoom:70%;" />

<img src="/image/d.png" style="zoom:30%;" />



 즉, 여러개의 training set 이 있으면 전체의 거리 D (차이) 를 합하고 평균을 내준 것이 'Loss' 이다.