# Thomas Calculus
## Chapter 13 Vector-Valued Functions and Motion in Space
### 13.1 Curves in Space and Their Tangents
#### Limits and Continuity
>**DEFINITION**    
Let $\mathbf{r}(t) = f(t)\mathbf{i} + g(t)\mathbf{j} + h(t)\mathbf{k}$ be a vector function with domain $D$, and let $L$ be a vector. We say that $\mathbf{r}$ has limit $\mathbf{L}$ as $t$ approaches $t_0$ and write  
>$$
>\lim_{t\to t_0}\mathbf{r}(t) = \mathbf{L}
>$$
>if, for every number $\varepsilon > 0$, there exists a corresponding number $\delta < 0$ such that for all $t\in D$
>$$
>|\mathbf{r}(t) - L| < \varepsilon\quad\mathsf{whenever}\quad0 < |t - t_0| < \delta
>$$

>**DEFINITION**   
A vector function $\mathbf{r}(t)$ is continuous at a point $t = t_0$ in its domain if $\lim\limits_{t\to t_0}\mathbf{r}(t) = \mathbf{r}(t_0)$. The function is continuous if it is continuous at every point in its domain.
#### Derivatives and Motion
>**DEFINITION**  
The vector function $\mathbf{r}(t) = f(t)\mathbf{i} + g(t)\mathbf{j} + h(t)\mathbf{k}$ has a derivative (is differentiable) at $t$ if $f, g,$ and $h$ have derivatives at $t$. The derivative is the vector function  
>$$
>\mathbf{r}'(t) = \dfrac{d\mathbf{r}}{dt}=\lim_{\Delta t\to 0}\dfrac{\mathbf{r}(t + \Delta t)}{\Delta t} = \dfrac{df}{dt}\mathbf{i} + \dfrac{dg}{dt}\mathbf{j} + \dfrac{dh}{dt}\mathbf{k}
>$$
#### Differentiation Rules
#### Vector Functions of Constant Length
### 13.2 Integrals of Vector Functions; Projectile Motion
#### Integrals of Vector Functions
>**DEFINITION**   
The indefinite integral of $\mathbf{R}$ with respect to $t$ is the set of all antiderivatives of $\mathbf{r}$, denoted by $\int \mathbf{r}(t) dt$. If $\mathbf{R}$ is any antiderivative of $\mathbf{R}$, then
>$$
>\int \mathbf{r}(t)dt = \mathbf{R}(t) + \mathbf{C}
>$$

>**DEFINITION**   
If the components of $\mathbf{r}(t) = f(t)\mathbf{i} + g(t)\mathbf{j} + h(t)\mathbf{k}$ are integrable
over $[a, b]$ , then so is $\mathbf{r}$, and the definite integral of $\mathbf{r}$ from $a$ to $b$ is 
>$$
>\int_a^b \mathbf{r}(t)dt = \int_a^b f(t)dt\mathbf{i} + \int_a^bg(t)dt\mathbf{j} + \int_a^bh(t)dt\mathbf{k}
>$$ 
#### The Vector and Parametric Equations for Ideal Projectile Motion
>Ideal Projectile Motion Equation
>$$
>\mathbf{r} = (v_0\cos\alpha)t\mathbf{i} + ((v_0\sin\alpha) t - \dfrac{1}{2}gt^2)\mathbf{j} 
>$$

>Height, Flight Time, and Range for Ideal Projectile Motion  
For ideal projectile motion when an object is launched from the origin over a horizontal surface with initial speed $v_0$ and launch angle $\alpha$   
Maximum height:
>$$
>y_{\max} = \dfrac{(v_0\sin\alpha)^2}{2g}
>$$
>Flight time:
>$$
>t = \dfrac{2v_0\sin\alpha}{g}
>$$
>Range:
>$$
>t = \dfrac{v_0^2}{g}\sin2\alpha
>$$
#### Projectile Motion with Wind Gusts
### 13.3 Arc Length in Space
#### Arc Length Along a Space Curve
>**DEFINITION** 
The length of a smooth curve $\mathbf{r}(t) = x(t)\mathbf{i} + y(t)\mathbf{j} + z(t)\mathbf{k}, a \le t \le b$  that is traced exactly once as $t$ increases from $t = a$ to $t = b$, is
>$$
>L = \int_a^b\sqrt{(\dfrac{dx}{dt})^2 + (\dfrac{dy}{dt})^2 + (\dfrac{dz}{dt})^2}dt
>$$  
>$$
>L = \int_a^b|\mathbf{v}|dt
>$$   

>Arc Length Parameter with Base Point $P(t_0)$
>$$
>s(t) = \int_{t_0}^t\sqrt{(x'(\tau))^2 + (y'(\tau))^2 + (z'(\tau))^2}d\tau = \int_{t_0}^t|\mathbf{v}(\tau)|d\tau
>$$ 
#### Speed on a Smooth Curve
#### Unit Tangent Vector
### 13.4 Curvature and Normal Vectors of a Curve
#### Curvature of a Plane Curve
>**DEFINITION** 
If $\mathbf{T}$ is the unit vector of a smooth curve, the curvature function of the curve is
>$$
>\kappa = |\dfrac{d\mathbf{T}}{ds}|
>$$ 

>Formula for Calculating Curvature  
If $\mathbf{r}(t)$ is a smooth curve, then the curvature is the scalar function
>$$
>\kappa = \dfrac{1}{|\mathbf{v}|}|\dfrac{d\mathbf{T}}{dt}|
>$$  
>where $\mathbf{T} = \dfrac{\mathbf{v}}{|\mathbf{v}|}$ is the unit tangent vector.


>**DEFINITION**  
At a point where $\kappa \ne 0$, the principal unit normal vector for a smooth curve in the plane is
>$$
>N = \dfrac{1}{\kappa}\dfrac{d\mathbf{T}}{dt}
>$$   

>Formula for Calculating $\mathbf{N}$  
If $\mathbf{r}(t)$ is a smooth curve, then the principal unit normal is
>$$
>N = \dfrac{\frac{d\mathbf{T}}{dt}}{|\frac{d\mathbf{T}}{dt}|}
>$$ 
>where $\mathbf{T} = \dfrac{\mathbf{v}}{|\mathbf{v}|}$ is the unit tangent vector.
#### Circle of Curvature for Plane Curves
#### Curvature and Normal Vectors for Space Curves
### 13.5 Tangential and Normal Components of Acceleration
#### The TNB Frame
#### Tangential and Normal Components of Acceleration
>**DEFINITION**  
If the acceleration vector is written as
>$$
>a = a_{\mathbf{T}}\mathbf{T} + a_{\mathbf{N}}\mathbf{N}
>$$ 
>then
>$$
>a_{\mathbf{T}} = \dfrac{d^s}{dt^2}= \dfrac{d}{dt}|\mathbf{v}|,a_{\mathbf{N}} = \kappa(\dfrac{ds}{dt})^2= \kappa|\mathbf{v}|^2
>$$ 
>are the tangential and normal scalar components of acceleration

>Formula for Calculating the Normal Component of Acceleration
>$$
>a_{\mathbf{N}} = \sqrt{|\mathbf{a}|^2 - a_{\mathbf{T}}^2}
>$$ 
#### Torsion
>**DEFINITION**  
Let $\mathbf{B} = \mathbf{T} \times \mathbf{N}$. The torsion function of a smooth curve is
>$$
>\tau = -\dfrac{d\mathbf{B}}{ds}\cdot \mathbf{N}
>$$ 
#### Formulas for Computing Curvature and Torsion
>Vector Formula for Curvature
>$$
>\kappa = \dfrac{|\mathbf{v}\times\mathbf{a}|}{|\mathbf{v}|^3}
>$$ 

>Formula for Torsion
>$$
>\tau = \dfrac{\left|\begin{array}{cccc}
    \dot{x} & \dot{y} & \dot{z} \\  
    \ddot{x} & \ddot{y} & \ddot{z} \\ 
    \dot{\ddot{x}} & \dot{\ddot{y}} & \dot{\ddot{z}} \\
    \end{array}\right|}{|\mathbf{v}\times\mathbf{a}|^2}
>$$ 