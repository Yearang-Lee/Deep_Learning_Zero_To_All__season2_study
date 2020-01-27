## Relu activation function

#### Problem of sigmoid

```Input  => Network => Output```

<=======================Backpropagation

> Backpropagation

: loss를 미분한 것을 backpropagation하면서 Network를 학습을 시킨다.

이 때, backpropagation으로 전달되는 loss를 미분한 것이 ```gradient```(그래프 기울기)이다.

```d(loss) = gradient```

##### * Sigmoid Function



<img src="/image/10_1.png" style="zoom:60%;" /> 

이 부분은 ```gradient```값이 0에 매우 가까운(매우 작은)값을 가짐

<img src="/image/d.png" style="zoom:60%;" />

NN이 학습할 때 ```gradient```를 전달받아서 그걸 이용해서 학습을 하는 데 너무 작으면 안 된다.

<img src="/image/d.png" style="zoom:60%;" />

그런데 sigmoid함수는 위 그림처럼 ```gradient```가 0에 가까워져서 전달 받은 ```gradient```가 없어지게 된다. 

 ==> Vanishing Gradient



#### ReLU Function

>  f(x) = max( 0, x )
>
> ==> x가 0보다 크면 x, 작으면 0

<img src="/image/10_2.png" style="zoom:60%;" />

## Weight Initialization

<img src="/image/10_3.png" style="zoom:60%;" />

이렇게 단순한 형태이면 minimum을 한 번에 찾을 수 있지만

<img src="/image/10_4.png" style="zoom:60%;" />

이 경우는 초기 값이 어디냐에 따라 minimum이 달라질 수 있다.

<img src="/image/d.png" style="zoom:60%;" />

```Weight Initialization``` 해야 한다. ( 어디서 출발할지 설정해야 한다.)

- Xavier Initialization
- He Initialization ( Relu 함수에 특화된 초기화 방법)



## Dropout

> under-fitting이나 over-fitting이 되지 않게  도와주는 regularization

<img src="/image/10_5.png" style="zoom:60%;" />

Train할 때는 일부 노드만 가지고 학습하고 Test할 때는 모든 노드를 사용한다.