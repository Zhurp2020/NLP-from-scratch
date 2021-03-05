# Thomas Calculus
## Chapter 13 Vector-Valued Functions and Motion in Space
### 13.1 Curves in Space and Their Tangents
In Exercises 1–4, find the given limits.  
1. $\lim\limits_{t\to\pi}(\sin\dfrac{t}{2}\mathbf{i} + \cos\dfrac{2t}{3}\mathbf{j} + \dfrac{5t}{4}\mathbf{k})$   
   $\lim\limits_{t\to\pi}(\sin\dfrac{t}{2}\mathbf{i} + \cos\dfrac{2t}{3}\mathbf{j} + \dfrac{5t}{4}\mathbf{k})$  
   $=\mathbf{i} -\dfrac{1}{2}\mathbf{j} + \dfrac{5\pi}{4}\mathbf{k}$  
#### Motion in the Plane
In Exercises 5–8, $\mathbf{r}(t)$ is the position of a particle in the $xy$-plane at time $t$. Find an equation in $x$ and $y$ whose graph is the path of the particle. Then find the particle’s velocity and acceleration vectors at the given value of $t$.  

5. $\mathbf{r}(t) = (t + 1)\mathbf{i} + (t^2 -1)\mathbf{j}, t = 1$  
   $x = t + 1, y = t^2 -1$  
   $y = (x-1)^2 - 1 = x^2 -2x$  
   $\mathbf{v} = \dfrac{d\mathbf{r}}{dt} = \mathbf{i} + 2t\mathbf{j}, \mathbf{v}(1) = \mathbf{i} + 2\mathbf{j}$  
   $\mathbf{a} = \dfrac{d\mathbf{v}}{dt} = 2\mathbf{j}, \mathbf{a}(1) = 2\mathbf{j}$ 
#### Motion in Space
In Exercises 13–18, $\mathbf{r}(t)$ is the position of a particle in space at time $t$. Find the particle’s velocity and acceleration vectors. Then find the particle’s speed and direction of motion at the given value of $t$. Write the particle’s velocity at that time as the product of its speed and direction.  

13. $\mathbf{r}(t) = (t + 1)\mathbf{i} + (t^2 -1)\mathbf{j} + 2t\mathbf{k}, t = 1$  
   $\mathbf{v} = \dfrac{d\mathbf{r}}{dt} = \mathbf{i} + 2t\mathbf{j} + 2\mathbf{k}, \mathbf{v}(1) = \mathbf{i} + 2\mathbf{j} + 2\mathbf{k}$  
   $\mathbf{a} = \dfrac{d\mathbf{v}}{dt} = 2\mathbf{j}, \mathbf{a}(1) = 2\mathbf{j}$  
   $s = \sqrt{1 + 4 + 4 } = 3$  
   $d = \dfrac{1}{3}\mathbf{i} + \dfrac{2}{3}\mathbf{j} + \dfrac{2}{3}\mathbf{k}$
#### Tangents to Curves
As mentioned in the text, the tangent line to a smooth curve $\mathbf{r}(t) = f(t)\mathbf{i} + g(t)\mathbf{j} + h(t)\mathbf{k}$ at $t = t_0$ is the line that passes through the point $(f(t0), g(t_0), h(t_0))$ parallel to $\mathbf{v}(t_0),$ the curve’s velocity vector at $t_0$. In Exercises 23–26, find parametric equations for the line that is tangent to the given curve at the given parameter value $t = t_0$   

23.  $\mathbf{r}(t) =\sin t\mathbf{i} + (t^2 - \cos t)\mathbf{j} + e^t\mathbf{k}, t_0 = 0$  
     $\mathbf{v}(t) = \cos t\mathbf{i} + (2t + \sin t)\mathbf{j} + e^t\mathbf{k}$    
     $\mathbf{v}(t_0) = \mathbf{i} + \mathbf{k}$  
     $P(0,-1,1)$  
     $x = t\mathbf{i}, y = -1, j = 1 + t\mathbf{k}$
#### Theory and Examples
37. Motion along a circle Each of the following equations in parts (a)–(e) describes the motion of a particle having the same path, namely the unit circle $x^2 + y^2 = 1$. Although the path of each particle in parts (a)–(e) is the same, the behavior, or “dynamics,” of each particle is different. For each particle, answer the following questions.  
 i) Does the particle have constant speed? If so, what is its constant speed?   
 ii) Is the particle’s acceleration vector always orthogonal to its velocity vector?   
 iii) Does the particle move clockwise or counterclockwise around the circle?  
 iv) Does the particle begin at the point $(1, 0)$?  
 a) $\mathbf{r}(t) =\cos t\mathbf{i} + \sin t\mathbf{j}, t \ge 0$  
 b) $\mathbf{r}(t) =\cos 2t\mathbf{i} + \sin 2t\mathbf{j}, t \ge 0$  
 c) $\mathbf{r}(t) =\cos (t - \dfrac{\pi }{2})\mathbf{i} + \sin (t - \dfrac{\pi }{2}\mathbf{j}, t \ge 0$  
 d) $\mathbf{r}(t) =\cos t\mathbf{i} - \sin t\mathbf{j}, t \ge 0$  
 e) $\mathbf{r}(t) =\cos t^2\mathbf{i} + \sin t^2\mathbf{j}, t \ge 0$  
 a) No, No,Counterclockwise,Yes  
 b) No,No, counterclockwise, Yes  
 c) $\mathbf{r}(t) =\sin t \mathbf{i} - \cos t \mathbf{j}, t \ge 0$   
 No,No, counterclockwise, No   
 d) No, No, clockwise, Yes  
 e) No,   
 $\mathbf{v}(t) =-2t\sin t^2 \mathbf{i} + 2t\cos t^2 \mathbf{j}$  
 $\mathbf{a}(t) =(-4t^2\cos t^2 - 2\sin t^2)\mathbf{i} + (4t^2\sin t^2 + 2\cos t^2) \mathbf{j}$  
 No, counterclockwise, yes
#### COMPUTER EXPLORATIONS
Use a CAS to perform the following steps in Exercises 49–52.  
a. Plot the space curve traced out by the position vector $\mathbf{r}$.
b. Find the components of the velocity vector $\dfrac{d\mathbf{r}}{dt}$.    
c. Evaluate $\dfrac{d\mathbf{r}}{dt}$ at the given point $t_0$ and determine the equation of the tangent line to the curve at $\mathbf{r}(t_0).$  
d. Plot the tangent line together with the curve over the given interval.  

49. $\mathbf{r}(t) =(\sin t - t\cos t)\mathbf{i} + (\cos t + t\sin t )\mathbf{j} + t^2 \mathbf{k},0 \le t \le 6\pi t_0 = \dfrac{3}{2}\pi$  
    $\mathbf{v}(t) =[\cos t - (-t\sin t + \cos t)] \mathbf{i} + (-\sin t - t\cos t + \sin t)\mathbf{j} + 2t \mathbf{k}$  
    $=t \sin t \mathbf{i} -t\cos t \mathbf{j} +  2t \mathbf{k}$  
    $\mathbf{v}(t)(\dfrac{3}{2}\pi) =-\dfrac{3}{2}\pi \mathbf{i} + 3\pi \mathbf{k}$  
    $x = 1  -\dfrac{3}{2}\pi t\mathbf{i}, y =-\dfrac{3}{2}\pi, z = \dfrac{9}{4}\pi^2 + 3\pi t \mathbf{k}$  
### 13.2 Integrals of Vector Functions; Projectile Motion
#### Integrating Vector-Valued Functions
Evaluate the integrals in Exercises 1–10.
1. $\int_0^1t^3\mathbf{i} + 7\mathbf{j} + (t + 1)\mathbf{k}dt$  
   $\int_0^1t^3\mathbf{i} + 7\mathbf{j} + (t + 1)\mathbf{k}dt$  
   $=[\dfrac{1}{4}t^4]_0^1\mathbf{i} + [7t]_0^1\mathbf{j} + [\dfrac{1}{2}t^2 + t]_0^1\mathbf{k}$   
   $= \mathbf{i} + 7\mathbf{j} + \dfrac{3}{2}\mathbf{k}$
#### Initial Value Problems
Solve the initial value problems in Exercises 11–20 for $\mathbf{r}$ as a vector function of $t$

11. Differential equation: $\dfrac{d\mathbf{r}}{dt}= -t\mathbf{i} -t \mathbf{j} -t\mathbf{k}$  
    Initial condition: $\mathbf{r}(0) =\mathbf{i} + 2\mathbf{j} + 3 \mathbf{k}$   
    $\int -t\mathbf{i} -t \mathbf{j} -t\mathbf{k}dt = -\dfrac{1}{2}t^2\mathbf{i} -\dfrac{1}{2}t^2\mathbf{j} -\dfrac{1}{2}t^2\mathbf{k} + \mathbf{C}$  
    $\mathbf{r}(0) = \mathbf{C} = \mathbf{i} + 2\mathbf{j} + 3 \mathbf{k}$  
    $\mathbf{r}(t) = (1 -\dfrac{1}{2}t^2)\mathbf{i} + (2 -\dfrac{1}{2}t^2)\mathbf{j} + (3 -\dfrac{1}{2}t^2) \mathbf{k}$
#### Motion Along a Straight Line
21. At time $t = 0$, a particle is located at the point $(1, 2, 3)$. It travels in a straight line to the point $(4, 1, 4)$, has speed $2$ at $(1, 2, 3)$ and constant acceleration $3\mathbf{i} -\mathbf{j} + \mathbf{k}$. Find an equation for the position vector $\mathbf{r}(t)$ of the particle at time $t$   
    $\mathbf{v}(t) = \int 3\mathbf{i} -\mathbf{j} +\mathbf{k}dt = 3t\mathbf{i} -t\mathbf{j} + t\mathbf{k} + \mathbf{C}$   
    $\mathbf{v}(0) = \mathbf{C}$  
    $\dfrac{\mathbf{v}(0)}{|\mathbf{v}(0)|} = \dfrac{\mathbf{C}}{2}=  \dfrac{3}{\sqrt{11}}\mathbf{i} -\dfrac{1}{\sqrt{11}}\mathbf{j} + \dfrac{1}{\sqrt{11}}\mathbf{k}$  
    $\mathbf{C} = \dfrac{6}{\sqrt{11}}\mathbf{i} -\dfrac{2}{\sqrt{11}}\mathbf{j} + \dfrac{2}{\sqrt{11}}\mathbf{k}$  
    $\mathbf{v}(t) = (3t + \dfrac{6}{\sqrt{11}})\mathbf{i} -(t + \dfrac{2}{\sqrt{11}})\mathbf{j} + (t + \dfrac{2}{\sqrt{11}})\mathbf{k}$  
    $\mathbf{r}(t) = (\dfrac{3}{2}t^2 + \dfrac{6}{\sqrt{11}}t)\mathbf{i} -(\dfrac{1}{2}t^2 + \dfrac{2}{\sqrt{11}}t)\mathbf{j} + (\dfrac{1}{2}t^2 + \dfrac{2}{\sqrt{11}}t)\mathbf{k} + \mathbf{C}$  
    $\mathbf{r}(0) = \mathbf{C} = \mathbf{i} +2\mathbf{j} + 3\mathbf{k}$   
    $\mathbf{r}(t) = (\dfrac{3}{2}t^2 + \dfrac{6}{\sqrt{11}}t + 1)\mathbf{i} -(\dfrac{1}{2}t^2 + \dfrac{2}{\sqrt{11}}t -2)\mathbf{j} + (\dfrac{1}{2}t^2 + \dfrac{2}{\sqrt{11}}t + 3)\mathbf{k} + \mathbf{C}$ 
#### Projectile Motion
Projectile flights in the following exercises are to be treated as ideal unless stated otherwise. All launch angles are assumed to be measured from the horizontal. All projectiles are assumed to be launched from the origin over a horizontal surface unless stated otherwise.

23. travel time. A projectile is fired at a speed of 840 m/sec at an angle of 60°. How long will it take to get 21 km downrange?   
    $420 t = 21000, t =50s$
#### Projectile Motion with Linear Drag
The main force affecting the motion of a projectile, other than gravity, is air resistance. This slowing down force is drag force, and it acts in a direction opposite to the velocity of the projectile (see accompanying figure). For projectiles moving through the air at relatively low speeds, however, the drag force is (very nearly) proportional to the speed (to the first power) and so is called linear.  
![](../images/Thomas%20Calculus/13-1.jpg)  

41. Linear drag Derive the equations  
    $$
    x = \dfrac{v_0}{k}(1-e^{-kt})\cos \alpha \\
    y = \dfrac{v_0}{k}(1-e^{-kt})\sin \alpha + \dfrac{g}{k^2}(1 - kt - e^{-kt})
    $$  
    by solving the following initial value problem for a vector $\mathbf{r}$ in the plane.
    Differential equation $\dfrac{d^2\mathbf{r}}{dt^2}= -g\mathbf{j} -k\mathbf{v} = -g\mathbf{j} -k\dfrac{d\mathbf{r}}{dt}$  
    Initial conditions $\mathbf{r}(0) = 0$  
    $\dfrac{d\mathbf{r}}{dt}|_{t = 0}= v_0\cos\alpha\mathbf{i} + v_0\sin\alpha\mathbf{j}$  
    The drag coefficient $k$ is a positive constant representing resistance due to air density, $v_0$ and $\alpha$ are the projectile’s initial speed and launch angle, and $g$ is the acceleration of gravity.  
    $\dfrac{d\mathbf{v}}{dt} = -g\mathbf{j} -k\mathbf{v}$  
    $\dfrac{dx}{dt} = -kx$  
    $\dfrac{dy}{dt} = -g-ky$  
    $\dfrac{dx}{dt}  e^{\int kdt}+kxe^{\int kdt}= 0, \dfrac{d}{dt}e^{\int kdt} = ke^{kt}$  
    $\dfrac{dx}{dt}e^{kt} + \dfrac{d}{dt}e^{kt}x = 0$  
    $\dfrac{d}{dt}e^{kt}x = 0$  
    $e^{kt}x = C, x = \dfrac{C}{e^{kt}}$  
    $\dfrac{dy}{dt}  e^{\int kdt}+kxe^{\int kdt}= -ge^{kt}, \dfrac{d}{dt}e^{\int kdt} = ke^{kt}$  
    $\dfrac{dy}{dt}e^{kt} + \dfrac{d}{dt}e^{kt}y = -ge^{kt}$  
    $\dfrac{d}{dt}e^{kt}y = -ge^{kt}$  
    $e^{kt}y = -g\dfrac{1}{k}e^{kt} + C, y = -\dfrac{g}{k} + \dfrac{C}{e^{kt}}$  
    $x(0) = C = v_0\cos\alpha$  
    $y(0) = -\dfrac{g}{k} + C = v_0\sin\alpha$  
    $x = \int \dfrac{v_0\cos\alpha}{e^{kt}}dt$  
    $= -\dfrac{v_0\cos\alpha}{k}e^{-kt} + C$  
    $x(0) = -\dfrac{v_0\cos\alpha}{k} + C = 0, C= \dfrac{v_0\cos\alpha}{k}$  
    $y = \int -\dfrac{g}{k} + \dfrac{v_0\sin\alpha + \frac{g}{k}}{e^{kt}}dt$  
    $= -\dfrac{g}{k}t - \dfrac{v_0\sin\alpha + \frac{g}{k}}{k}e^{-kt} + C$  
    $y(0) = -\dfrac{v_0\sin\alpha + \frac{g}{k}}{k} + C = 0$  
    $x =\dfrac{v_0}{k}(1-e^{-kt})\cos\alpha$  
    $y = -\dfrac{g}{k}t + \dfrac{kv_0\sin\alpha + g}{k^2}(1-e^{-kt})$    
    $= \dfrac{v_0}{k}(1-e^{-kt})\sin\alpha + \dfrac{g}{k^2}(1-kt - e^{-kt})$
#### Theory and Examples
43. Establish the following properties of integrable vector functions.  
    a. The Constant Scalar Multiple Rule  
    $$
    \int_a^bk\mathbf{r}(t)dt = k\int_a^b\mathbf{r}(t)dt
    $$
    (any scalar $k$)  
    The Rule for Negatives,  
    $$
    \int_a^b-\mathbf{r}(t)dt = -\int_a^b\mathbf{r}(t)dt
    $$
    is obtained by taking $k = -1.$  
    b. The Sum and Difference Rules:  
    $$
    \int_a^b\mathbf{r}_1(t)\pm\mathbf{r}_2(t)dt = \int_a^b\mathbf{r}_1(t)dt \pm \int_a^b\mathbf{r}_2(t)dt
    $$  
    c. The Constant Vector Multiple Rules:  
    $$
    \int_a^b\mathbf{C}\cdot\mathbf{r}(t)dt = \mathbf{C}\cdot\int_a^b\mathbf{r}(t)dt
    $$  
    and 
    $$
    \int_a^b\mathbf{C}\times\mathbf{r}(t)dt = \mathbf{C}\times\int_a^b\mathbf{r}(t)dt
    $$  
    a. $\int_a^bk\mathbf{r}(t)dt =\int_a^bkf(t)dt\mathbf{i} + \int_a^bkg(t)dt\mathbf{j}$    
    $= k(\int_a^bf(t)dt\mathbf{i} + \int_a^bg(t)dt\mathbf{j})$  
    $= k\int_a^b\mathbf{r}(t)dt$  
    b. $\int_a^b\mathbf{r}_1(t)\pm\mathbf{r}_2(t)dt$  
    $= \int_a^bf_1(t)dt\mathbf{i} + \int_a^bg_1(t)dt\mathbf{j} \pm \int_a^bf_2(t)dt\mathbf{i} + \int_a^bg_2(t)dt\mathbf{j}$  
    $= (\int_a^bf_1(t)dt \pm \int_a^bf_2(t)dt)\mathbf{i} + (\int_a^bg_1(t)dt\pm \int_a^bg_2(t)dt)\mathbf{j}$  
    $= \int_a^bf_1(t)dt\mathbf{i} + \int_a^bg_1(t)dt\mathbf{j} \pm \int_a^bf_2(t)dt\mathbf{i} + \int_a^bg_2(t)dt\mathbf{j}$  
    $= \int_a^b\mathbf{r}_1(t)dt \pm \int_a^b\mathbf{r}_2(t)dt$  
    c. $\int_a^b\mathbf{C}\cdot\mathbf{r}(t)dt$  
    $= \int_a^bmf(t)dt\mathbf{i} + \int_a^bng(t)dt\mathbf{j}$  
    $= (m\mathbf{i} + n\mathbf{j})\cdot(\int_a^bf(t)dt\mathbf{i} + \int_a^bg(t)dt\mathbf{j})$  
    $= \mathbf{C}\cdot\int_a^b\mathbf{r}(t)dt$   
    $\int_a^b\mathbf{C}\times\mathbf{r}(t)dt =\int_a^b|\begin{array}{cccc}\mathbf{i}&\mathbf{j}&\mathbf{k} \\ m&n&p\\f(t)&g(t)&h(t)\end{array}|dt$   
    $= \int_a^b(nh(t)-pg(t))\mathbf{i}+(mh(t)-pf(t))\mathbf{j}+(mg(t)-nf(t))\mathbf{k}dt$  
    $\mathbf{C}\times\int_a^b\mathbf{r}(t)dt$   
    $= |\begin{array}{cccc}\mathbf{i}&\mathbf{j}&\mathbf{k} \\ m&n&p\\\int_a^bf(t)dt&\int_a^bg(t)dt&\int_a^bh(t)dt\end{array}|$  
    $= (n\int_a^bh(t)dt-p\int_a^bg(t)dt)\mathbf{i}+(m\int_a^bh(t)dt-p\int_a^bf(t)dt)\mathbf{j}+(m\int_a^bg(t)dt-n\int_a^bf(t)dt)\mathbf{k}$  
    $= \int_a^b\mathbf{C}\times\mathbf{r}(t)dt$
### 13.3 Arc Length in Space
#### Finding Tangent Vectors and Lengths
In Exercises 1–8, find the curve’s unit tangent vector. Also, find the length of the indicated portion of the curve.  
1. $\mathbf{r}(t) = (2\cos t)\mathbf{i} + 2\sin t\mathbf{j} + \sqrt{5}t\mathbf{k}, 0 \le t \le \pi$  
   $\mathbf{v}(t) = (-2\sin t)\mathbf{i} + 2\cos t\mathbf{j} + \sqrt{5}\mathbf{k}$  
   $|\mathbf{v}(t)| = \sqrt{4 + 5} = 3$   
   $\mathbf{T} = (-\dfrac{2}{3}\sin t)\mathbf{i} + \dfrac{2}{3}\cos t\mathbf{j} + \dfrac{\sqrt{5}}{3}\mathbf{k}$  
   $L = \int_0^{\pi}3dt = 3\pi$
#### Arc Length Parameter
In Exercises 11–14, find the arc length parameter along the curve from the point where $t = 0$ by evaluating the integral  
$$
s = \int_0^t|\mathbf{v}(\tau)|d\tau
$$   
from Equation (3). Then find the length of the indicated portion of the curve.  

11. $\mathbf{r}(t) = (4\cos t)\mathbf{i} + 4\sin t\mathbf{j} + 3t\mathbf{k}, 0 \le t \le \dfrac{\pi}{2}$  
    $\mathbf{v}(t) = (-4\sin t)\mathbf{i} + 4\cos t\mathbf{j} + 3\mathbf{k}$  
    $|\mathbf{v}| = 5$  
    $\int_0^{\frac{\pi}{2}}5d\tau = \dfrac{5}{2}\pi$
#### Theory and Examples
15. Arc length Find the length of the curve  
    $$
    \mathbf{r}(t) = \sqrt{2}t\mathbf{i} + \sqrt{2}t\mathbf{j} + (1 - t^2)\mathbf{k}
    $$  
    from $(0, 0, 1)$ to $(\sqrt{2},\sqrt{2},0)$.  
    $0 \le t \le 1$  
    $\mathbf{v}(t) = \sqrt{2}\mathbf{i} + \sqrt{2}\mathbf{j}  - 2t\mathbf{k}$  
    $|\mathbf{v}| = \sqrt{4 + 4t^2}$  
    $L = 2\int_0^1\sqrt{1 + t^2}dt$  
    Let $u = \sqrt{1 + t^2}, \dfrac{du}{dt} = \dfrac{1}{2\sqrt{1 + t^2}} = \dfrac{1}{2u}$   
    $= 2\int_1^{\sqrt{2}}2u^2du$  
    $= 4[\dfrac{1}{3}u^3]_1^{\sqrt{2}}$  
    $= \dfrac{8}{3}\sqrt{2}-\dfrac{4}{3}$
### 13.4 Curvature and Normal Vectors of a Curve
#### Plane Curves
Find $\mathbf{T}, \mathbf{N},$ and $\kappa$ for the plane curves in Exercises 1–4.
1. $\mathbf{r}(t) = t\mathbf{i} + \ln(\cos t)\mathbf{j}, -\dfrac{\pi}{2} < t < \dfrac{\pi}{2}$  
   $\mathbf{v}(t) = \mathbf{i} -\dfrac{\sin t}{\cos t}\mathbf{j} = \mathbf{i} -\tan t\mathbf{j}$   
   $\mathbf{T}(t) = \dfrac{1}{\sqrt{\tan ^2 t + 1}}\mathbf{i} -\dfrac{\tan t}{\sqrt{\tan ^2 t + 1}}\mathbf{j} = \dfrac{1}{\sec t}\mathbf{i} -\dfrac{\tan t}{\sec t}\mathbf{j} = \cos t\mathbf{i} -\sin t\mathbf{j}$  
   $\mathbf{N}(t) =\dfrac{-\sin t\mathbf{i} -\cos t\mathbf{j}}{1} = -\sin t\mathbf{i} -\cos t\mathbf{j}$  
   $\kappa =\dfrac{1}{\sqrt{1 + \tan^2t}} = \cos t$  
#### Space Curves
Find $\mathbf{T}, \mathbf{N},$ and $\kappa$ for the space curves in Exercises 9–16.

9. $\mathbf{r}(t) = 3\sin t\mathbf{i} + 3\cos t\mathbf{j} + 4t\mathbf{k}$  
   $\mathbf{v}(t) = 3\cos t\mathbf{i} -3\sin t\mathbf{j} + 4\mathbf{k}$  
   $\mathbf{T}(t) = \dfrac{3}{5}\cos t\mathbf{i} - \dfrac{3}{5}\sin t\mathbf{j} +  \dfrac{4}{5}\mathbf{k}$   
   $\mathbf{N}(t) = \dfrac{-\frac{3}{5}\sin t\mathbf{i} - \frac{3}{5}\cos t\mathbf{j}}{\frac{3}{5}} =-\sin t\mathbf{i} - \cos t\mathbf{j}$  
   $\kappa = \dfrac{1}{5}\dfrac{3}{5} = \dfrac{3}{25}$ 
#### More on Curvature
17. Show that the parabola $y = ax^2, a \ne 0$, has its largest curvature at its vertex and has no minimum curvature. (Note: Since the curvature of a curve remains the same if the curve is translated or rotated, this result is true for any parabola.)  
    $\mathbf{v}(t) = \mathbf{i} -2at\mathbf{j}$  
    $\mathbf{T}(t) = \dfrac{1}{\sqrt{1 + 4a^2t^2}}\mathbf{i} -\dfrac{2at}{\sqrt{1 + 4a^2t^2}}\mathbf{j}$  
    $\dfrac{d\mathbf{T}}{dt} =  -\dfrac{4a^2t}{(1 + 4a^2t^2)^{\frac{3}{2}}}\mathbf{i} -(-\dfrac{8a^3t^2}{(1 + 4a^2t^2)^{\frac{3}{2}}} + \dfrac{2a}{\sqrt{1 + 4a^2t^2}})\mathbf{j}$  
    $|\dfrac{d\mathbf{T}}{dt}|^2 = \dfrac{16a^4t^2}{(1 + 4a^2t^2)^3} + (\dfrac{4a^2}{1 + 4a^2t^2} - \dfrac{32a^4t^2}{(1 + 4a^2t^2)^2} + \dfrac{64a^6t^4}{(1 + 4a^2t^2)^3})$  
    $= \dfrac{16a^4t^2 + 64a^6t^4}{(1 + 4a^2t^2)^3} +  \dfrac{4a^2 + 16a^4t^2 -32a^4t^2}{(1 + 4a^2t^2)^2}$  
    $= \dfrac{16a^4t^2}{(1 + 4a^2t^2)^2} +  \dfrac{4a^2 - 16a^4t^2}{(1 + 4a^2t^2)^2}$  
    $|\dfrac{d\mathbf{T}}{dt}| = \dfrac{2a}{1 + 4a^2t^2}$  
    $\kappa = \dfrac{1}{\sqrt{1 + 4a^2t^2}}\dfrac{2a}{1 + 4a^2t^2} = \dfrac{2a}{(1 + 4a^2t^2)^{\frac{3}{2}}}$  
    $\dfrac{d\kappa}{dt} = -\dfrac{24a^3t}{(1 + 4a^2t^2)^{\frac{5}{2}}} = 0, t = 0$   
    $t < 0, \kappa < 2a, t > 0, \kappa >2a$  
    $\kappa_{max} = 2a$  
### COMPUTER EXPLORATIONS
In Exercises 31–38 you will use a CAS to explore the osculating circle at a point $P$ on a plane curve where $\kappa \ne 0$. Use a CAS to perform the following steps:  
a. Plot the plane curve given in parametric or function form over the specified interval to see what it looks like.  
b. Calculate the curvature $\kappa$ of the curve at the given value $t_0$ using the appropriate formula from Exercise 5 or 6. Use the parametrization $x = t$ and $y = f(t)$ if the curve is given as a function $y = f(x)$.  
c. Find the unit normal vector $\mathbf{N}$ at $t_0$ . Notice that the signs of the components of $\mathbf{N}$ depend on whether the unit tangent vector $\mathbf{t}$ is turning clockwise or counterclockwise at $t = t_0$. (See Exercise 7.)  
d. If $\mathbf{C} = a\mathbf{i} + b\mathbf{j}$ is the vector from the origin to the center $(a, b)$ of the osculating circle, find the center $\mathbf{C}$ from the vector equation  
$$
\mathbf{C} = \mathbf{r}(t_0) + \dfrac{1}{\kappa(t_0)}\mathbf{N}(t_0)
$$
The point $P(x_0, y_0)$ on the curve is given by the position vector $\mathbf{r}(t_0)$.  
e. Plot implicitly the equation $(x - a)^2 + (y - b)^2 =\dfrac{1}{\kappa^2}$ of the osculating circle. Then plot the curve and osculating circle together. You may need to experiment with the size of the viewing window, but be sure the axes are equally scaled.  

31. $\mathbf{r}(t) = 3\cos t\mathbf{i} + 5\sin t\mathbf{j}, 0 \le t \le 2\pi, t_0 = \dfrac{\pi}{4}$  
    $\kappa = \dfrac{|15\sin^2 t  + 15\cos^2 t|}{(9\sin^2 t+ 25\cos^2t)^{\frac{3}{2}}} =\dfrac{15}{17\sqrt{17}}$    
    $\mathbf{N} = -5\cos t \mathbf{i} - 3\sin t\mathbf{j} = -\dfrac{5}{2}\sqrt{2}\mathbf{i} - \dfrac{3}{2}\sqrt{2}\mathbf{j}$  
    $\mathbf{C} = \dfrac{3}{2}\sqrt{2}\mathbf{i} + \dfrac{5}{2}\sqrt{2}\mathbf{j} + \dfrac{17\sqrt{17}}{15}(-\dfrac{5}{2}\sqrt{2}\mathbf{i} - \dfrac{3}{2}\sqrt{2}\mathbf{j})$  
    $= \dfrac{15\sqrt{2}-85\sqrt{34}}{30}\mathbf{i} + \dfrac{75\sqrt{2}-51\sqrt{34}}{30}\mathbf{j}$