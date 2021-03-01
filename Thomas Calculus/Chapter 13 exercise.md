# Thomas Calculus
## Chapter 13 Vector-Valued Functions and Motion in Space
### 13.1 Curves in Space and Their Tangents
In Exercises 1–4, find the given limits.  
1. $\lim\limits_{t\to\pi}(\sin\dfrac{t}{2}\mathbf{i} + \cos\dfrac{2t}{3}\mathbf{j} + \dfrac{5t}{4}\mathbf{k})$   
   $\lim\limits_{t\to\pi}(\sin\dfrac{t}{2}\mathbf{i} + \cos\dfrac{2t}{3}\mathbf{j} + \dfrac{5t}{4}\mathbf{k})$  
   $=\lim\limits_{t\to\pi}(\sin\dfrac{t}{2}\mathbf{i} + \cos\dfrac{2t}{3}\mathbf{j} + \dfrac{5t}{4}\mathbf{k}$  
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

