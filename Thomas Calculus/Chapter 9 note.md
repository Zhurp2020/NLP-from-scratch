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
### 9.3 Applications
#### Motion with Resistance Proportional to Velocity
$$
m\dfrac{dv}{dt} = -kv, k>0
$$
With initial conditions $v = v_0$  
$$
v = v_0e^{-\frac{k}{m}t}
$$
distance to stop:
$$
\dfrac{ds}{dt} = v_0e^{-\frac{k}{m}t}, s(0) = 0 \\
s = -\dfrac{mv_0}{k}e^{-\frac{k}{m}t}+C   \\
s(0) = -\dfrac{mv_0}{k} + C = 0 \\
s(t) = \dfrac{mv_0}{k}(1-e^{-\frac{k}{m}t}) \\
\lim_{t\to\infty}s(t) = \dfrac{mv_0}{k}
$$
#### Orthogonal Trajectories
An orthogonal trajectory of a family of curves is a curve that intersects each curve of the family at right angles, or orthogonally
#### Mixture Problems
### 9.4 Graphical Solutions of Autonomous Equations
#### Equilibrium Values and Phase Lines
A differential equation for which $\dfrac{dy}{dx}$ is a function of $y$ only is called an autonomous differential equation.  
> DEFINITION   
> If $\dfrac{dy}{dx} = g(y)$ is an autonomous differential equation, then the values of $y$ for which $\dfrac{dy}{dx} = 0$ are called equilibrium values or rest points.  

a phase line for the equation is a plot on the y-axis that shows the equation’s equilibrium values along with the intervals where $\dfrac{dy}{dx}$ and $\dfrac{d^2y}{dx^2}$ are positive and negative
#### Stable and Unstable Equilibria
#### Newton’s Law of Cooling
#### A Falling Body Encountering Resistance
#### Logistic Population Growth
### 9.5 Systems of Equations and Phase Planes
#### Phase Planes
$$
\dfrac{dx}{dt} = F(x,y) \\
\dfrac{dy}{dt} = G(x,y)
$$
#### A Competitive-Hunter Model
#### Limitations of the Phase-Plane Analysis Method
#### Another Type of Behavior