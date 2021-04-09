# Thomas Calculus
## Chapter 16 Integrals and Vector Fields
### 16.1 Line Integrals of Scalar Functions
#### Graphs of Vector Equations
Match the vector equations in Exercises 1–8 with the graphs (a)–(h) given here.
![](../images/Thomas%20Calculus/16-1.jpg)  
1. $\mathbf{r}(t) =t\mathbf{i} + (1-t)\mathbf{j},0\le t \le 1$  '
   c. 
#### Evaluating Line Integrals over Space Curves
9. Evaluate $\int_C(x + y) ds$ where $C$ is the straight-line segment  $x = t, y = (1 - t), z = 0,$ from $(0, 1, 0)$ to $(1, 0, 0).$  
    $\int_C(x + y) ds$  
    $=\int_0^1(t+1-t)\sqrt{2}dt=\sqrt{2}$
#### Line Integrals over Plane Curves
19. Evaluate $\int_Cx ds$, where $C$ is  
a. the straight-line segment $x = t, y = \dfrac{t}{2}$, from $(0, 0)$ to $(4, 2)$.   
b. the parabolic curve $x = t, y = t^2$ , from $(0, 0)$ to $(2, 4).$   
a. $\int_Cx ds$  
$=\int_0^42\sqrt{5}tdt=16\sqrt{5}$  
b. $\int_Cx ds$  
$=\int_0^22\sqrt{5}tdt=4\sqrt{5}$  
#### Masses and Moments
33. Mass of a wire Find the mass of a wire that lies along the curve  $\mathbf{r}(t) =(t^2-1)\mathbf{i} + 2t\mathbf{k},0\le t \le 1$ if the density is $\delta = \dfrac{3}{2}t.$   
    $M = \int_0^1\dfrac{3}{2}t\sqrt{4t^2 + 4}dt$  
    Let $t^2 + 1 = u, \dfrac{du}{dt} = 2t$  
    $M = \int_1^2\sqrt{u}\dfrac{3}{2}du$  
    $=[u^{\frac{3}{2}}]_1^2=2\sqrt{2}-1$
#### COMPUTER EXPLORATIONS
In Exercises 43–46, use a CAS to perform the following steps to   evaluate the line integrals.   
a. Find $ds = |\mathbf{v}(t)| dt$ for the path $\mathbf{r}(t) =g(t)\mathbf{i} + h(t)\mathbf{j} + k(t)\mathbf{k}$  
b. Express the integrand $f(g(t), h(t), k(t))|\mathbf{v}(t)|$ as a function of the parameter $t$.  
c. Evaluate $\int_Cf ds$ using Equation (2) in the text.

43. $f(x, y, z) = \sqrt{1 + 30x^2 + 10y},\mathbf{r}(t) =t\mathbf{i} + t^2(t)\mathbf{j} + 3t^2\mathbf{k},0\le t \le 2$   
    $|\mathbf{v}(t)|=\sqrt{1+40t^2}$  
    $\int_Cf ds = \int_0^21 + 40t^2dt=[t + \dfrac{40}{3}t^3]_0^2=\dfrac{6+320}{3}=\dfrac{326}{3}$
### 16.2 Vector Fields and Line Integrals: Work, Circulation, and Flux
#### Vector Fields
Find the gradient fields of the functions in Exercises 1–4.
1. $f(x, y, z) = (x^2 + y^2 + z^2)^{-\frac{1}{2}}$  
   $\nabla f =-\dfrac{x}{(x^2 + y^2 + z^2)^{\frac{3}{2}}}\mathbf{i}-\dfrac{y}{(x^2 + y^2 + z^2)^{\frac{3}{2}}}\mathbf{j}-\dfrac{z}{(x^2 + y^2 + z^2)^{\frac{3}{2}}}\mathbf{k}$
#### Line Integrals of Vector Fields
In Exercises 7–12, find the line integrals of $\mathbf{F}$ from $(0, 0, 0)$ to $(1, 1, 1)$ over each of the following paths in the accompanying figure.   
a. The straight-line path $C_1: \mathbf{r}(t) =t\mathbf{i} +t\mathbf{j}+ t\mathbf{k},0\le t \le 1$  
b. The curved path $C_1: \mathbf{r}(t) =t\mathbf{i} +t^2\mathbf{j}+ t^4\mathbf{k},0\le t \le 1$  
c. The path $C_3 \cup C_4$ consisting of the line segment from $(0, 0, 0)$ to $(1, 1, 0)$ followed by the segment from $(1, 1, 0)$ to $(1, 1, 1)$

7. $\mathbf{F}=3y\mathbf{i} +2x\mathbf{j}+ 4z\mathbf{k}$  
   a.$\int_0^1(3t\mathbf{i} +2t\mathbf{j}+ 4t\mathbf{k})(\mathbf{i} +\mathbf{j}+ \mathbf{k})dt$  
   $=\int_0^19tdt=\dfrac{9}{2}$   
   b. $\int_0^1(3t^2\mathbf{i} +2t\mathbf{j}+ 4t^4\mathbf{k})(\mathbf{i} +2t\mathbf{j}+ 4t^3\mathbf{k})dt$  
   $=\int_0^116t^7+7t^2dt=[2t^8+\dfrac{7}{3}t^3]_0^1=\dfrac{13}{3}$  
   c. $C_3:t\mathbf{i} +t\mathbf{j},0\le t \le 1,C_4:\mathbf{i} +\mathbf{j} + t\mathbf{k},0\le t \le 1$  
   $\int_0^1(3t\mathbf{i} +2t\mathbf{j})(\mathbf{i} +\mathbf{j})dt + \int_0^1(3\mathbf{i} +2\mathbf{j}+4t\mathbf{k})(\mathbf{k})dt$  
   $= \int_0^15tdt + \int_0^14tdt$  
   $= \dfrac{9}{2}$  
#### Line Integrals with Respect to $x, y$, and $z$
In Exercises 13–16, find the line integrals along the given path $C$.  

13. $\int_C (x - y) dx$, where $C: x = t, y = 2t + 1,$ for $0\le t \le 3$   
    $=\int_0^3(-t-1)dt=[-\dfrac{1}{2}t^2-t]_0^3=-\dfrac{15}{2}$  
#### Work
In Exercises 19–22, find the work done by $\mathbf{F}$ over the curve in the direction of increasing $t$.

19. $\mathbf{F} = xy\mathbf{i} +y\mathbf{j}-yz \mathbf{k},\mathbf{r}(t) =t\mathbf{i} +t^2\mathbf{j}+ t\mathbf{k}, 0 \le t\le 1$  
    $W = \int_0^1(t^3\mathbf{i} +t^2\mathbf{j}-t^3\mathbf{k})(\mathbf{i} +2t\mathbf{j}+ \mathbf{k})dt$  
    $=\int_0^3 2t^3dt=\dfrac{81}{2}$  
#### Line Integrals in the Plane
23. Evaluate $\int_Cxy dx + (x + y) dy$ along the curve $y = x^2$ from $(-1, 1)$ to $(2, 4)$.  
    $C: t\mathbf{i} +t^2\mathbf{j},-1\le t \le 2$  
    $dx = dt,dy=2tdt$  
    $\int_Cxy dx + (x + y) dy$  
    $=\int_{-1}^2(t^3+(t+t^2)2t)dt$  
    $= \int_{-1}^23t^3+2t^2dt$  
    $= \dfrac{3}{4}t^4+\dfrac{2}{3}t^3]_{-1}^2$  
    $= 12+\dfrac{16}{3}-\dfrac{3}{4}+\dfrac{2}{3}$  
    $=\dfrac{69}{4}$
#### Work, Circulation, and Flux in the Plane
27. Work Find the work done by the force $\mathbf{F} = xy\mathbf{i} +(y-x)\mathbf{j}$ over the straight line from $(1, 1)$ to $(2, 3)$.   
    $l: (1 + t)\mathbf{i} +(1 + 2t)\mathbf{j}, 0 \le t \le 1$  
    $W = \int_0^1((2t^2+3t + 1)\mathbf{i} +t\mathbf{j})(\mathbf{i} +2\mathbf{j})dt$  
    $= \int_0^12t^2+5t + 1dt= \dfrac{2}{3}+\dfrac{5}{2} + 1=\dfrac{25}{6}$  
#### Vector Fields in the Plane
47. Spin field Draw the spin field   
    $$
    \mathbf{F} = -\dfrac{y}{\sqrt{x^2 + y^2}}\mathbf{i} +\dfrac{x}{\sqrt{x^2 + y^2}}\mathbf{j}
    $$
    (see Figure 16.13) along with its horizontal and vertical components at a representative assortment of points on the circle $x^2 + y^2 = 4.$
#### Flow Integrals in Space
In Exercises 55–58, $\mathbf{F}$ is the velocity field of a fluid flowing through a region in space. Find the flow along the given curve in the direction of increasing $t$.

55. $\mathbf{F} = -4xy\mathbf{i} +8y\mathbf{j} + 2\mathbf{k}, \mathbf{r} = t\mathbf{i} +t^2\mathbf{j} + \mathbf{k},0 \le t \le 2$  
    $\int_0^2(-4t^3\mathbf{i} +8t^2\mathbf{j} + 2\mathbf{k})(\mathbf{i} +2t\mathbf{j})dt$  
    $=\int_0^2-4t^3+16t^3+2dt$  
    $=3t^4+2t]_0^2=52$
#### COMPUTER EXPLORATIONS
In Exercises 63–68, use a CAS to perform the following steps for finding the work done by force $\mathbf{F}$ over the given path:  
a. Find $d\mathbf{r}$ for the path $\mathbf{r}(t) = g(t)\mathbf{i} + h(t)\mathbf{j} + k(t)\mathbf{k}.$  
b. Evaluate the force $\mathbf{F}$ along the path.  
c. Evaluate $\int_C\mathbf{F}\cdot d\mathbf{r}.$    

63. $F = xy^6\mathbf{i} + 3x(xy^5+2)\mathbf{j}; \mathbf{r}(t) = 2\cos t\mathbf{i} + \sin t\mathbf{j},0 \le t \le 2\pi$   
    $d\mathbf{r}=-2\sin t\mathbf{i} + \cos t\mathbf{j}$  
    $F = 2\cos t \sin^6t\mathbf{i} + (2\cos t\sin^5t + 2)\mathbf{j}$  
    $\int_C\mathbf{F}\cdot d\mathbf{r}$  
    $= \int_0^{2\pi}-4\cos t \sin^8t + 2\cos^2t\sin^5t+2\cos tdt$  
### 16.3 Path Independence, Conservative Fields, and Potential Functions
#### Testing for Conservative Fields  
Which fields in Exercises 1–6 are conservative, and which are not?
1. $F = yz\mathbf{i} + xz\mathbf{j} + xy\mathbf{j}$  
   $\dfrac{\partial P}{\partial y} = x,\dfrac{\partial N}{\partial z} = x$,  
   $\dfrac{\partial M}{\partial z} =y, \dfrac{\partial P}{\partial x}=y$  
   $,\dfrac{\partial N}{\partial x} =z, \dfrac{\partial M}{\partial y} = z$  
   is conservative
#### Finding Potential Functions
In Exercises 7–12, find a potential function $f$ for the field $\mathbf{F}$.

7. $\mathbf{F} = 2x\mathbf{i} + 3y\mathbf{j} + 4z\mathbf{k}$   
   $f(x) =x^2+\dfrac{3}{2}y^2 + 2z^2$
#### Exact Differential Forms
In Exercises 13–17, show that the differential forms in the integrals are exact. Then evaluate the integrals.

13. $\int_{(2,3, -6)}^{(0,0,0)}2x dx + 2y dy + 2z dz$    
    $f = x^2 + y^2 + z^2$  
    $\int_{(2,3, -6)}^{(0,0,0)}2x dx + 2y dy + 2z dz$  
    $= f(2,3, -6)-f(0,0,0) = 49$
#### Finding Potential Functions to Evaluate Line Integrals
Although they are not defined on all of space $R^3$, the fields associated with Exercises 18–22 are conservative. Find a potential function for each field and evaluate the integrals as in Example 6.

18. $\int_{(1,\frac{\pi}{2},2)}^{(0,2,1)}2 \cos y dx + (\dfrac{1}{y}- 2x \sin y )dy +\dfrac{1}{z}dz$   
    $f = 2(\cos y)x+\ln y + \ln z$  
    $\int_{(1,\frac{\pi}{2},2)}^{(0,2,1)}2 \cos y dx + (\dfrac{1}{y}- 2x \sin y )dy +\dfrac{1}{z}dz$  
    $= \ln 2 + \ln 1-\ln\dfrac{\pi}{2}-\ln 2=-\ln\dfrac{\pi}{2}$
#### Applications and Examples
23. Revisiting Example 6 Evaluate the integral   
    $$
    \int_{(2,3, -1)}^{(1,1,1)}y dx + x dy + 4 dz
    $$
    from Example 6 by finding parametric equations for the line segment from $(1, 1, 1)$ to $(2, 3, -1)$ and evaluating the line integral of $\mathbf{F} = y\mathbf{i} + x\mathbf{j} + 4\mathbf{k}$ along the segment. Since $\mathbf{F}$ is conservative, the integral is independent of the path.  
    $l:(1 + t)\mathbf{i} + (1 + 2t)\mathbf{j} + (1-2t)\mathbf{k},0\le t\le 1$  
    $\int_0^1((1 + 2t)\mathbf{i} + (1 + t)\mathbf{j} + 4\mathbf{k})(1\mathbf{i} + 2\mathbf{j} -2\mathbf{k})dt$  
    $= \int_0^1-5+4tdt=-3$