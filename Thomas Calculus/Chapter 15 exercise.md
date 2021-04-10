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
### 15.6 Applications
#### Plates of Constant Density
1. Finding a center of mass Find the center of mass of a thin plate of density $\delta = 3$ bounded by the lines $x = 0, y = x$, and the parabola $y = 2 - x^2$ in the first quadrant  
   $x = 2-x^2, x > 0, x = 1$  
   $M = \int_0^1\int_{x}^{2-x^2} 3dydx$  
   $= \int_0^1[6-3x^2-3x]dx$  
   $= [6x-x^3-\dfrac{3}{2}x^2]_0^1 = \dfrac{7}{2}$  
   $M_y = \int_0^1\int_{x}^{2-x^2} 3xdydx$  
   $= \int_0^1[6x-3x^3-3x^2]dydx$  
   $=[3x^2-\dfrac{3}{4}x^4-x^3]_0^1 =\dfrac{5}{4}$  
   $M_x = \int_0^1\int_{x}^{2-x^2} 3ydydx$  
   $= \int_0^1[\dfrac{3}{2}(2-x^2)^2-\dfrac{3}{2}x^2]dx$  
   $=\int_0^1[\dfrac{3}{2}x^4-\dfrac{15}{2}x^2 + 6]dx$  
   $= [\dfrac{3}{10}x^5-\dfrac{5}{2}x^3+6x]_0^1 = \dfrac{19}{5}$  
   $\bar{x} = \dfrac{5}{14}, \bar{y} =\dfrac{38}{35}$  
#### Plates with Varying Density
11. Finding a moment of inertia Find the moment of inertia about the $x$-axis of a thin plate bounded by the parabola $x = y - y^2$ and the line $x + y = 0$ if $\delta(x, y) = x + y$.   
    $I_x= \int_{0}^2\int_{-y}^{y-y^2}(x+y)y^2dxdy$  
    $= \int_{0}^2[\dfrac{1}{2}y^2(y-y^2)^2+y^3(y-y^2)-\dfrac{1}{2}y^4+y^4]dy$  
    $=\int_{0}^2[(y-y^2)(\dfrac{3}{2}y^3-\dfrac{1}{2}y^4)+\dfrac{1}{2}y^4]dy$  
    $=\int_{0}^2[\dfrac{1}{2}y^6-2y^5-y^4]dy$  
    $= [\dfrac{1}{14}y^7-\dfrac{1}{3}y^6-\dfrac{1}{5}y^5]_{0}^2=\dfrac{64}{7}-\dfrac{64}{3}-\dfrac{32}{5} = \dfrac{960-2240-672}{105} = -\dfrac{1952}{105}$
#### Solids with Constant Density
21. Moments of inertia Find the moments of inertia of the rectangular solid shown here with respect to its edges by calculating $I_x$, $I_y$, and $I_z$.  
    ![](../images/Thomas%20Calculus/15-5.jpg)  
    $I_x = \int_0^a\int_0^b\int_0^c(y^2 + z^2)\delta dzdydx$  
    $= \int_0^a\int_0^b[y^2\delta c- \dfrac{1}{3}\delta c^3]dydx$  
    $= \int_0^a[\dfrac{1}{3}\delta c b^3 - \dfrac{1}{3}\delta c^3 b]dx$  
    $= \dfrac{1}{3}\delta c b^3a - \dfrac{1}{3}\delta c^3a b$   
    $I_x = \int_0^a\int_0^b\int_0^c(x^2 + z^2)\delta dzdydx$  
    $= \int_0^a\int_0^b[x^2\delta c- \dfrac{1}{3}\delta c^3]dydx$  
    $= \int_0^a[x^2 \delta c b - \dfrac{1}{3}\delta c^3 b]dx$  
    $= \dfrac{1}{3}\delta c ba^3 - \dfrac{1}{3}\delta c^3a b$  
    $I_z = \int_0^a\int_0^b\int_0^c(y^2 + x^2)\delta dzdydx$  
    $= \int_0^a\int_0^b[y^2\delta c- \delta x^2c]dydx$  
    $= \int_0^a[\dfrac{1}{3}\delta c b^3 - \delta x^2c b]dx$  
    $= \dfrac{1}{3}\delta c b^3a - \dfrac{1}{3}\delta ca^3 b$
#### Solids with Varying Density
In Exercises 29 and 30, find   
a. the mass of the solid. b. the center of mass.

29. A solid region in the first octant is bounded by the coordinate planes and the plane $x + y + z = 2$. The density of the solid is $\delta(x, y, z) = 2x$ gm/cm3.   
    a. $M = \int_0^2\int_0^{-x+2}\int_0^{2-x-y}2x dzdydx$  
    $= \int_0^2\int_0^{-x+2}[(2-x-y)2x]dydx$  
    $= \int_0^2\int_0^{-x+2}(-2x^2+4x-2xy)dydx$  
    $= \int_0^2((-2x^2+4x)(2-x)-x(2-x)^2)dx$   
    $= \int_0^2[2x^3-8x^2+8x-4x+4x^2-x^3]dx$  
    $= \int_0^2[x^3-4x^2+4x]dx$  
    $= [\dfrac{1}{4}x^4-\dfrac{4}{3}x^3+2x^2]_0^2=4-\dfrac{32}{3}+8 = \dfrac{4}{3}$  
    b. $M_{yz} =\int_0^2\int_0^{-x+2}\int_0^{2-x-y}2x^2 dzdydx$  
    $= \int_0^2\int_0^{-x+2}[(2-x-y)2x^2]dydx$  
    $= \int_0^2\int_0^{-x+2}(-2x^3+4x^2-2x^2y)dydx$  
    $= \int_0^2((-2x^3+4x^2)(2-x)-x^2(2-x)^2)dx$   
    $= \int_0^2[x^4-4x^3+4x^2]dx$  
    $= [\dfrac{1}{5}x^5-x^4+\dfrac{4}{3}x^3]_0^2=\dfrac{32}{5}-16+\dfrac{32}{3} = -\dfrac{48}{5}+\dfrac{32}{3}=\dfrac{16}{15}$  
    $M_{xz} =\int_0^2\int_0^{-x+2}\int_0^{2-x-y}2xy dzdydx$  
    $= \int_0^2\int_0^{-x+2}[(2-x-y)2xy]dydx$  
    $= \int_0^2\int_0^{-x+2}(-2x^2y+4xy-2xy^2)dydx$  
    $= \int_0^2((2x-x^2)(2-x)^2-\dfrac{2}{3}x(2-x)^3)dx$   
    $= \int_0^2[(4-4x+x^2)(2x-x^2-\dfrac{4}{3}x+\dfrac{2}{3}x^2)]dx$  
    $= \int_0^2[(4-4x+x^2)(\dfrac{1}{3}x^2+\dfrac{2}{3}x)]dx$   
    $= \int_0^2[\dfrac{1}{3}x^4-\dfrac{2}{3}x^3-\dfrac{4}{3}x^2+\dfrac{8}{3}x]dx$  
    $= [\dfrac{1}{15}x^5-\dfrac{1}{6}x^4-\dfrac{4}{9}x^3+\dfrac{4}{3}x^2]_0^2=\dfrac{32}{15}-\dfrac{8}{3}-\dfrac{32}{9}+\dfrac{16}{3} = \dfrac{32}{15}-\dfrac{8}{9}=\dfrac{56}{45}$   
    $M_{xy} =\int_0^2\int_0^{-x+2}\int_0^{2-x-y}2xz dzdydx$  
    $= \int_0^2\int_0^{-x+2}[(2-x-y)^2x]dydx$  
    $= \int_0^2\int_0^{-x+2}(4-4x+4y+x^2-2xy+y^2)xdydx$   
    $= \int_0^2((x^3-4x^2+4x)(2-x)+(2x-x^2)(2-x)^2+\dfrac{1}{3}x(2-x)^3)dx$  
    $= \int_0^2((x^3-4x^2+4x+x^3-4x^2+4x)(2-x)+\dfrac{1}{3}x(4-4x+x^2)(2-x))dx$   
    $= \int_0^2((2x^3-8x^2+8x)(2-x)+(\dfrac{4}{3}x-\dfrac{4}{3}x^2+\dfrac{1}{3}x^3)(2-x))dx$  
    $= \int_0^2((\dfrac{7}{3}x^3-\dfrac{28}{3}x^2+\dfrac{28}{3}x)(2-x))dx$   
    $= \int_0^2[-\dfrac{7}{3}x^4+14x^3-28x^2+\dfrac{56}{3}x]dx$  
    $= [-\dfrac{7}{15}x^5+\dfrac{7}{2}x^4-\dfrac{28}{3}x^3+\dfrac{28}{3}x^2]_0^2=-\dfrac{224}{15}+56-\dfrac{224}{3}+\dfrac{112}{3} = \dfrac{840}{15}-\dfrac{224}{15}-\dfrac{560}{15} = \dfrac{56}{15}$  
    $\bar{x}=\dfrac{4}{5},\bar{y}=\dfrac{14}{15},\bar{z}=\dfrac{14}{5}$ 
#### Theory and Examples
the parallel Axis theorem Let $L_{c.m.}$ be a line through the center of mass of a body of mass $m$ and let $L$ be a parallel line $h$ units away from $L_{c.m.}$. The Parallel Axis Theorem says that the moments of inertia $I_{c.m.}$ and $I_L$ of the body about $L_{c.m.}$ and $L$ satisfy the equation
$$
I_L = I_{c.m.} + mh^2
$$
As in the two-dimensional case, the theorem gives a quick way to calculate one moment when the other moment and the mass are known.

35. proof of the parallel Axis theorem  
    a. Show that the first moment of a body in space about any plane through the body’s center of mass is zero. (Hint: Place the body’s center of mass at the origin and let the plane be the $yz$-plane. What does the formula $\bar{x} = \dfrac{M_{yz}}{M}$ then tell you?)  
    ![](../images/Thomas%20Calculus/15-6.jpg)  
    b. To prove the Parallel Axis Theorem, place the body with its center of mass at the origin, with the line $L_{c.m.}$ along the $z$-axis and the line $L$ perpendicular to the $xy$-plane at the point $(h, 0, 0)$. Let $D$ be the region of space occupied by the body. Then, in the notation of the figure,  
    $$
    I_L = \iiint\limits_D|\mathbf{v}-h\mathbf{i}|^2dm
    $$
    Expand the integrand in this integral and complete the proof.   
    a. $\bar{x}=\bar{y}=\bar{z} = 0, \dfrac{M_{plane}}{M} = 0, M_{plane} = 0$  
    b.  $\mathbf{v}-h\mathbf{i} = (x-h,y,0)$  
    $\iiint\limits_D|\mathbf{v}-h\mathbf{i}|^2dm$  
    $=\iiint\limits_D(x^2-2xh+h^2+y^2)dm$  
    $\overrightarrow{PS} = (x-h,y,0)$  
    $r(x,y,z) = \dfrac{\begin{array}{cccc}\mathbf{i}&\mathbf{j}&\mathbf{k}\\x-h&y&0\\0&0&1\end{array}}{1}=y\mathbf{i} + (x-h)\mathbf{j}$  
    $I_{cm} = \iiint\limits_Dy^2+x^2-2xh+h^2dV$   
    $I_L = I_{c.m.} + mh^2$
#### Joint Probability Density Functions
For Exercises 39–42, verify that $f$ gives a joint probability density function. Then find the expected values $\mu X$ and $\mu Y$.

39. $f(x, y) = \begin{cases}x + y&\quad0\le x\le 1, 0\le y\le 1 \\0&\quad\mathsf{otherwise}\end{cases}$   
    $f(x,y)\ge 0$  
    $\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}f(x, y) dx dy$  
    $=\int_0^1\int_0^{1}x + ydxdy$  
    $=\int_0^1[\dfrac{1}{2}+y]dy$  
    $= 1$
### 15.7 Triple Integrals in Cylindrical and Spherical Coordinates
In Exercises 1–12, sketch the graph described by the following cylindrical coordinates in three-dimensional space.
1. $r = 2$  
#### Evaluating Integrals in Cylindrical Coordinates
Evaluate the cylindrical coordinate integrals in Exercises 23–28.

23. $\int_0^{2\pi}\int_0^1\int_r^{\sqrt{2-r^2}}dzrdrd\theta$   
    $= \int_0^{2\pi}\int_0^1[\sqrt{2-r^2}-r]rdrd\theta$  
    $\int_0^{2\pi}\int_0^1[r\sqrt{2-r^2}-r^2]drd\theta$  
    Let $2-r^2 = u,\dfrac{du}{dr} = -2r$  
    $\int_0^1r\sqrt{2-r^2}dr$  
    $=\int_1^2\dfrac{1}{2}\sqrt{u}dr$  
    $=[\dfrac{1}{3}u^{\frac{3}{2}}]_1^2=\dfrac{2\sqrt{2}}{3}-\dfrac{1}{3}$  
    $\int_0^{2\pi}\int_0^1\int_r^{\sqrt{2-r^2}}dzrdrd\theta$  
    $= \int_0^{2\pi}[\dfrac{2\sqrt{2}-2}{3}]d\theta$  
    $=\dfrac{4\sqrt{2}-2}{3}\pi$  
#### Changing the Order of Integration in Cylindrical Coordinates
The integrals we have seen so far suggest that there are preferred orders of integration for cylindrical coordinates, but other orders usually work well and are occasionally easier to evaluate. Evaluate the integrals in Exercises 29–32.

29. $\int_0^{2\pi}\int_0^3\int_0^{\frac{z}{3}}r^3drdzd\theta$   
    $= \int_0^{2\pi}\int_0^3[\dfrac{z^4}{108}]dzd\theta$  
    $= \int_0^{2\pi}\dfrac{243}{540}d\theta$  
    $=\dfrac{9}{10}\pi$
#### Finding Iterated Integrals in Cylindrical Coordinates
35. Give the limits of integration for evaluating the integral 
    $$
    \iiint f(r, \theta, z) dz r dr d\theta
    $$
    as an iterated integral over the region that is bounded below by the plane $z = 0$, on the side by the cylinder $r = \cos \theta$, and on top by the paraboloid $z = 3r^2$.   
    $\int_0^{2\pi}\int_0^1\int_0^{3r^2}r^3drdzd\theta$
#### Evaluating Integrals in Spherical Coordinates
Evaluate the spherical coordinate integrals in Exercises 43–48.

43. $\int_0^{\pi}\int_0^{\pi}\int_0^{2\sin\phi}\rho^2\sin\phi d\rho d\phi d\theta$   
    $= \int_0^{\pi}\int_0^{\pi}[\dfrac{1}{3}\sin\phi 8\sin^3\phi] d\phi d\theta$  
    $=\dfrac{8}{3}\int_0^{\pi}\int_0^{\pi}\sin^4\phi d\phi d\theta$  
    $= \dfrac{8}{3}\int_0^{\pi}\int_0^{\pi}(\dfrac{1-\cos2\phi}{2})^2 d\phi d\theta$  
    $\dfrac{2}{3}\int_0^{\pi}\int_0^{\pi}1-2\cos2\phi +\cos^22\phi d\phi d\theta$  
    $= \dfrac{2}{3}\int_0^{\pi}\int_0^{\pi}1-2\cos2\phi +\dfrac{1-\cos4\phi}{2} d\phi d\theta$  
    $= \dfrac{2}{3}\int_0^{\pi}[\dfrac{3}{2}\phi-\sin2\phi -\dfrac{1}{8}\sin 4\phi]_0^{\pi} d\theta$  
    $= \dfrac{2}{3}\int_0^{\pi}\dfrac{3}{2}\pi d\theta =\pi^2$  
#### Changing the Order of Integration in Spherical Coordinates
The previous integrals suggest there are preferred orders of integration for spherical coordinates, but other orders give the same value and are occasionally easier to evaluate. Evaluate the integrals in Exercises 49–52.  

49. $\int_0^{2}\int_{-\pi}^{0}\int_{\frac{\pi}{2}}^{\frac{\pi}{4}}\rho^3\sin2\phi d\phi d\theta d\rho$  
    $=\int_0^{2}\int_{-\\pi}^{0}[-\dfrac{1}{2}\rho^3\cos2\phi]_{\frac{\pi}{2}}^{\frac{\pi}{4}} d\theta d\rho$  
    $= \int_0^{2}\int_{-\pi}^{0}[-\dfrac{1}{2}\rho^3]d\theta d\rho$  
    $= \int_0^{2}[-\dfrac{1}{2}\rho^3\pi] d\rho$  
    $=-\rho^3\pi$
#### Finding Iterated Integrals in Spherical Coordinates
In Exercises 55–60, (a) find the spherical coordinate limits for the integral that calculates the volume of the given solid and then (b) evaluate the integral.  

55. The solid between the sphere $\rho = \cos\phi$ and the hemisphere $\rho = 2, z \ge 0$  
    ![](../images/Thomas%20Calculus/15-7.jpg)  
    $\int_0^{2\pi}\int_0^{\pi}\int_{\cos\phi}^{2}\rho^2\sin\phi d\rho d\phi d\theta$   
    $= \int_0^{2\pi}\int_0^{\pi}[\dfrac{8}{3}\sin\phi-\dfrac{\cos^3\phi\sin\phi}{3}]d\phi d\theta$   
    $\cos^3\phi\sin\phi = \cos\phi\sin\phi(1-\sin^2\phi)$  
    $= \dfrac{1}{2}\sin2\phi(1-\dfrac{1-\cos2\phi}{2})$
    $= \dfrac{1}{4}\sin2\phi +\dfrac{1}{4}\sin2\pi\cos2\phi = \dfrac{1}{4}\sin2\phi +\dfrac{1}{8}\sin4\phi$  
    $\int_0^{2\pi}\int_0^{\pi}\int_{\cos\phi}^{2}\rho^2\sin\phi d\rho d\phi d\theta$  
    $=\int_0^{2\pi}[-\dfrac{8}{3}\cos\phi+\dfrac{1}{2}\cos2\phi +\dfrac{1}{4}\cos4\phi]_0^{\pi} d\theta$  
    $=\int_0^{2\pi}[\dfrac{41}{12}+\dfrac{23}{12}]d\theta = \dfrac{32}{3}\pi$  
#### Finding Triple Integrals
61. Set up triple integrals for the volume of the sphere $\rho = 2$ in (a) spherical, (b) cylindrical, and (c) rectangular coordinates.   
    a. $\int_0^{2\pi}\int_0^{\pi}\int_{0}^{2}\rho^2\sin\phi d\rho d\phi d\theta$  
    b. $\int_0^{2\pi}\int_0^{2}\int_{-\sqrt[3]{8-r^3\cos^3\theta-r^3\sin^3\theta}}^{\sqrt[3]{8-r^3\cos^3\theta-r^3\sin^3\theta}} dz rdr d\theta$  
    c. $\int_{-2}^{2}\int_{-\sqrt{4-x^2}}^{\sqrt{4-x^2}}\int_{-\sqrt[3]{8-x^3-y^3}}^{\sqrt[3]{8-x^3-y^3}} dz dydx$  
#### Volumes
Find the volumes of the solids in Exercises 65–70.

65. ![](../images/Thomas%20Calculus/15-8.jpg)  
    $V =\int_0^{2\pi}\int_0^{1}\int_{r^4-1}^{4-4r^2} dz rdr d\theta$  
    $= \int_0^{2\pi}\int_0^{1}[5-4r^2-r^4]rdr d\theta$  
    $=\int_0^{2\pi}[\dfrac{5}{2}r^2-r^4-\dfrac{1}{6}r^6]_0^{1}d\theta$  
    $= \int_0^{2\pi}\dfrac{7}{6}d\theta = \dfrac{7}{3}\pi$
#### Average Values
85. Find the average value of the function $f(r, \theta, z) = r$ over the region bounded by the cylinder $r = 1$ between the planes $z = -1$ and $z = 1.$     
    $\dfrac{1}{2\pi}\int_0^{2\pi}\int_0^{1}\int_{-1}^{1} rdz rdr d\theta$  
    $= \dfrac{1}{2\pi}\int_0^{2\pi}\int_0^{1}2 r^2dr d\theta$  
    $= \dfrac{1}{2\pi}\int_0^{2\pi}\dfrac{2}{3} d\theta = \dfrac{2}{3}$
#### Masses, Moments, and Centroids
89. Center of mass A solid of constant density is bounded below by the plane $z = 0$, above by the cone $z = r, r \ge 0$, and on the sides by the cylinder $r = 1$. Find the center of mass.  
    $\bar{x} = \bar{y} = 0$  
    $M = \int_0^{2\pi}\int_0^{1}\int_{0}^{r} dz rdr d\theta$  
    $= \int_0^{2\pi}\int_0^{1} r^2dr d\theta$  
    $= \int_0^{2\pi}\dfrac{1}{3} d\theta$  
    $= \dfrac{2}{3}\pi$  
    $M_{r\theta} = \int_0^{2\pi}\int_0^{1}\int_{0}^{r} zdz rdr d\theta$  
    $= \int_0^{2\pi}\int_0^{1}\dfrac{1}{2} r^3dr d\theta$  
    $= \int_0^{2\pi}\dfrac{1}{6}  d\theta = \dfrac{1}{3}\pi$  
    $\bar{z} = \dfrac{1}{2}$
#### Theory and Examples
105. Vertical planes in cylindrical coordinates   
a. Show that planes perpendicular to the $x$-axis have equations of the form $r = a \sec \theta$ in cylindrical coordinates.  
b. Show that planes perpendicular to the $y$-axis have equations of the form $r = b \csc \theta$  
a. $x=a=r\cos\theta,r=a\sec\theta$    
b. $y=b=r\sin\theta,r=b\csc\theta$
### 15.8 Substitutions in Multiple Integrals
#### Jacobians and Transformed Regions in the Plane
1. a. Solve the system  
    $$
    u = x - y, v = 2x + y
    $$
    for $x$ and $y$ in terms of $u$ and $v.$ Then find the value of the Jacobian $\dfrac{\partial(x,y)}{\partial(u,v)}$.  
    b. Find the image under the transformation $u = x - y,v = 2x + y$ of the triangular region with vertices $(0, 0),(1, 1)$, and $(1, -2)$ in the $xy$-plane. Sketch the transformed region in the $uv$-plane.   
    a. $x = \dfrac{u + v}{3},y=-\dfrac{2}{3}u+\dfrac{1}{3}v$   
    $\dfrac{\partial(x,y)}{\partial(u,v)}=\dfrac{1}{3}\dfrac{1}{3}-(-\dfrac{2}{3}\dfrac{1}{3})= \dfrac{1}{3}$   
    $x-y = 0,v=0$  
    $2x + y=0,v=0$  
    $x=1,u +v = 3$  
#### Substitutions in Double Integrals
5. Evaluate the integral  
   $$
   \int_0^4\int_{\frac{y}{2}}^{\frac{y}{2} + 1}\dfrac{2x-y}{2}dxdy
   $$
   from Example 1 directly by integration with respect to $x$ and $y$ to confirm that its value is 2  
   $= \int_0^4[\dfrac{1}{2}x^2-\dfrac{y}{2}x]_{\frac{y}{2}}^{\frac{y}{2} + 1}dy$  
   $= \int_0^4[\dfrac{1}{2}(\dfrac{1}{4}y^2+y+1)-\dfrac{y}{2}(\dfrac{y}{2} + 1)-\dfrac{1}{2}\dfrac{y^2}{4}+\dfrac{y^2}{4}]_{\frac{y}{2}}^{\frac{y}{2} + 1}dy$  
   $= \int_0^4\dfrac{1}{2}dy = 2$
#### Substitutions in Triple Integrals
17. Evaluate the integral in Example 5 by integrating with respect to $x, y$, and $z$  
    $\int_0^3\int_0^4\int_{\frac{y}{2}}^{\frac{y}{2} + 1}\dfrac{2x-y}{2} + \dfrac{z}{3}dxdydz$  
    $= \int_0^3\int_0^4[\dfrac{1}{2} + \dfrac{yz}{6}+\dfrac{z}{3}-\dfrac{yz}{6}]dydz$  
    $= \int_0^32+\dfrac{4}{3}zdz$  
    $=[2z + \dfrac{2}{3}z^2]_0^3=12$
#### Theory and Examples
21. Find the Jacobian $\dfrac{\partial(x,y)}{\partial(u,v)}$ of the transformation  
a. $x = u \cos v, y = u \sin v$  
b. $x = u \sin v, y = u \cos v$  
a. $\cos v\cdot u\cos v-(-u\sin v\cdot\sin v)=u$  
b. $\sin v\cdot (-u\sin v)-(u\cos v\cdot\cos v)=-u$
### Practice Exercises
#### Evaluating Double Iterated Integrals
In Exercises 1–4, sketch the region of integration and evaluate the  double integral.

1. $\int_1^{10}\int_0^{\frac{1}{y}}ye^{xy}dxdy$  
   $=\int_1^{10}[e^{xy}]_0^{\frac{1}{y}}dy$  
   $= \int_1^{10}[e-1]dy=9e-9$  
#### Areas and Volumes Using Double Integrals
13. Area between line and parabola Find the area of the region  enclosed by the line $y = 2x + 4$ and the parabola $y = 4 - x^2$ in  the $xy$-plane.   
    $2x + 4 = 4-x^2, x_1 = -2, x_2 = 0$   
    $A = \int_{-2}^0\int_{2x + 4}^{4-x^2}dydx$  
    $=\int_{-2}^0-x^2 - 2xdx$  
    $= -\dfrac{1}{3}x^3 - x^2]_{-2}^0=\dfrac{4}{3}$  
#### Average Values
Find the average value of $f(x, y) = xy$ over the regions in Exercises  17 and 18.

17. The square bounded by the lines $x = 1, y = 1$ in the first quadrant   
    $\dfrac{1}{1}\int_0^1\int_0^1xydxdy$  
    $=\int_0^1\dfrac{1}{2}ydy$  
    $= \dfrac{1}{6}y^3]_0^1=\dfrac{1}{6}$
#### Polar Coordinates
Evaluate the integrals in Exercises 19 and 20 by changing to polar  coordinates.

19. $\int_{-1}^1\int_{-\sqrt{1-x^2}}^{\sqrt{1-x^2}}\dfrac{2dydx}{(1+x^2+y^2)^2}$  
    $\int_0^{2\pi}\int_0^1\dfrac{2rdrd\theta}{(1+r^2)^2}$  
    $=\int_0^{2\pi}\int_0^1\dfrac{2rdrd\theta}{(1+r^2)^2}$  
    Let $1 + r^2 = u,\dfrac{du}{dr} = 2r$  
    $\int_0^1\dfrac{2rdr}{(1+r^2)^2}$  
    $=\int_1^2\dfrac{du}{u^2}=[-\dfrac{1}{u}]_1^2=\dfrac{1}{2}$  
    $\int_0^{2\pi}\int_0^1\dfrac{2rdrd\theta}{(1+r^2)^2}$  
    $= \int_0^{2\pi}\dfrac{1}{2}d\theta = \pi$  
#### Evaluating Triple Iterated Integrals
Evaluate the integrals in Exercises 23–26 

23. $\int_0^{\pi}\int_0^{\pi}\int_0^{\pi}\cos(x+y+z)dxdydz$  
    $=\int_0^{\pi}\int_0^{\pi}[\sin(x + y + z)]_0^{\pi}dydz$  
    $=\int_0^{\pi}[2\cos( y + z)]_0^{\pi}dz$  
    $=-4\sin z]_0^{\pi}=0$
#### Volumes and Average Values Using Triple Integrals
27. Volume Find the volume of the wedge-shaped region enclosed  on the side by the cylinder $x = -\cos y, -\dfrac{\pi}{2} \le y \le \dfrac{\pi}{2}$, on the top by the plane $z = -2x$, and below by the $xy$-plane.  
    ![](../images/Thomas%20Calculus/15-9.jpg)  
    $-V = \int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\int_0^{-\cos y}\int_0^{-2x}dzdxdy$  
    $= \int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\int_0^{-\cos y}-2xdxdy$  
    $= \int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}[-\cos^2y]dy$  
    $= \int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}[-\dfrac{1+\cos 2y}{2}]dy$  
    $= [-\dfrac{1}{2}y-\dfrac{1}{4}\sin 2y]_{-\frac{\pi}{2}}^{\frac{\pi}{2}}=-\dfrac{\pi}{2}$  
    $V = \dfrac{\pi}{2}$
#### Cylindrical and Spherical Coordinates
31. Cylindrical to rectangular coordinates Convert    
    $$
    \int_0^{2\pi}\int_0^{\sqrt{2}}\int_r^{\sqrt{4-r^2}}3dzrdrd\theta
    $$  
    to (a) rectangular coordinates with the order of integration $dz dx dy$ and (b) spherical coordinates. Then (c) evaluate one of the integrals.    
    a. $\int_{-\sqrt{2}}^{\sqrt{2}}\int_{-\sqrt{2-y^2}}^{\sqrt{2-y^2}}\int_{\sqrt{x^2 + y^2}}^{\sqrt{4-x^2-y^2}}3dzdxdy$  
    b. $\int_0^{2\pi}\int_0^{\frac{\pi}{4}}\int_0^{2}3\rho^2\sin\phi d\rho d\phi d\theta$  
    c. $\int_0^{2\pi}\int_0^{\frac{\pi}{4}}\int_0^{2}3\rho^2\sin\phi d\rho d\phi d\theta$  
    $=\int_0^{2\pi}\int_0^{\frac{\pi}{4}}8\sin\phi d\phi d\theta$  
    $= \int_0^{2\pi}[-8\cos\phi]_0^{\frac{\pi}{4}}d\theta$  
    $= (16-8\sqrt{2})\pi$
#### Masses and Moments
38. Finding $I_z$ in spherical coordinates Find the moment of inertia about the z-axis of a solid of constant density $\delta = 1$ that is bounded above by the sphere $r = 2$ and below by the cone $\phi = \dfrac{\pi}{3}$ (spherical coordinates).   
    $I_z = \int_0^{2\pi}\int_0^{\frac{\pi}{3}}\int_0^{2}\rho^4\sin^2\phi d\rho d\phi d\theta$  
    $= \int_0^{2\pi}\int_0^{\frac{\pi}{3}}\dfrac{32}{5}\sin^2\phi  d\phi d\theta$  
    $= \int_0^{2\pi}\int_0^{\frac{\pi}{3}}\dfrac{16}{5}(1-\cos 2\phi) d\phi d\theta$  
    $=\dfrac{16}{5}\int_0^{2\pi}[\phi - \dfrac{1}{2}\sin2\phi]_0^{\frac{\pi}{3}} d\theta$
    $= \dfrac{16}{5}\int_0^{2\pi}[\dfrac{\pi}{3}-\dfrac{\sqrt{3}}{4}] d\theta=\dfrac{32}{15}\pi^2-\dfrac{8}{5}\sqrt{3}\pi$
#### Substitutions
53. Show that if $u = x - y$ and $y = v,$ then for any continuous $f$  
    $$
    \int_0^{\infty}\int_0^xe^{-sx}f(x-y,y)dydx=\int_0^{\infty}\int_0^{\infty}e^{-s(u+v)}f(u,v)dyd
    $$
    $x = u + v$
### Additional and Advanced Exercises
#### Volumes
1. Sand pile: double and triple integrals The base of a sand pile  covers the region in the $xy$-plane that is bounded by the parabola  $x^2 + y = 6$ and the line $y = x$. The height of the sand above the  point $(x, y)$ is $x^2$. Express the volume of sand as (a) a double integral, (b) a triple integral. Then (c) find the volume.  
   $V = \int_{-3}^2\int_x^{6-x^2}x^2dydx$  
   $= \int_{-3}^2\int_x^{6-x^2}\int_0^{x^2}dzdydx$  
   $= \int_{-3}^2[6x^2-x^4-x^3]dx$  
   $= [2x^3-\dfrac{1}{5}x^5-\dfrac{1}{4}x^4]_{-3}^2$  
    $=(16-\dfrac{32}{5}-4-(-54+\dfrac{243}{5}-\dfrac{91}{4}))$  
    $=66+\dfrac{81}{4}-\dfrac{275}{5}=\dfrac{44+81}{4}=\dfrac{125}{4}$  
#### Changing the Order of Integration
11. Evaluate the integral  
    $$
    \int_0^{\infty}\dfrac{e^{-ax}-e^{-bx}}{x}dx
    $$
     (Hint: Use the relation
     $$
    \dfrac{e^{-ax}-e^{-bx}}{x}=\int_a^be^{-x}dy
    $$ 
    to form a double integral and evaluate the integral by changing the order of integration.)  
    $\int_0^{\infty}\dfrac{e^{-ax}-e^{-bx}}{x}dx$  
    $=\int_0^{\infty}\int_a^be^{-x}dydx$  
    $= \int_a^b\int_0^{\infty}e^{-x}dxdy$  
    $= \int_a^b\lim\limits_{c\to\infty}[-e^{-c}+1]dy=b-a$
#### Masses and Moments
15. Minimizing polar inertia A thin plate of constant density is to  occupy the triangular region in the first quadrant of the $xy$-plane  having vertices $(0, 0), (a, 0),$ and $(a, \dfrac{1}{a})$. What value of a will minimize the plate’s polar moment of inertia about the origin?  
    $I_O = \int_0^a\int_0^{\frac{1}{a^2}x}(x^2 +y^2)dydx$  
    $= \int_0^a[\dfrac{1}{a^2}x^3+\dfrac{1}{3a^6}x^3]dx$  
    $=\dfrac{1}{4a^2}x^4 + \dfrac{1}{12a^6}x^4]_0^a=\dfrac{1}{4}a^2 + \dfrac{1}{12a^2}$    
    $\dfrac{dI_O}{da} = \dfrac{1}{2}a -\dfrac{1}{6a^3}=0$  
    $3a^4=1, a= \pm\dfrac{1}{\sqrt[4]{3}}$
#### Theory and Examples
19. Evaluate  
    $$
    \int_0^a\int_0^be^{\max(b^2x^2,a^2y^2)}dydx
    $$  
    where $a$ and $b$ are positive numbers and  
    $$
    \max(b^2x^2,a^2y^2)=\begin{cases}
        b^2 x^2 \quad&b^2 x^2\ge a^2 y^2  \\
        a^2 y^2 \quad&b^2 x^2< a^2 y^2 
    \end{cases}
    $$  
    if $b^2 x^2\ge a^2 y^2,y \le \dfrac{bx}{a}$  
    $\int_0^a\int_0^{\frac{bx}{a}}e^{\max(b^2x^2,a^2y^2)}dydx$  
    $=\int_0^a\int_0^{\frac{bx}{a}}e^{b^2x^2}dydx$   
    $=\int_0^a\dfrac{bx}{a}e^{b^2x^2}dx$  
    $=[\dfrac{b}{2a}xe^{b^2x^2}]_0^a=\dfrac{b}{2}e^{a^2b^2}$  
    if $b^2 x^2< a^2 y^2,x < \dfrac{ay}{b}$  
    $\int_0^a\int_0^{b}e^{\max(b^2x^2,a^2y^2)}dydx$  
    $=\int_0^{b}\int_0^{\frac{ay}{b}}e^{a^2y^2}dxdy$   
    $=\int_0^b\dfrac{ay}{b}e^{a^2y^2}dy$  
    $=[\dfrac{a}{2b}xe^{a^2y^2}]_0^b=\dfrac{a}{2}e^{a^2b^2}$