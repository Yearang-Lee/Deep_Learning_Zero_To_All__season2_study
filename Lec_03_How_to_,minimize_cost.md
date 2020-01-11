* Simplified hypothesis

​      Hypothesis :  H(x) = Wx

​      Cost : <img src="/image/3_0.png" style="zoom:0%;" />

<img src="/image/3_1.png" style="zoom:0%;" />

​                                                              => cost가 제일 작게 되는 w를 찾는 것



## Gradient descent algorithm

> 경사를 따라 내려가면서 최저점을 찾는 알고리즘



W와 b값을 랜덤 값으로 정해 --> Cost(W,b)가 작아지도록 업데이트 --> 최저점에 도달 할 때까지 반복



<img src="/image/3_2.png" style="zoom:0%;" />

​                                                      ====> "기울기 : +, W : - " 의 의미 : 기울기는 양수(+)이고,                            

​                                                                                                                  W는 작은 쪽(-)으로 움직인다.

## Gradient descent

> W(Weight)를 계속 수정하면서 업데이트하는 알고리즘



<img src="/image/3_3.png" style="zoom:0%;" />



   - learning rate : 기울기 값을 얼마만큼 반영해서 W에서 뺄지 결정하는 계수
     - ex) learning rate값이 크다면 큰 값을 빨리 빼서 크게 변할 것임 ( W의 값이 큰 폭으로 움직일 것임), 주로 0.001 같은 작은 값을 사용

미분하기 위해



  <img src="/image/3_4.png" style="zoom:0%;" />



 으로 변경

<img src="/image/3_5.png" style="zoom:0%;" />



