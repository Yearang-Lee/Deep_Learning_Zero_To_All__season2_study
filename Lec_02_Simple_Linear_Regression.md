## Linear Regression

> 데이터에 잘 맞는 '직선' 
>
> 즉,  a와 b를 찾는 것 
>
> > - y =ax + b

![image-20200102184704861](C:\Users\student\AppData\Roaming\Typora\typora-user-images\image-20200102184704861.png)





## Hypothesis

> Which hypothesis is better? -> 이거 정하기 위해서 Cost함수 씀

  H(x) = Wx + b      

(W : Weight, b : bias)



## Cost

<img src="C:\Users\student\AppData\Roaming\Typora\typora-user-images\image-20200102185215483.png" alt="image-20200102185215483" style="zoom:80%;" />

#### H(x) - y

 (예측 값- 실제 값)

   => '빨간색 선'들의 합이 작을 수록 good!

   => 이 차이를 cost, lost, error 라고 함.

==> 어떻게 이 cost 값을 최소화할까?



## Cost function 

#### : error^2의 평균값

  H(x) = Wx + b 

<img src="C:\Users\student\AppData\Roaming\Typora\typora-user-images\image-20200102185411182.png" alt="image-20200102185411182" style="zoom:67%;" />



  => Cost함수를 최소화하는 W와 b를 찾는 것

​       (학습의 목적이기도 함)





