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
