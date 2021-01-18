# Thomas Calculus
## Chapter 9 First-Order Differential Equations
### 9.1 Solutions, Slope Fields, and Euler’s Method
#### General First-Order Differential Equations and Solutions
A first-order differential equation is an equation
$$
\dfrac{dy}{dx} = f(x,y)
$$
#### Slope Fields: Viewing Solution Curves
#### Euler’s Method
### 7.2 First-Order Linear Equations
$$
\dfrac{dy}{dx} + P(x)y = Q(x)
$$
#### Solving Linear Equations
Chose $v(x)$ such that 
$$
v(x)\dfrac{dy}{dx}+P(x)v(x)y = \dfrac{d}{dx}(v(x)y)  \\
v(x)\dfrac{dy}{dx}+P(x)v(x)y = Q(x)v(x) \\
\dfrac{d}{dx}(v(x)y) =  Q(x)v(x) \\
v(x)y = \int Q(x)v(x) dx\\
y = \dfrac{1}{v(x)}\int  Q(x)v(x) dx\\
v(x)\dfrac{dy}{dx}+P(x)v(x)y = \dfrac{d}{dx}(v(x)y)  \\
v(x)\dfrac{dy}{dx}+P(x)v(x)y = y\dfrac{dv}{dx} + v(x)\dfrac{dy}{dx} \\
\dfrac{dv}{dx} = P(x)v(x) \\
\dfrac{dv}{v(x)} = P(x)dx \\
\int \dfrac{1}{v(x)}dv = \int P(x)dx \\
\ln v(x) = \int P(x)dx \\
v(x) = e^{\int P(x)dx}
$$
#### $RL$ Circuits
![](../images/Thomas%20Calculus/9-1.jpg)  
$$
L\dfrac{di}{dt} + Ri = V 
$$