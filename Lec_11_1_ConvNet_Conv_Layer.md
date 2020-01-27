## Convolutional Neural Networks

<img src="/image/11_1.png" style="zoom:60%;" />

filter를 6개 적용 ==> 각 각의 filter는 weight가 다르기 때문에 값이 다 다르다.

===> 이렇게 나온 6개를 쌓은 게 오른 쪽 그림이다.



### Stride

<img src="/image/11_2.png" style="zoom:60%;" />

output size : <img src="/image/11_3.png" style="zoom:60%;" />

- ```Stride : 1``` :  5*5 output       ( ==> 25개의 점을 뽑아냈다.) 

- ```Stride : 2``` :  3*3 output       ( ==> 9개의 점을 뽑아냈다.) 

  

  

### Max pooling and Full Network

#### * Pooling layer (sampling)

<img src="/image/11_4.png" style="zoom:60%;" />

ex ) Max Pooling

<img src="/image/11_5.png" style="zoom:60%;" />

#### * Activation Function  ==> 이거 다음이 pooling

##### ReLU

<img src="/image/11_6.png" style="zoom:60%;" />

