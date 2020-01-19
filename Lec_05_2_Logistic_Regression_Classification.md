## Cost Function

<img src="/image/5_6.png" style="zoom:70%;" />



=> '빨간색 선' (차이)을 좁혀서 'cost=0'이 되는 선을 만드는 게 목표!



- H(x) = Wx + b일 때 cost function은

<img src="/image/5_8.png" style="zoom:70%;" />



- H(x)가 

<img src="/image/5_7.png" style="zoom:70%;" />일 때 cost function은 

<img src="/image/5_9.png" style="zoom:70%;" />



 ==> 어는 지점에서 시작 하는냐에 따라서 최저점이 달라질 수 있음. ( 최저점으로 global minimum을 찾고자하는 게 목표인데 local minimum으로 나올 수 있음 )

====> 그래서 convex(볼록)한 그래프를 가져야 한다.



## sigmoid함수의 Cost function => Convex하게 만들기

> y=1 일 때  :  C( H(x) , y ) = - log ( H(X) ) 
>
> y=0 일 때  :  C( H(x) , y ) = - log ( 1- H(X) ) 
>

 

1) 실제값 y = 1

- H(x) = 1, cost(1) = 0
- H(x) = 0, cost(0) = ∞       (=> 예측이 틀리니까 cost 값이 커짐)



<img src="/image/5_10.png" style="zoom:60%;" />

  2) 실제값 y = 0   

- H(x) = 0, cost(0) = 0
- H(x) = 1, cost(1) = ∞ 

<img src="/image/5_11.png" style="zoom:60%;" />

위 두 그래프를 합치면

 ##### C( H(x) , y ) = - y log ( H(X) ) - (1-y) log ( 1- H(X) )

-  y=1, C = - log ( H(X) )
-  y=0, C = - log (1-H(X) )

<img src="/image/d.png" style="zoom:30%;" />

이제 이 Cost Function을 이용하여 Cost를 최소화시키는 Gradient Descent 알고리즘 수행 ( Optimization)

<img src="/image/d.png" style="zoom:30%;" />

## Gradient Descent algorithm

<img src="/image/5_12.png" style="zoom:70%;" />







