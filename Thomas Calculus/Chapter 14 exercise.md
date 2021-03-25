# Thomas Calculus
## Chapter 14 Partial Derivatives
### 14.1 Functions of Several Variables
#### Domain, Range, and Level Curves
In Exercises 1–4, find the specific function values.
1. $f(x, y) = x^2 + xy^3$  
a. $f(0, 0)$ b. $f(-1, 1)$  
c. $f(2, 3)$ d. $f(-3, -2)$    
a. $0$ b. $0$  c. $58$ d. $33$
#### Matching Surfaces with Level Curves
Exercises 31–36 show level curves for six functions. The graphs of these functions are given on the next page (items a–f ), as are their equations (items g–l). Match each set of level curves with the appropriate graph and appropriate equation  
![](../images/Thomas%20Calculus/14-2.jpg)  
![](../images/Thomas%20Calculus/14-3.jpg)  
g. $z = -\dfrac{xy^2}{x^2 + y^2}$  
h. $z = y^2 - y^4 - x^2$  
i.$z = \cos x \cos y e^{-\frac{\sqrt{x^2 + y^2}}{4}}$  
j. $z = e^{-y}\cos x$  
k. $z = -\dfrac{1}{4x^2 + y^2}$   
l. $z = -\dfrac{xy(x^2 - y^2)}{x^2 + y^2}$  
31.   f,h
    ![](../images/Thomas%20Calculus/14-1.jpg)  
#### Functions of Two Variables  
Display the values of the functions in Exercises 37–48 in two ways: (a) by sketching the surface $z=f(x,y)$ and (b) by drawing an assortment of level curves in the function’s domain. Label each level curve with its function value.

37. $f(x,y)=y^2$   
#### Finding Level Curves
In Exercises 49–52, find an equation for and sketch the graph of the level curve of the function $f(x,y)$ that passes through the given point.

49. $f(x,y) = 16 - x^2 - y^2,(2\sqrt{2},\sqrt{2})$  
    $16 -x^2 - y^2 = 6$
#### Sketching Level Surfaces
In Exercises 53–60, sketch a typical level surface for the function.

53. $f(x,y,z)=x^2+y^2+z^2$
#### Finding Level Surfaces
In Exercises 61–64, find an equation for the level surface of the function through the given point.

61. $f(x, y, z) = \sqrt{x - y} - \ln z, (3, -1, 1)$  
    $\sqrt{x - y} - \ln z = 2$
#### COMPUTER EXPLORATIONS
Use a CAS to perform the following steps for each of the functions in Exercises 69–72.  
a. Plot the surface over the given rectangle.  
b. Plot several level curves in the rectangle.  
c. Plot the level curve of $f$ through the given point.  

69. $f(x,y) = x\sin\dfrac{y}{2} + y\sin 2x,0 \le x \le 5\pi, 0 \le y \le 5\pi, P(3\pi,\pi)$
### 14.2 Limits and Continuity in Higher Dimensions
#### Limits with Two Variables
Find the limits in Exercises 1–12
1. $\lim\limits_{(x,y)\to(0,0)}\dfrac{3x^2-y^2+5}{x^2 + y^2 + 2}$   
   $\lim\limits_{(x,y)\to(0,0)}\dfrac{3x^2-y^2+5}{x^2 + y^2 + 2} = \dfrac{5}{2}$
#### Limits of Quotients
Find the limits in Exercises 13–24 by rewriting the fractions first.

13. $\lim\limits_{(x,y)\to(1,1),x \ne y}\dfrac{x^2-2xy+y^2}{x - y}$  
    $\lim\limits_{(x,y)\to(1,1),x \ne y}\dfrac{x^2-2xy+y^2}{x - y}$  
    $=\lim\limits_{(x,y)\to(1,1),x \ne y}x + y = 2$
#### Limits with Three Variables
Find the limits in Exercises 25–30

25. $\lim\limits_{P\to(1,3,4)}(\dfrac{1}{x} + \dfrac{1}{y } + \dfrac{1}{z})$  
    $\lim\limits_{P\to(1,3,4)}(\dfrac{1}{x} + \dfrac{1}{y } + \dfrac{1}{z}) = \dfrac{19}{12}$
#### Continuity for Two Variables
At what points $(x, y)$ in the plane are the functions in Exercises 31–34 continuous?

31. a. $f(x, y) = \sin (x + y)$ b. $f(x, y) = \ln (x^2 + y^2)$  
    a. At all points  
    b. every point except $(0,0)$  
#### Continuity for Three Variables
At what points $(x, y, zdf  )$ in space are the functions in Exercises 35–40 continuous?

35. a. $f(x, y, z) = x^2 + y^2 - 2z^2$ b. $f(x, y, z) = \sqrt{x^2 + y^2 - 1}$  
    a. At all points,b. outside or on $x^2 + y^2 = 1, z\in R$
#### No Limit Exists at the Origin
By considering different paths of approach, show that the functions in Exercises 41–48 have no limit as $(x, y) \to (0, 0)$.

41. $f(x,y) = -\dfrac{x}{\sqrt{x^2 + y^2}}$  
    ![](../images/Thomas%20Calculus/14-4.jpg)  
    $y = kx, f(x,y) = -\dfrac{x}{\sqrt{x^2 + k^2 x^2}} = -\dfrac{1}{\sqrt{1 + k^2}}$  
    $\lim\limits_{(x,y) \to (0,0)} f(x,y) = -\dfrac{1}{1 + k^2}$
#### Theory and Examples
In Exercises 49–54, show that the limits do not exist.

49. $\lim\limits_{(x,y) \to (1,1)} \dfrac{xy^2 - 1}{y - 1}$    
    $y = kx^2, f(x,y) = \dfrac{xk^2x^4 -1}{kx^2 -1}$  
    $\lim\limits_{(x,y) \to (1,1)} \dfrac{xy^2 - 1}{y - 1} = \dfrac{k^2 -1}{k-1} = k + 1$
#### Changing Variables to Polar Coordinates
If you cannot make any headway with $\lim\limits_{(x,y) \to (0,0)} f(x,y)$ in rectangular coordinates, try changing to polar coordinates. Substitute $x = r \cos \theta, y = r \sin \theta$, and investigate the limit of the resulting expression as $r \to 0$. In other words, try to decide whether there exists a number $L$ satisfying the following criterion:  
Given $\varepsilon > 0$, there exists a $\delta > 0$ such that for all $r$ and $\theta$,  
$$
|r| < \delta \rArr |f(r,\theta) - L| < \varepsilon
$$
If such an $L$ exists, then
$$
\lim\limits_{(x,y) \to (0,0)} f(x,y) =\lim\limits_{r\to 0} f(r\cos\theta,r\sin\theta) = L
$$
In Exercises 65–70, find the limit of $f$ as $(x, y) \to (0, 0)$ or show that the limit does not exist.

65. $f(x,y) = \dfrac{x^3 - xy^2}{x^2 + y^2}$ 
    $\lim\limits_{(x,y) \to (0,0)} f(x,y)$  
    $= \lim\limits_{r\to 0} \dfrac{r^3\cos^3\theta-r^3\cos^2\theta\sin\theta}{r^2\cos^2\theta + r^2\sin^2\theta}$  
    $= 0$
#### Using the Limit Definition
Each of Exercises 73–78 gives a function $f(x, y)$ and a positive number $\varepsilon$. In each exercise, show that there exists a $\delta < 0$ such that for all $(x, y),$
$$
 \sqrt{x^2 + y^2} < \delta \rArr|f(x,y) - f(0,0) |<  \varepsilon
$$

73. $f(x,y) = x^2 + y^2, \varepsilon = 0.01$  
    $f(x,y) - f(0,0) =  x^2 + y^2 < 0.01$  
    $\delta = 0.1$
### 14.3 Partial Derivatives
#### Calculating First-Order Partial Derivatives
In Exercises 1–22, find $\dfrac{\partial f}{\partial x}$ and $\dfrac{\partial f}{\partial y}$.
1. $f(x, y) = 2x^2 - 3y - 4$  
   $\dfrac{\partial f}{\partial x} = 4x$  
   $\dfrac{\partial f}{\partial y} = -3$
#### Calculating Second-Order Partial Derivatives
Find all the second-order partial derivatives of the functions in Exercises 41–50.

41. $f(x, y) = x + y + xy$  
    $\dfrac{\partial f}{\partial x} = 1 +y$  
    $\dfrac{\partial f}{\partial y} = x + 1$  
    $f_{xx} = 0, f_{yy} = 0,f_{xy} = 1$
#### Mixed Partial Derivatives
In Exercises 55–60, verify that $w_{xy} = w_{yx}$ .

55. $w = \ln (2x + 3y)$  
    $\dfrac{\partial w}{\partial x} = \dfrac{2}{2x + 3y}$  
    $\dfrac{\partial w}{\partial y} = \dfrac{3}{2x + 3y}$  
    $w_{xy} = -\dfrac{6}{(2x + 3y)^2} = w_{yx}$
#### Using the Partial Derivative Definition
In Exercises 63–66, use the limit definition of partial derivative to compute the partial derivatives of the functions at the specified points.

63. $f(x, y) = 1 - x + y - 3x^2y,\dfrac{\partial f}{\partial x}$ and $\dfrac{\partial f}{\partial y}$ at $(1,2)$  
    $\dfrac{\partial f}{\partial x} = \lim\limits_{h\to0}\dfrac{(1-x-h+y-3(x+h)^2y)-(1 - x + y - 3x^2y)}{h}$   
    $= \lim\limits_{h\to0}\dfrac{(2-h-6(1+h)^2) + 4}{h}$  
    $=\lim\limits_{h\to0}\dfrac{-6h^2-13h}{h} = -13$  
    $\dfrac{\partial f}{\partial y} = \lim\limits_{h\to0}\dfrac{(1-x+y +h-3x^2(y + h))+4}{h}$   
    $= \lim\limits_{h\to0}\dfrac{(2+h-3(2+h)) + 4}{h}$  
    $=\lim\limits_{h\to0}\dfrac{-2h}{h} = -2$
#### Differentiating Implicitly
75. Find the value of $\dfrac{\partial z}{\partial x}$ at the point $(1, 1, 1)$ if the equation  
    $$
    xy + z^3x - 2yz = 0
    $$
    defines $z$ as a function of the two independent variables $x$ and $y$ and the partial derivative exists.  
    $\dfrac{\partial}{\partial x}xy + z^3x - 2yz = 0$  
    $y + \dfrac{\partial z^3}{\partial x}x + z^3 - 2y\dfrac{\partial z}{\partial x} = 0$  
    $y + 3z^2x\dfrac{\partial z}{\partial x} + z^3 - 2y\dfrac{\partial z}{\partial x} = 0$  
    $\dfrac{\partial z}{\partial x} = \dfrac{-z^3 - y}{3z^2x -2y}$  
    $= -2$
#### Theory and Examples
81. Let $f(x,y) = \begin{cases}y^3&\quad y \ge 0 \\-y^2&\quad y < 0 \end{cases}$  
    Find $f_x, f_y, f_{xy} ,$ and $f_{yx}$ , and state the domain for each partial derivative.  
    $f_x = 0$  
    $f_y =  \begin{cases}3y^2&\quad y \ge 0 \\-2y&\quad y < 0 \end{cases}$  
    $f_{xy} = f_{yx} = 0$
### 14.4 The Chain Rule
#### Chain Rule: One Independent Variable
In Exercises 1–6, (a) express $\dfrac{\partial w}{\partial t}$ as a function of $t$, both by using the Chain Rule and by expressing w in terms of $t$ and differentiating directly with respect to $t$. Then (b) evaluate $\dfrac{\partial w}{\partial t}$ at the given value of $t$.
1. $w = x^2 + y^2, x = \cos t, y = \sin t; t = \pi$  
   $\dfrac{\partial w}{\partial t} =-2x\sin t + 2y\cos t =0$  
   $w = 1, \dfrac{\partial w}{\partial t} = 0$
#### Chain Rule: Two and Three Independent Variables
In Exercises 7 and 8, (a) express $\dfrac{\partial z}{\partial u}$ and $\dfrac{\partial z}{\partial v}$ as functions of $u$ and $v$ both by using the Chain Rule and by expressing $z$ directly in terms of $u$ and $z$ before differentiating. Then (b) evaluate $\dfrac{\partial z}{\partial u}$ and $\dfrac{\partial z}{\partial v}$ at the given point $(u, v)$.  

7. $z = 4e^x\ln y,x = \ln(u\cos v), y = u\sin v,(u,v) = (2,\dfrac{\pi}{4})$  
   $\dfrac{\partial z}{\partial u} = 4e^x\ln y\dfrac{1}{u} + \dfrac{4e^x}{y}\sin v$  
   $= \dfrac{4e^{\ln(u\cos v)}\ln (u\sin v)}{u} + \dfrac{4e^{\ln(u\cos v)}\sin v}{u\sin v}$  
   $= 4\cos v\ln(u\sin v) + 4\cos v$  
   $z = 4u\cos v\ln(u\sin v),\dfrac{\partial z}{\partial u}=4\cos vu\dfrac{1}{u} + 4\cos v\ln(u\sin v) = 4\cos v\ln(u\sin v) + 4\cos v$  
   $\dfrac{\partial z}{\partial u}|_{(u,v) = (2,\frac{\pi}{4})} =2\sqrt{2}\ln\sqrt{2} + 2\sqrt{2}$  
   $\dfrac{\partial z}{\partial v} = 4e^x\ln y\dfrac{-\sin v}{\cos v} + \dfrac{4e^x}{y}u\cos v$  
   $= \dfrac{-4u\cos v\sin v\ln (u\sin v)}{\cos v} + \dfrac{4u^2\cos^2 v}{u\sin v}$  
   $= -4u\sin v\ln(u\sin v) + 4u\cos v\cot v$  
   $z = 4u\cos v\ln(u\sin v),\dfrac{\partial z}{\partial v}=4u(\cos v\dfrac{\cos v}{\sin v} -\sin v\ln(u\sin v)) =-4u\sin v\ln(u\sin v) + 4u\cos v\cot v$  
   $\dfrac{\partial z}{\partial u}|_{(u,v) = (2,\frac{\pi}{4})} =-4\sqrt{2}\ln\sqrt{2} + 4\sqrt{2}$ 
#### Using a Dependency Diagram
In Exercises 13–24, draw a dependency diagram and write a Chain Rule formula for each derivative.

13. $\dfrac{\partial z}{\partial t}$ for $z = f(x, y), x = g(t), y = h(t)$  
    $\dfrac{\partial z}{\partial t} = \dfrac{\partial z}{\partial x}\dfrac{\partial x}{\partial t} + \dfrac{\partial z}{\partial y}\dfrac{\partial y}{\partial t}$
#### Implicit Differentiation
Assuming that the equations in Exercises 25–30 define $y$ as a differentiable function of $x$, use Theorem 8 to find the value of $\dfrac{dy}{dx}$ at the given point.

25.  $x^3 - 2y^2 + xy = 0, (1, 1)$   
     $\dfrac{dy}{dx} = -\dfrac{3x^2+y}{-4y+x}$  
     $\dfrac{dy}{dx}|_{(1,1)} = \dfrac{4}{3}$
#### Finding Partial Derivatives at Specified Points
35. Find $\dfrac{\partial w}{\partial r}$ when $r = 1, s = -1$ if $w = (x + y + z)^2,x = r - s, y = \cos (r + s), z = \sin (r + s).$   
    $w = x^2+y^2+z^2 + 2xy + 2xz + 2yz$  
    $\dfrac{\partial w}{\partial r}= (2x + 2y + 2z) - (2x + 2y + 2z)\sin(r + s)+  (2x + 2y + 2z)\cos(r + s)$  
    $=(2r -2s + 2\cos(r +s) + 2\sin(r+ s))(1-\sin (r + s) + \cos(r + s))$  
    $\dfrac{\partial w}{\partial r}|_{(1,1)} = (4+2)(1+1) = 12$  
#### Theory and Examples
41. Assume that $w = f(s^3 + t^2)$ and $f'(x) = e^x$. Find $\dfrac{\partial w}{\partial t}$ and $\dfrac{\partial w}{\partial s}$  
    $w = e^{s^3 + t^2} + C$  
    $\dfrac{\partial w}{\partial t}= 2te^{s^3 + t^2}$  
    $\dfrac{\partial w}{\partial s}= 3s^2e^{s^3 + t^2}$
### 14.5 Directional Derivatives and Gradient Vectors
#### Calculating Gradients
In Exercises 1–6, find the gradient of the function at the given point. Then sketch the gradient together with the level curve that passes through the point.
1. $f(x, y) = y - x, (2, 1)$  
   $\nabla f = \dfrac{\partial f}{\partial x}\mathbf{i} + \dfrac{\partial f}{\partial y}\mathbf{j}$  
   $=-\mathbf{i} + {j}$
#### Finding Directional Derivatives
In Exercises 11–18, find the derivative of the function at $P_0$ in the direction of $\mathbf{u}$.

11. $f(x, y) = 2xy - 3y^2, P_0(5, 5), \mathbf{u} = 4\mathbf{i} + 3{j}$  
    $\nabla f = 2y\mathbf{i} + (2x-6y)\mathbf{j} =10\mathbf{i}-20\mathbf{j}$  
    $D_uf = -20$
#### Tangent Lines to Level Curves
In Exercises 25–28, sketch the curve $f(x, y) = c$ together with $\nabla f$ and the tangent line at the given point. Then write an equation for the tangent line.

25. $x^2 + y^2 = 4,(\sqrt{2},\sqrt{2})$   
    $\nabla f =2y\mathbf{i} + 2z\mathbf{j} =2\sqrt{2}\mathbf{i}-2\sqrt{2}\mathbf{j}$  
    $f_x = f_y = 2\sqrt{2}$  
    $2\sqrt{2}(x-\sqrt{2})+2\sqrt{2}(y-\sqrt{2}) = 0$  
    $2\sqrt{2}x-2\sqrt{2}y = 0, x = y$  
#### Theory and Examples
29. Let $f(x, y) = x^2 - xy + y^2 - y$. Find the directions $\mathbf{u}$ and the values of $D_{\mathbf{u}} f(1, -1)$ for which  
    a. $D_{\mathbf{u}} f(1, -1)$ is largest b. $D_{\mathbf{u}} f(1, -1)$ is smallest    
    c. $D_{\mathbf{u}} f(1, -1) = 0$ d. $D_{\mathbf{u}} f(1, -1) =4$  
    e. $D_{\mathbf{u}} f(1, -1) = -3$  
    $\nabla f = (2x-y)\mathbf{i} + (2y-x-1)\mathbf{j}=3\mathbf{i}-4\mathbf{j}$  
    a. $\mathbf{u} = \dfrac{3}{5}\mathbf{i}-\dfrac{4}{5}\mathbf{j},D_{\mathbf{u}} f(1, -1) =5$  
    b.  $\mathbf{u} = -\dfrac{3}{5}\mathbf{i}+\dfrac{4}{5}\mathbf{j},D_{\mathbf{u}} f(1, -1) =-5$  
    c. $\mathbf{u} = \dfrac{4}{5}\mathbf{i}+\dfrac{3}{5}\mathbf{j},$ or $\mathbf{u} = -\dfrac{4}{5}\mathbf{i}-\dfrac{3}{5}\mathbf{j},D_{\mathbf{u}} f(1, -1) =0$   
    d. $3t-4(\sqrt{1-t^2}) = 4$  
    $9t^2-24t + 16 = 16-16t^2$  
    $25t^2-24t = 0,t = 0$ or $t = \dfrac{24}{25}$  
    $\mathbf{u} = \dfrac{24}{25}\mathbf{i}+\dfrac{7}{25}\mathbf{j},\mathbf{u} = \mathbf{j}$  
    e.$3t-4(\sqrt{1-t^2}) = -3$  
    $9t^2+18t + 9 = 16-16t^2$  
    $25t^2 + 18t-7 = 0$  
    $(t-1)(25t-7) = 0, t = 1, t = \dfrac{7}{25}$  
    $\mathbf{u} = \dfrac{7}{25}\mathbf{i}+\dfrac{24}{25}\mathbf{j},\mathbf{u} = \mathbf{i}$
### 14.6 Tangent Planes and Differentials
#### Tangent Planes and Normal Lines to Surfaces
In Exercises 1–10, find equations for the  
(a) tangent plane and   
(b) normal line at the point $P_0$ on the given surface.
1. $x^2 + y^2 + z^2 = 3, P_0(1, 1, 1)$  
   a. $2(x-1) + 2(y-1) +2(z-1) = 0$  
   b. $x = 1+2t, y=1+2t,z=1+2t$
#### Tangent Lines to Intersecting Surfaces
In Exercises 15–20, find parametric equations for the line tangent to the curve of intersection of the surfaces at the given point.

15. Surfaces: $x + y^2 + 2z = 4, x = 1$  
    Point: $(1, 1, 1)$  
    $y^2 + 2z = 3$  
    $x = 1,y=1 + 2t,z = 1+ 2t$ 
#### Estimating Change
21. By about how much will  
    $$
    f(x, y, z) = \ln\sqrt{x^2 + y^2 + z^2}
    $$
    change if the point $P(x, y, z)$ moves from $P_0(3, 4, 12)$a distance of $ds = 0.1$ unit in the direction of $3\mathbf{i}+6\mathbf{j}-2\mathbf{k}$?  
    $\nabla f=\dfrac{\frac{x}{\sqrt{x^2 + y^2 + z^2}}}{\sqrt{x^2 + y^2 + z^2}}\mathbf{i}+\dfrac{\frac{y}{\sqrt{x^2 + y^2 + z^2}}}{\sqrt{x^2 + y^2 + z^2}}\mathbf{j} + \dfrac{\frac{z}{\sqrt{x^2 + y^2 + z^2}}}{\sqrt{x^2 + y^2 + z^2}}\mathbf{k}$  
    $=\dfrac{x}{x^2 + y^2 + z^2}\mathbf{i}+\dfrac{y}{x^2 + y^2 + z^2}\mathbf{j} + \dfrac{z}{x^2 + y^2 + z^2}\mathbf{k}$  
    $df = (\nabla f|_{P_0}\cdot \mathbf{u})ds$  
    $=(\dfrac{3}{169}\mathbf{i}+\dfrac{4}{169}\mathbf{j} + \dfrac{144}{169}\mathbf{k})(3\mathbf{i}+6\mathbf{j}-2\mathbf{k})ds$  
    $= \dfrac{9+24-288}{169}ds$   
    $= -\dfrac{255}{1690} = -\dfrac{51}{338}$  
#### Finding Linearizations
In Exercises 27–32, find the linearization $L(x, y)$ of the function at each point.

27. $f(x, y) = x^2 + y^2 + 1$ at a. $(0, 0)$, b. $(1, 1)$   
    a.$L(x,y) =1$  
    b. $L(x,y) = 3 + 2(x-1) + 2(y-1)$  
#### Bounding the Error in Linear Approximations
In Exercises 35–40, find the linearization $L(x, y)$ of the function $f(x, y)$ at $P_0$. Then find an upper bound for the magnitude $E$ of the error in the approximation $f(x, y) ≈ L(x, y)$ over the rectangle $R$.

35. $f(x, y) = x^2 - 3xy + 5$ at $P_0(2, 1),R: | x - 2| \le 0.1, | y - 1 |\le0.1$    
    $f_{x} = 2x-3y,f_{xx} = 2,f_{yy} =0, f_{xy} =-3M = 2$  
    $E(x,y) \le \dfrac{1}{2}M(| x - 2|^2 + | y - 1 |^2)$  
    $\le 0.02$  
#### Linearizations for Three Variables
Find the linearizations $L(x, y, z)$ of the functions in Exercises 41–46 at the given points.

41. $f(x, y, z) = xy + yz + xz$ at  
a. $(1, 1, 1)$ b. $(1, 0, 0)$ c. $(0, 0, 0)$  
    a. $L(x,y,z) = 3 + 2(x-1) + 2(y-1) + 2(z-1)$  
    b. $L(x,y,z) = 1 + 2(x-1)$  
    c. $L(x,y,z) = 0$
#### Estimating Error; Sensitivity to Change
51. Estimating maximum error Suppose that $T$ is to be found from the formula $T = x(e^y + e^{-y})$, where $x$ and $y$ are found to be $2$ and $\ln 2$ with maximum possible errors of $| dx | = 0.1$ and $| dy | =0.02$. Estimate the maximum possible error in the computed value of $T$.  
    $T_x =(e^y + e^{-y}), T_{xx} = 0,T_{xy} = e^y -\dfrac{1}{e^{2y}}, T_y =x(e^y -\dfrac{1}{e^{2y}}), T_{yy} = x(e^y -\dfrac{2}{e^{3y}}), M =4$  
    $E(x,y) \le \dfrac{1}{2}M(dx^2 + dy^2) \le 0.0208$  
#### Theory and Examples
57. the linearization of $f(x, y)$ is a tangent-plane approximation. Show that the tangent plane at the point $P_0(x_0, y_0, f(x_0, y_0))$ on the surface $z = f(x, y)$ defined by a differentiable function $f$ is the plane  
    $$
    f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0)-(z-f(x_0, y_0)) = 0 
    $$
    or 
    $$
    z = f(x_0, y_0) + f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0)
    $$
     Thus, the tangent plane at $P_0$ is the graph of the linearization of $f$ at $P_0$ (see accompanying figure)
     ![](../images/Thomas%20Calculus/14-5.jpg)  
     $f_x(P_0)(x - x_0) + f_y(P_0)(y - y_0) + f_z(P_0)(z - z_0) = 0$
### 14.7 Extreme Values and Saddle Points
#### Finding Local Extrema
Find all the local maxima, local minima, and saddle points of the functions in Exercises 1–30.
1. $ƒ(x, y) = x^2 + xy + y^2 + 3x - 3y + 4$  
   $f_x = 2x +y + 3,f_y = 2y + x -3$  
   $f_{xx} = 2,f_{yy} = 2, f_{xy} = 1$  
   $f_x = f_y = 0$  
   $\begin{cases}2x + y = -3 \\x + 2y = 3\end{cases}$  
   $\begin{cases}x  = -3 \\y = 3\end{cases}$   
   Critical point $(-3,3)$  
   $f_{xx}f_{yy} - f_{xy}^2 = 3>0,$ local maximum
#### Finding Absolute Extrema
In Exercises 31–38, find the absolute maxima and minima of the functions on the given domains.

31. $f(x, y) = 2x^2 - 4x + y^2 - 4y + 1$ on the closed triangular plate bounded by the lines $x = 0, y = 2, y = 2x$ in the first quadrant    
    boundary points $(0,0),(0,2),(1,2)$  
    $f(0,0) = 1,f(0,2) = -3,f(1,2) = -5$  
    $f_x =2x-4,f_y = 2y-4$  
    $f_x = f_y = 0,x =2,y=2$  
    maximum $(0,0,1)$,minimum $(1,2,-5)$  
#### Theory and Examples
43. Find the maxima, minima, and saddle points of $f(x, y)$, if any, given that  
a. $f_x = 2x - 4y$ and $f_y = 2y - 4x$   
b. $f_x = 2x - 2$ and $f_y = 2y - 4$  
c. $f_x = 9x^2 - 9$ and $f_y = 2y + 4$  
Describe your reasoning in each case  
a. $f_{xx} = 2,f_{yy} = 2, f_{xy} = -4$  
$f_x = f_y = 0,x = 0,y=0$  
$f_{xx}f_{yy} - f_{xy}^2=-12>0$  
saddle point at $(0,0)$  
b. $f_{xx} = 2,f_{yy} = 2, f_{xy} = 0$  
$f_x = f_y = 0,x = 1,y=2$  
$f_{xx}f_{yy} - f_{xy}^2=4>0$  
local minimum at $(1,2)$    
c. $f_{xx} = 18x,f_{yy} = 2, f_{xy} = 0$  
$f_x = f_y = 0,x = 1,y=-2$ or $x = 0,y=-2$  
at $(1,-2),f_{xx}f_{yy} - f_{xy}^2=36>0$   
at $(0,-2),f_{xx}f_{yy} - f_{xy}^2=0$  
local minimum $(1,-2)$  
#### COMPUTER EXPLORATIONS
In Exercises 71–76, you will explore functions to identify their local extrema. Use a CAS to perform the following steps:  
a. Plot the function over the given rectangle.  
b. Plot some level curves in the rectangle.  
c. Calculate the function’s first partial derivatives and use the CAS equation solver to find the critical points. How do the critical points relate to the level curves plotted in part (b)?  Which critical points, if any, appear to give a saddle point?Give reasons for your answer.  
d. Calculate the function’s second partial derivatives and find the discriminant $f_{xx}f_{yy} - f_{xy}^2$  
e. Using the max-min tests, classify the critical points found in part (c). Are your findings consistent with your discussion in part (c)?

71. $f(x, y) = x^2 + y^3 - 3xy, -5 \le x \le 5, -5 \le y \le 5$  
    $f_x = 2x-3y,f_y=3y^2-3x$  
    $f_x = f_y = 0$  
    $3y^2-\dfrac{9}{2}y = 0,y_1 = 0,y_2 = \dfrac{3}{2}$  
    Critical point $(0,0),(\dfrac{9}{4},\dfrac{3}{2})$  
    $f_{xx} = 2,f_{yy} = 6y, f_{xy} = -3$   
    $f_{xx}f_{yy} - f_{xy}^2 = -9<0$  
    $f_{xx}f_{yy} - f_{xy}^2 = 9>0$  
    Saddle point $(0,0)$    
### 14.8 Lagrange Multipliers
#### Two Independent Variables with One Constraint
1. Extrema on an ellipse. Find the points on the ellipse $x^2 + 2y^2 = 1$ where $f(x, y) = xy$ has its extreme values.   
   $f(x,y) = xy, g(x,y) = x^2 + 2y^2 - 1$  
   $\nabla f = y\mathbf{i},\nabla g = 2x\mathbf{i} +4y\mathbf{j}$  
   $\nabla f = \lambda \nabla y$  
   $\begin{cases}2x\lambda = y \\4y\lambda = 0\\ x^2 + 2y^2 - 1 = 0\end{cases}$   
   $\begin{cases}\lambda = 0 \\x = \pm 1\\y = 0\end{cases}$   
#### Three Independent Variables with One Constraint
17. Minimum distance to a point Find the point on the plane $x + 2y + 3z = 13$ closest to the point $(1, 1, 1)$   
    $f(x,y,z) = \sqrt{(x-1)^2 + (y-1)^2 +(z-1)^2},g(x,y,z) = x + 2y + 3z - 13$  
    $\nabla f = \dfrac{x + 1}{\sqrt{(x-1)^2 + (y-1)^2 +(z-1)^2}}\mathbf{i} + \dfrac{y + 1}{\sqrt{(x-1)^2 + (y-1)^2 +(z-1)^2}}\mathbf{j} + \dfrac{z + 1}{\sqrt{(x-1)^2 + (y-1)^2 +(z-1)^2}}\mathbf{k},$  
    $\nabla g = \mathbf{i} + 2\mathbf{j} + 3\mathbf{k}$   
    $\begin{cases}\lambda = \dfrac{x + 1}{\sqrt{(x-1)^2 + (y-1)^2 +(z-1)^2}} \\2\lambda =\dfrac{y + 1}{\sqrt{(x-1)^2 + (y-1)^2 +(z-1)^2}}\\3\lambda = \dfrac{z + 1}{\sqrt{(x-1)^2 + (y-1)^2 +(z-1)^2}} \\ x + 2y + 3z - 13 = 0\end{cases}$   
    $\begin{cases}2x -y=-1 \\3x -z = -2 \\ x + 2y + 3z - 13 = 0\end{cases}$   
    $x + 4x + 2 + 9x + 6 -13 = 0, x = -\dfrac{5}{14}$  
    $\begin{cases} x = -\dfrac{5}{14} \\y = \dfrac{2}{7} \\ z = \dfrac{13}{14}\end{cases}$  
#### Extreme Values Subject to Two Constraints
37. Maximize the function $f(x, y, z) = x^2 + 2y - z^2$ subject to the constraints $2x - y = 0$ and $y + z = 0.$   
    $f(x,y,z) =  x^2 + 2y - z^2,g_1(x,y,z) =  2x -y, g_2(x,y) = y + z$  
    $\nabla f = 2x\mathbf{i} + 2\mathbf{j} -2z\mathbf{k},\nabla g_1 = 2\mathbf{i} -\mathbf{j},\nabla g_2 = \mathbf{j} + \mathbf{k}$  
    $\begin{cases}2\lambda = 2x \\-\lambda + u =2 \\ u = -2z \\2x - y = 0\\ y + z = 0.\end{cases}$   
    $\begin{cases}-x -2z = 2 \\2x - y = 0\\ y + z = 0.\end{cases}$  
    $\begin{cases}x = \dfrac{2}{3} \\y = \dfrac{4}{3}\\ z = -\dfrac{4}{3}.\end{cases}$   
    $f(x)_{\max} = \dfrac{3}{9}+\dfrac{8}{3}-\dfrac{16}{9} =\dfrac{11}{9}$
#### Theory and Examples
45. the condition $\nabla f = \lambda \nabla g$ is not sufficient Although $\nabla f = \lambda \nabla g$ is a necessary condition for the occurrence of an extreme value of $f(x, y)$ subject to the conditions $g(x, y) = 0$ and $\nabla g \ne 0,$ it does not in itself guarantee that one exists. As a case in point, try using the method of Lagrange multipliers to find a maximum value of $f(x, y) = x + y$ subject to the constraint that $xy = 16$. The method will identify the two points $(4, 4)$ and $(-4, -4)$ as candidates for the location of extreme values. Yet the sum $x + y$ has no maximum value on the hyperbola $xy = 16$. The farther you go from the origin on this hyperbola in the first quadrant, the larger the sum $f(x, y) = x + y$ becomes.
#### COMPUTER EXPLORATIONS
In Exercises 49–54, use a CAS to perform the following steps implementing the method of Lagrange multipliers for finding constrained extrema:   
a. Form the function $h = f - \lambda_1g_1 - \lambda_2g_2$, where $f$ is the
function to optimize subject to the constraints $g_1 = 0$ and $g_2 = 0$.   
b. Determine all the first partial derivatives of $h,$ including the partials with respect to $\lambda_1$ and $\lambda_2$, and set them equal to $0$.   
c. Solve the system of equations found in part (b) for all the unknowns, including $\lambda_1$ and $\lambda_2$.  
d. Evaluate $f$ at each of the solution points found in part (c) and select the extreme value subject to the constraints asked for in the exercise.  

49. Minimize $f(x, y, z) = xy + yz$ subject to the constraints $x^2 + y^2 - 2 = 0$ and $x^2 + z^2 - 2 = 0.$   
    $h = xy + yz-\lambda_1(x^2 + y^2 - 2) - \lambda_2(x^2 + z^2 - 2)$  
    $h_x =(-2\lambda_1 - 2\lambda_2)x +y$  
    $h_y =-2\lambda_1y +x + z$  
    $h_z = -2\lambda_2z + y$  
    $h_{\lambda_1} = -(x^2 + y^2 - 2)$  
    $h_{\lambda_2} = -(x^2 + z^2 - 2)$  
    $\begin{cases}(-2\lambda_1 - 2\lambda_2)x +y = 0  \\-2\lambda_1y +x + z = 0\\  -2\lambda_2z + y = 0 \\-(x^2 + y^2 - 2) = 0 \\ -(x^2 + z^2 - 2) = 0\end{cases}$  
    if $y = z$  
    $\begin{cases}(-2\lambda_1 - 2\lambda_2)x +y = 0  \\ x + (1-2\lambda_1) y= 0\\  (1-2\lambda_2) y = 0 \\ x^2 +y^2 = 2\end{cases}$  
    $\lambda_2 =\dfrac{1}{2}$   
    $\begin{cases}(-2\lambda_1 - 1)x +y = 0  \\ x + (1-2\lambda_1) y= 0 \\ x^2 +y^2 = 2\end{cases}$   
    $\begin{cases} x^2 + (4\lambda_1^2 + 4\lambda_1 +1)x^2 = 2\\ x^2 + \dfrac{x^2}{4\lambda_1^2 - 4\lambda_1 +1}= 2 \end{cases}$  
    No solution 
    $y = -z$      
    $\begin{cases}(-2\lambda_1 - 2\lambda_2)x +y = 0  \\ x - (1+2\lambda_1) y= 0\\  (1+2\lambda_2) y = 0 \\ x^2 +y^2 = 2\end{cases}$   
    $\lambda_2 = -\dfrac{1}{2}$   
    $\begin{cases}(-2\lambda_1 - 1)x +y = 0  \\ x - (1+2\lambda_1) y= 0 \\ x^2 +y^2 = 2\end{cases}$  
    $\begin{cases}x = \sqrt{2}\\y = -\sqrt{2}\\  z= \sqrt{2} \\ \lambda_1 = -1\\ \lambda_2 = -\dfrac{1}{2}\end{cases}$  or $\begin{cases}x = -\sqrt{2}\\y = \sqrt{2}\\  z =-\sqrt{2} \\ \lambda_1 = -1\\ \lambda_2 = -\dfrac{1}{2}\end{cases}$  
    $f(x)_{\min} = -4$