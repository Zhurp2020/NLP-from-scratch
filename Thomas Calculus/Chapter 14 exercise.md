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