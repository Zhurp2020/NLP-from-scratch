# Thomas Calculus
## Chapter 15 Multiple Integrals
### 15.1  Double and Iterated Integrals over Rectangles 
#### Evaluating Iterated Integrals
In Exercises 1–14, evaluate the iterated integral.
1. $\int_1^2\int_0^42xydydx$  
    $\int_1^2\int_0^42xydydx$  
    $=\int_1^2[xy^2]_{y=0}^{y=4}dx$  
    $=\int_1^2[16x]dx$  
    $=8x^2]_1^2 = 24$
#### Evaluating Double Integrals over Rectangles
In Exercises 17–24, evaluate the double integral over the given region $R$.

17. $\iint(6y^2 - 2x) dA, R: 0 \le x \le 1, 0 \le y \le 2$  
    $\iint(6y^2 - 2x) dA$  
    $=\int_0^1\int_0^2(6y^2 - 2x) dydx$  
    $=\int_0^1[2y^3-2xy]_{y=0}^{y=2}dx$   
    $= \int_0^1[16-4x]dx$  
    $= 16x-2x^2]_0^1 = 14$  
### 15.2 Double Integrals over General Regions
#### Sketching Regions of Integration
In Exercises 1–8, sketch the described regions of integration.
1. $0 \le x \le 3, 0 \le y \le 2x$
#### Finding Limits of Integration
In Exercises 9–18, write an iterated integral for $\iint\limits_RdA$ over the described region $R$ using (a) vertical cross-sections, (b) horizontal cross-sections.  

9. ![](../images/Thomas%20Calculus/15-1.jpg)  
    $\iint\limits_RdA = \int_0^2\int_{x^3}^8dydx$  
    $= \int_0^8\int_0^{\sqrt[3]{y}}dxdy$  
#### Finding Regions of Integration and Double Integrals
In Exercises 19–24, sketch the region of integration and evaluate the integral

19. $\int_0^{\pi}\int_0^xx\sin ydydx$  
    $= \int_0^{\pi}[-x\cos y]_{y=0}^{y=x}dx$  
    $=\int_0^{\pi}[-x\cos x + x]dx$  
    $=\int_0^{\pi}xdx - \int_0^{\pi}[x\cos x]dx$   
    Let $u(x) = x,v'(x) = \cos x$  
    $u'(x) = 1,v(x) = \sin x$  
    $\int[x\cos x]dx$  
    $= x -\int\sin xdx = x + \cos x$  
    $\int_0^{\pi}[x\cos x]dx =\pi - 2$  
    $\int_0^{\pi}\int_0^xx\sin ydydx$  
    $= \dfrac{1}{2}x^2]_0^{\pi} - \pi + 2$  
    $= \dfrac{1}{2}\pi^2-\pi + 2$
#### Reversing the Order of Integration
In Exercises 33–46, sketch the region of integration and write an  equivalent double integral with the order of integration reversed.

33. $\int_0^1\int_2^{4-2x}xdydx$  
    $= \int_2^4\int_0^{2-\frac{1}{2}y}ydxdy$  
#### Volume Beneath a Surface $z = f(x, y)$
57. Find the volume of the region bounded above by the paraboloid $z = x^2 + y^2$ and below by the triangle enclosed by the lines $y = x, x = 0$, and $x + y = 2$ in the $xy$-plane.  
    $V = \int_0^1\int_y^{2-y}x^2 + y^2dxdy$  
    $= \int_0^1[\dfrac{1}{3}x^3+y^2x]_{x=y}^{x=2-y}dy$   
    $= \int_0^1[\dfrac{1}{3}(2-y)^3+y^2(2-y) - \dfrac{1}{3}y^3-y^3]_dy$  
    $\dfrac{1}{3}(2-y)^3+y^2(2-y) - \dfrac{1}{3}y^3-y^3$  
    $= \dfrac{1}{3}(4-4y+y^2)(2-y) + y^2(2-y)-\dfrac{4}{3}y^3$  
    $= (2-y)(\dfrac{4}{3}y^2-\dfrac{4}{3}y+\dfrac{4}{3})-\dfrac{4}{3}y^3$  
    $=4y^2-4y+\dfrac{8}{3}$  
    $V = \dfrac{4}{3}y^3-2y^2+\dfrac{8}{3}y]_0^1$  
    $= 2$
#### Integrals over Unbounded Regions
Improper double integrals can often be computed similarly to improper integrals of one variable. The first iteration of the following improper integrals is conducted just as if they were proper integrals. One then evaluates an improper integral of a single variable by taking  appropriate limits, as in Section 8.8. Evaluate the improper integrals  in Exercises 69–72 as iterated integrals.

69. $\int_1^{\infty}\int_{e^{-x}}^1\dfrac{1}{x^3y}dydx$  
    $=\int_1^{\infty}[\dfrac{1}{x^3}\ln y]_{y=e^{-x}}^{y=1}dx$   
    $=\int_1^{\infty}[\dfrac{1}{x^2}]dx$   
    $=\lim\limits_{a\to \infty}(-\dfrac{1}{a} + 1) = 1$  
#### Approximating Integrals with Finite Sums
In Exercises 73 and 74, approximate the double integral of $f(x, y)$ over the region $R$ partitioned by the given vertical lines $x = a$ and horizontal lines $y = c$. In each subrectangle, use $(x_k, y_k)$ as indicated for your approximation.
$$
\iint\limits_Rf(x,y)dA \approx\sum_{k=1}^nf(x_k,y_k)\Delta A_k
$$
73. $f(x, y) = x + y$ over the region $R$ bounded above by the semicircle $y = \sqrt{1 - x^2}$ and below by the $x$-axis, using the partition $x = -1, -\dfrac{1}{2}, 0, \dfrac{1}{4}, \dfrac{1}{2}, 1$ and $y = 0, \dfrac{1}{2}, 1$ with $(x_k, y_k)$ the lower left corner in the $k$th subrectangle (provided the subrectangle lies within $R$)  
    $V =\dfrac{1}{4}(-1+0) + \dfrac{1}{4}(-\dfrac{1}{2} + 0) +\dfrac{1}{8}(0 + 0) + \dfrac{1}{8}(\dfrac{1}{4} +0) + \dfrac{1}{4}(\dfrac{1}{2} + 0)$  
    $= \dfrac{17}{32}$  
#### Theory and Examples
75. circular sector Integrate $f(x, y) = \sqrt{4 - x^2}$ over the smaller sector cut from the disk $x^2 + y^2 \le 4$ by the rays $\theta = \dfrac{\pi}{6}$ and  $\theta = \dfrac{\pi}{2}$    
    $V = \int_0^2\int_{\frac{\sqrt{3}}{3}x}^{\sqrt{4-x^2}}\sqrt{4-x^2}dydx$    
    $=\int_0^2[\sqrt{4-x^2}y]_{y=\frac{\sqrt{3}}{3}x}^{y=\sqrt{4-x^2}}dx$  
    $= \int_0^2[4-x^2-\sqrt{4-x^2}\frac{\sqrt{3}}{3}x]dx$  
    Let $4-x^2 = u, \dfrac{du}{dx} =2x$  
    $\int_0^2\sqrt{4-x^2}\frac{\sqrt{3}}{3}xdx = \int_0^4\sqrt{u}\dfrac{\sqrt{3}}{6}du =\dfrac{\sqrt{3}}{6}\cdot\dfrac{2}{3}4^{\frac{3}{2}}=\dfrac{8\sqrt{3}}{9}$  
    $V = [4x-\dfrac{1}{3}x^3]_0^2- \dfrac{8\sqrt{3}}{9}$  
    $=8-\dfrac{8}{3}-\dfrac{8\sqrt{3}}{9}$
#### COMPUTER EXPLORATIONS
Use a CAS double-integral evaluator to estimate the values of the  integrals in Exercises 85–88.

85. $\int_1^3\int_1^x\dfrac{1}{xy}dydx$   
    $= \int_1^3[\dfrac{1}{x}\ln y]_1^xdx$  
    $= \int_1^3\dfrac{\ln x}{x}dx$  
### 15.3 Area by Double Integration
#### Area by Double Integrals
In Exercises 1–12, sketch the region bounded by the given lines and  curves. Then express the region’s area as an iterated double integral  and evaluate the integral.
1. The coordinate axes and the line $x + y = 2$  
   $A = \int_0^2\int_0^{2-x}dydx$  
   $=\int_0^22-xdx$  
   $= 2x-\dfrac{1}{2}x^2]_0^2=2$
#### Identifying the Region of Integration
The integrals and sums of integrals in Exercises 13–18 give the areas  of regions in the $xy$-plane. Sketch each region, label each bounding  curve with its equation, and give the coordinates of the points where  the curves intersect. Then find the area of the region

13. $\int_0^6\int_{\frac{1}{3}y^2}^{2y}dxdy$   
    $= \int_0^6[2y - \dfrac{1}{3}y^2]dy$  
    $= y^2-\dfrac{1}{9}y^3]_0^6 =36-24=12$
#### Finding Average Values
19. Find the average value of $f(x, y) = \sin (x + y)$ over  
a. the rectangle $0 \le x \le \pi, 0 \le y \le \pi$.  
b. the rectangle $0 \le x \le \pi, 0 \le y \le \dfrac{\pi}{2}$  
a. $\dfrac{1}{\pi^2}\int_0^{\pi}\int_0^{\pi}\sin (x + y)dydx$    
$= \dfrac{1}{\pi^2}\int_0^{\pi}[-\cos(x + y)]_0^{\pi}dx$  
$= \dfrac{1}{\pi^2}\int_0^{\pi}[-\cos(x + \pi)+\cos(x)]dx$    
$= \dfrac{1}{\pi^2}2\sin x]_0^{\pi}=0$  
b. $\dfrac{2}{\pi^2}\int_0^{\pi}\int_0^{\frac{\pi}{2}}\sin (x + y)dydx$    
$= \dfrac{2}{\pi^2}\int_0^{\pi}[-\cos(x + y)]_0^{\frac{\pi}{2}}dx$  
$= \dfrac{2}{\pi^2}\int_0^{\pi}[-\cos(x + \dfrac{\pi}{2})+\cos(x)]dx$    
$= \dfrac{2}{\pi^2}[-\cos x + \sin x]_0^{\pi}=\dfrac{4}{\pi^2}$
#### Theory and Examples
23. geometric area Find the area of the region
R: $0 \le x \le 2, 2 - x \le y \le \sqrt{4-x^2}$,
using (a) Fubini’s Theorem, (b) simple geometry  
a. $S = \int_0^2\int_{2-x}^{\sqrt{4-x^2}}dydx$  
$= \int_0^2[\sqrt{4-x^2}-2+x]dx$  
$= [\dfrac{x}{2}\sqrt{4-x^2}+2\arcsin \dfrac{x}{2}-2x+\dfrac{1}{2}x^2]_0^2$  
$=\pi-4+2=\pi -2$  
b. $S = \dfrac{1}{4}4\pi - \dfrac{1}{2}\cdot 2\cdot2 = \pi - 2$