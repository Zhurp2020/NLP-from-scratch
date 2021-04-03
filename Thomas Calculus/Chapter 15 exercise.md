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
### 15.4 Double Integrals in Polar Form
#### Regions in Polar Coordinates
In Exercises 1–8, describe the given region in polar coordinates.
1. ![](../images/Thomas%20Calculus/15-2.jpg)   
   $r \le 9, -\dfrac{3}{2}\pi \le \theta \le 0$
#### Evaluating Polar Integrals
In Exercises 9–22, change the Cartesian integral into an equivalent polar integral. Then evaluate the polar integral.

9. $\int_{-1}^1\int_0^{\sqrt{1-x^2}}dydx$  
    $= \int_0^{\pi}\int_0^1rdrd\theta$  
    $=\int_0^{\pi}[\dfrac{1}{2}r^2]_0^1d\theta$  
    $=\int_0^{\pi}\dfrac{1}{2}d\theta$  
    $= \dfrac{\pi}{2}$
#### Area in Polar Coordinates
27. Find the area of the region cut from the first quadrant by the curve $r = 2(2 - \sin 2\theta)^{\frac{1}{2}}$   
    $A = \int_0^{\frac{1}{2}\pi}\int_0^{2(2 - \sin 2\theta)^{\frac{1}{2}}}rdrd\theta$  
    $=\int_0^{\frac{1}{2}\pi}[\dfrac{1}{2}r^2]_0^{2(2 - \sin 2\theta)^{\frac{1}{2}}}d\theta$  
    $=\int_0^{\frac{1}{2}\pi}[4-2\sin2\theta]d\theta$  
    $= [4\theta +\cos2\theta]_0^{\frac{1}{2}\pi}=2\pi$
#### Average Values
In polar coordinates, the average value of a function over a region $R$ (Section 15.3) is given by  
$$
\dfrac{1}{A(R)} \iint\limits_Rf(r,\theta)r drd\theta
$$
33. Average height of a hemisphere Find the average height of the hemispherical surface $z = \sqrt{a^2 - x^2 - y^2}$ above the disk $x^2 + y^2 \le a^2$ in the $xy$-plane   
    $\dfrac{1}{a^2\pi}\int_0^{2\pi}\int_0^{a}\sqrt{a^2-r^2\cos^2\theta - r^2\sin^2\theta}rdrd\theta$  
    Let $u = a^2-r^2,\dfrac{du}{dr} =-2r$   
    $\int_0^{a}\sqrt{a^2-r^2}rdr$  
    $= -\int_{a^2}^0\sqrt{u}2du$  
    $=-2[\dfrac{2}{3}u^{\frac{3}{2}}]_{a^2}^0$   
    $=\dfrac{4}{3}a^3$   
    $\dfrac{1}{a^2\pi}\int_0^{2\pi}\int_0^{a}\sqrt{a^2-r^2\cos^2\theta - r^2\sin^2\theta}rdrd\theta$  
    $= \dfrac{1}{a^2\pi}\int_0^{2\pi}\dfrac{4}{3}a^3d\theta$  
    $=\dfrac{1}{a^2\pi}\dfrac{32\pi^3}{3} = \dfrac{32}{3a^2}\pi^2$
#### Theory and Examples
37. converting to a polar integral Integrate $f(x, y) =\dfrac{\ln (x^2 + y^2)}{\sqrt{x^2 +y^2}}$ over the region $1 \le x^2 + y^2 \le e.$  
    $f(r,\theta) = \dfrac{\ln r^2}{\sqrt{r^2}} =\dfrac{2}{r}\ln r,1\le r \le \sqrt{e}$
#### COMPUTER EXPLORATIONS
In Exercises 49–52, use a CAS to change the Cartesian integrals into an equivalent polar integral and evaluate the polar integral. Perform the following steps in each exercise.   
a. Plot the Cartesian region of integration in the $xy$-plane.  
b. Change each boundary curve of the Cartesian region in part (a) to its polar representation by solving its Cartesian equation for $r$ and $\theta$.  
c. Using the results in part (b), plot the polar region of integration in the $r\theta$-plane.   
d. Change the integrand from Cartesian to polar coordinates. Determine the limits of integration from your plot in part (c) and evaluate the polar integral using the CAS integration utility.   

49. $\int_0^1\int_x^1\dfrac{y}{x^2+y^2}dydx$  
    $\dfrac{y}{x^2+y^2} = \dfrac{\sin\theta}{r}$  
    $y \ge x, \cos \theta \le \sin\theta,  \dfrac{1}{4}\pi\le \theta \le\dfrac{5}{4}\pi$  
    $y\le1, r\sin \theta \le 1,r\le\dfrac{1}{\sin\theta}$  
    $x \ge 0, r\cos\theta \ge 0,  -\dfrac{1}{2}\pi\le\theta\le\dfrac{1}{2}\pi$  
    $x \le 1, r\cos\theta \le 1,  r\le\dfrac{1}{\cos\theta}$  
    $\int_{\frac{1}{4}\pi}^{\frac{1}{2}\pi}\int_0^{\frac{1}{\sin\theta}}\sin\theta drd\theta$  
    $=\int_{\frac{1}{4}\pi}^{\frac{1}{2}\pi}1 d\theta = \dfrac{1}{2}\pi$
### 15.5 Triple Integrals in Rectangular Coordinates
#### Triple Integrals in Different Iteration Orders
1. Evaluate the integral in Example 3 taking $F(x, y, z) = 1$ to find the volume of the tetrahedron in the order $dz, dx, dy$.  
   $V = \int_0^1\int_0^y\int_0^{y-x} 1dzdxdy$  
   $=\int_0^1\int_0^y[y-x]dxdy$  
   $=\int_0^1[yx-\dfrac{1}{2}x^2]_0^ydy$  
   $= \int_0^1\dfrac{1}{2}y^2dy$  
   $= \dfrac{1}{6}y^3]_0^1 = \dfrac{1}{6}$
#### Evaluating Triple Iterated Integrals
Evaluate the integrals in Exercises 7–20.

7. $\int_0^1\int_0^1\int_0^1 (x^2 + y^2 + z^2)dzdydx$  
   $= \int_0^1\int_0^1[x^2z + y^2z + \dfrac{1}{3}z^3]_0^1dydx$  
   $=\int_0^1[x^2y + \dfrac{1}{3}y^3 + \dfrac{1}{3}y]_0^1dx$  
   $=[\dfrac{1}{3}x^3 + \dfrac{2}{3}x]_0^1 = 1$
#### Finding Equivalent Iterated Integrals
21. Here is the region of integration of the integral  
    $$
    \int_{-1}^1\int_{x^2}^1\int_0^{1-y} dzdydx
    $$  
    ![](../images/Thomas%20Calculus/15-3.jpg)  
    a. $dydzdx$  b. $dydxdz$  
    c. $dxdydz$  d. $dxdzdy$  
    e. $dzdxdy$  
    a. $\int_{-1}^1\int_{0}^{1-x^2}\int_{x^2}^{1-z} dydzdx$  
    b. $\int_{0}^1\int_{-\sqrt{1-z}}^{\sqrt{1-z}}\int_{x^2}^{1-z} dydxdz$  
    c. $\int_{0}^1\int_{0}^{1-y}\int_{-\sqrt{y}}^{\sqrt{y}} dxdydz$  
    d. $\int_{0}^1\int_{0}^{1-z}\int_{-\sqrt{y}}^{\sqrt{y}} dxdzdy$  
    e. $\int_{0}^1\int_{-\sqrt{y}}^{\sqrt{y}}\int_{0}^{1-y} dzdxdy$
#### Finding Volumes Using Triple Integrals
Find the volumes of the regions in Exercises 23–36.

23. The region between the cylinder $z = y^2$ and the $xy$-plane that is bounded by the planes $x = 0, x = 1, y = -1, y = 1$   
    ![](../images/Thomas%20Calculus/15-4.jpg)  
    $V =\int_{-1}^1\int_{0}^{1}\int_{0}^{y^2} dzdxdy$   
    $=\int_{-1}^1\int_{0}^{1}[y^2]dxdy$  
    $=\int_{-1}^1[y^2]dy = \dfrac{2}{3}$  
#### Average Values
In Exercises 37–40, find the average value of $F(x, y, z)$ over the given region.

37. $F(x, y, z) = x^2 + 9$ over the cube in the first octant bounded by the coordinate planes and the planes $x = 2, y = 2$, and $z = 2$  
    $\dfrac{1}{8}\int_0^2\int_0^2\int_0^2 x^2 + 9 dzdydx$  
    $=\dfrac{1}{8}\int_0^2\int_0^2[2x^2 + 18]dydx$  
    $=\dfrac{1}{8}\int_0^2[4x^2 + 36]dydx$  
    $=\dfrac{1}{8}[\dfrac{4}{3}x^3 + 36x]_0^2=9 + \dfrac{4}{3}=\dfrac{31}{3}$
#### Changing the Order of Integration
Evaluate the integrals in Exercises 41–44 by changing the order of integration in an appropriate way.

41. $\int_0^4\int_0^1\int_{2y}^2 \dfrac{4\cos x^2}{2\sqrt{z}}dxdydz$  
    $= \int_0^4\int_{0}^2\int_0^{\frac{1}{2}x} \dfrac{4\cos x^2}{2\sqrt{z}}dydxdz$  
    $=\int_0^4\int_{0}^2[\dfrac{2x\cos x^2}{2\sqrt{z}}]dxdz$  
    $= \int_{0}^2\int_0^4[\dfrac{2x\cos x^2}{2\sqrt{z}}]dzdx$  
    $= \int_{0}^2[4x\cos x^2]dx$  
    Let $u = x^2, \dfrac{du}{dx} = 2x$  
    $\int_{0}^2[4x\cos x^2]dx$  
    $=2\int_{0}^4\cos udu = 2\sin 4$  
#### Theory and Examples
45. Finding an upper limit of an iterated integral Solve for $a$:  
    $$
    \int_0^1\int_0^{4-a-x^2}\int_{a}^{4-x^2-y} dzdydx=\dfrac{4}{15}
    $$   
    $\int_0^1\int_0^{4-a-x^2}[4-x^2-y -a]dydx=\dfrac{4}{15}$   
    $\int_0^1[4y-x^2y-\dfrac{1}{2}y^2 -ay]_0^{4-a-x^2}dx=\dfrac{4}{15}$  
    $\int_0^1[(4-x^2-a)(4-a-x^2)-\dfrac{1}{2}(4-a-x^2)^2]dx=\dfrac{4}{15}$  
    $\int_0^1[\dfrac{1}{2}(x^4-2(4-a)x^2 + 16-8a+a^2)]dx=\dfrac{4}{15}$  
    $\dfrac{1}{2}[\dfrac{1}{5}x^5-\dfrac{1}{3}(8-2a)x^3 + (16-8a+a^2)x]_0^1=\dfrac{4}{15}$  
    $\dfrac{1}{5}-\dfrac{8}{3}+\dfrac{2}{3}a + 16-8a+a^2 =\dfrac{8}{15}$  
    $a^2-\dfrac{22}{3}a + 16 -\dfrac{37}{15}-\dfrac{8}{15} = 0$  
    $3a^2-22a +39=0$   
    $a_1 = 3, a_2 = \dfrac{13}{3}(4-a-x^2 < 0)$  
    $a = 3$
#### COMPUTER EXPLORATIONS
In Exercises 49–52, use a CAS integration utility to evaluate the triple integral of the given function over the specified solid region.

49. $F(x, y, z) = x^2y^2z$ over the solid cylinder bounded by $x^2 + y^2 = 1$ and the planes $z = 0$ and $z = 1$  
    $\int_{-1}^1\int_{-\sqrt{1-x^2}}^{\sqrt{1-x^2}}\int_0^1x^2y^2zdzdydx$  
    $= \int_{-1}^1\int_{-\sqrt{1-x^2}}^{\sqrt{1-x^2}}[\dfrac{1}{2}x^2y^2]dydx$  
    $= \dfrac{1}{2}\int_{-1}^1[2x^2\sqrt{1-x^2}^{\frac{3}{2}}]dydx = 0$