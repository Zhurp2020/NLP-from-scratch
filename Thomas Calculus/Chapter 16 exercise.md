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
### 16.4 Green’s Theorem in the Plane
#### Computing the $\mathbf{k}$-Component of $(\mathsf{curl} \mathbf{F})$
In Exercises 1–6, find the $\mathbf{k}$-component of $(\mathsf{curl} \mathbf{F})$ for the following vector fields on the plane.
1. $\mathbf{F} = (x + y)\mathbf{i} + 2xy\mathbf{j}$  
   $= 2y-1$
#### Verifying Green’s Theorem
In Exercises 7–10, verify the conclusion of Green’s Theorem by evaluating both sides of Equations (3) and (4) for the field $\mathbf{F} = M\mathbf{i} + N\mathbf{j}$. Take the domains of integration in each case to be the disk $R: x^2 + y^2 \le a^2$ and its bounding circle $C: \mathbf{r} = (a \cos t)\mathbf{i} + (a \sin t)\mathbf{j}, 0 \le t \le 2\pi.$

7. $\mathbf{F} = -y\mathbf{i} + x\mathbf{j}$  
   a. $\int_0^{2\pi}(-a\sin t\mathbf{i} + a\cos t\mathbf{j})(-a\sin t\mathbf{i} + a\cos t\mathbf{j})dt$  
   $= \int_0^{2\pi}a^2dt=2a^2\pi$  
   $\int_{-a}^a\int_{-\sqrt{a^2-y^2}}^{\sqrt{a^2-y^2}}2dxdy$  
   $= \int_{-a}^a4\sqrt{a^2-y^2}dy$  
   $= 4[\dfrac{y}{2}\sqrt{a^2-y^2}+\dfrac{a^2}{2}\arcsin\dfrac{a}{y}]_{-a}^a$  
   $= 4\dfrac{a^2}{2}\dfrac{\pi}{2}+\dfrac{a^2}{2}\dfrac{1}{2}\pi =2a^2\pi$  
   b. $\int_0^{2\pi}(-a^2\sin t\cos t +a^2\cos t\sin t)dt = 0$  
   $\int_{-a}^a\int_{-\sqrt{a^2-y^2}}^{\sqrt{a^2-y^2}}0dxdy=0$
#### Circulation and Flux
In Exercises 11–20, use Green’s Theorem to find the counterclockwise circulation and outward flux for the field $\mathbf{F}$ and curve $C$.

11. $\mathbf{F} = (x - y)\mathbf{i} + (y - x)\mathbf{k}$  
$C$: The square bounded by $x = 0, x = 1, y = 0, y = 1$   
a. $\int_0^1\int_0^1(-1+1)dxdy = 0$  
b. $\int_0^1\int_0^1(1+1)dxdy = \int_0^14dy = 4$
#### Work
In Exercises 25 and 26, find the work done by $\mathbf{F}$ in moving a particle once counterclockwise around the given curve.

25. $\mathbf{F} = 2xy^3\mathbf{i} + 4x^2y^2\mathbf{k}$  
$C$: The boundary of the “triangular” region in the first quadrant enclosed by the $x$-axis, the line $x = 1$, and the curve $y = x^3$   
$\int_0^1\int_0^{x^3}(8y^2x-6xy^2)dydx$  
$= \int_0^1[\dfrac{8}{3}y^3x-2xy^3]_0^{x^3}dx$  
$= \int_0^1\dfrac{2}{3}x^{10}dx = \dfrac{2}{33}$  
#### Using Green’s Theorem
Apply Green’s Theorem to evaluate the integrals in Exercises 27–30.

27. $\oint(y^2 dx + x^2 dy)$  
$C$: The triangle bounded by $x = 0, x + y = 1, y = 0$   
$= \int_0^1\int_0^{1-x}2x-2ydydx$  
$= \int_0^1[2xy-y^2]_0^{1-x}dx$  
$= \int_0^1(2x-2x^2-1+2x-x^2)dx =-2$  
#### COMPUTER EXPLORATIONS
In Exercises 49–52, use a CAS and Green’s Theorem to find the counterclockwise circulation of the field F around the simple closed curve  
C. Perform the following CAS steps.  
a. Plot $C$ in the $xy$-plane.  
b. Determine the integrand $\dfrac{\partial N}{\partial x} - \dfrac{\partial M}{\partial y}$ for the tangential form of Green’s Theorem.  
c. Determine the (double integral) limits of integration from your plot in part (a) and evaluate the curl integral for the circulation.

49. $\mathbf{F} = (2x - y)\mathbf{i} + (x + 3y)\mathbf{j},$   
    $C$: The ellipse $x^2 + 4y^2 = 4$   
    $\dfrac{\partial N}{\partial x} - \dfrac{\partial M}{\partial y} = 1+1 =2$  
    $\int_{-2}^2\int_{-\frac{\sqrt{4-x^2}}{2}}^{\frac{\sqrt{4-x^2}}{2}}2dydx$  
    $= \int_{-2}^22\dfrac{\sqrt{4-x^2}}{2}dx$  
    $= [\dfrac{x}{2}\sqrt{4-x^2}+2\arcsin\dfrac{x}{2}]_{-2}^2$  
    $= [\pi+\pi ] = 2\pi$
### 16.5 Surfaces and Area
#### Finding Parametrizations
In Exercises 1–16, find a parametrization of the surface. (There are many correct ways to do these, so your answers may not be the same as those in the back of the book.)
1. The paraboloid $z = x^2 + y^2, z \le 4$  
   $\mathbf{r}(r, \theta) = r\cos \theta\mathbf{i} + r\sin \theta\mathbf{j} + r^2\mathbf{k},0\le r \le 2, 0\le \theta \le 2\pi$
#### Surface Area of Parametrized Surfaces
In Exercises 17–26, use a parametrization to express the area of the surface as a double integral. Then evaluate the integral. (There are many correct ways to set up the integrals, so your integrals may not be the same as those in the back of the book. They should have the same values, however.)

17. Tilted plane inside cylinder The portion of the plane $y + 2z = 2$ inside the cylinder $x^2 + y^2 = 1$   
    $\mathbf{r}(r,\theta) = r\cos\theta\mathbf{i} + r\sin\theta\mathbf{j} + \dfrac{2-r\sin\theta}{2}\mathbf{k}, 0\le r \le 1,0\le\theta \le 2\pi$  
    $\mathbf{r}_r = \cos\theta\mathbf{i} + \sin\theta\mathbf{j} - \dfrac{\sin\theta}{2}\mathbf{k}$  
    $\mathbf{r}_{\theta} = -r\sin\theta\mathbf{i} + r\cos\theta\mathbf{j} - \dfrac{r\cos\theta}{2}\mathbf{k}$   
    $\mathbf{r}_r\times \mathbf{r}_{\theta} = |\begin{array}{cccc}\mathbf{i}&\mathbf{j}&\mathbf{k} \\  \cos\theta& \sin\theta& \dfrac{\sin\theta}{2}\\-r\sin\theta& r\cos\theta& \dfrac{r\cos\theta}{2}\\ \end{array}|$  
    $= \dfrac{r}{2}\mathbf{j} +r\mathbf{k}$  
    $A = \int_0^1\int_0^{2\pi}\sqrt{\dfrac{5}{4}r^2}d\theta dr$  
    $=  \int_0^1\sqrt{5}\pi r dr=\dfrac{\sqrt{5}}{2}\pi$  
#### Planes Tangent to Parametrized Surfaces
The tangent plane at a point $P_0(f(u_0, v_0), g(u_0, v_0), h(u_0, v_0))$ on a parametrized surface $\mathbf{r}(u, v) = f(u, v)\mathbf{i} + g(u, v)\mathbf{j} + h(u, v)\mathbf{k}$ is the plane through $P_0$ normal to the vector $\mathbf{r}_u(u_0, v_0) \times \mathbf{r}_v(u_0, v_0)$, the cross product of the tangent vectors $\mathbf{r}_u(u_0, v_0)$ and $\mathbf{r}_v(u_0, v_0)$ at $P_0$. In Exercises 27–30, find an equation for the plane tangent to the surface at $P_0$. Then find a Cartesian equation for the surface and sketch the surface and tangent plane together.

27. Cone The cone $\mathbf{r}(r,\theta) = r\cos\theta\mathbf{i} + r\sin\theta\mathbf{j} + r\mathbf{k}, r \ge 0,0\le\theta \le 2\pi$ at the point $P(\sqrt{2},\sqrt{2},2)$ corresponding to $(r, \theta) = (2, \dfrac{\pi}{4})$   
    $\mathbf{r}_r = \cos\theta\mathbf{i} + \sin\theta\mathbf{j} +\mathbf{k}$  
    $\mathbf{r}_{\theta} = -r\sin\theta\mathbf{i} + r\cos\theta\mathbf{j}$   
    $\mathbf{r}_r\times \mathbf{r}_{\theta} = |\begin{array}{cccc}\mathbf{i}&\mathbf{j}&\mathbf{k} \\  \cos\theta& \sin\theta& 1\\-r\sin\theta& r\cos\theta& 0\\ \end{array}|$  
    $= -r\cos\theta\mathbf{i} + r\sin\theta\mathbf{j} +r\mathbf{k}$  
    $=-\sqrt{2}\mathbf{i} + \sqrt{2}\mathbf{j} +2\mathbf{k}$  
    $x^2 +y^2=z^2$  
    $-\sqrt{2}(x-\sqrt{2})+\sqrt{2}(y-\sqrt{2})+2(z-2) = 0$  
#### More Parametrizations of Surfaces
31. a. A torus of revolution (doughnut) is obtained by rotating a circle $C$ in the $xz$-plane about the $z$-axis in space. (See the accompanying figure.) If $C$ has radius $r \ge 0$ and center $(R, 0, 0)$, show that a parametrization of the torus is 
    $$
    \mathbf{r}(u, v) = ((R + r \cos u)\cos v)\mathbf{i}+ ((R + r \cos u)\sin v)\mathbf{j} + (r \sin u)\mathbf{k}
    $$
    where $0 \le u \le 2\pi$ and $0 \le v \le 2\pi$ are the angles in the figure.   
    b. Show that the surface area of the torus is $A = 4\pi^2Rr.$  
    ![](../images/Thomas%20Calculus/16-2.jpg)  
    $x_1 = R+r\cos u, z = r\sin u$  
    $x = x_1\cos v, y = x_1\sin v$  
    $\mathbf{r}_u = -r\cos v\sin u\mathbf{i} -r\sin v\sin u\mathbf{j} +r\cos u\mathbf{k}$  
    $\mathbf{r}_v = -(R + r\cos u)\sin v\mathbf{i} + (R + r\cos u)\cos v\mathbf{j}$   
    $\mathbf{r}_r\times \mathbf{r}_{\theta} = |\begin{array}{cccc}\mathbf{i}&\mathbf{j}&\mathbf{k} \\ -r\cos v\sin u& -r\sin v\sin u& r\cos u\\-(R + r\cos u)\sin v& (R + r\cos u)\cos v& 0\\ \end{array}|$  
    $= (R + r\cos u)r\cos v\cos u\mathbf{i} + (R + r\cos u)r\sin v\cos u\mathbf{j} -(R + r\cos u)r\sin u\mathbf{k}$  
    $S = \int_0^{2\pi}\int_0^{2\pi}\sqrt{(R + r\cos u)^2r^2\cos^2u + (R + r\cos u)^2r^2\sin^2u}dudv$  
    $= \int_0^{2\pi}\int_0^{2\pi}(R + r\cos u)rdudv$  
    $= \int_0^{2\pi}[Rru + r^2\sin u]_0^{2\pi}dv$  
    $= \int_0^{2\pi}2Rr\pi dv = 4Rr\pi^2$
#### Surface Area for Implicit and Explicit Forms
37. Find the area of the surface cut from the paraboloid $x^2 + y^2 - z =0$ by the plane $z = 2.$  
    $x^2 +y^2 = 2$  
    $A=2\pi$  
### 16.6 Surface Integrals
#### Surface Integrals of Scalar Functions
In Exercises 1–8, integrate the given function over the given surface.
1. Parabolic cylinder $G(x, y, z) = x,$ over the parabolic cylinder  $y = x^2, 0\le x \le 2, 0 \le z \le 3$  
   $\nabla F=2x\mathbf{i}-\mathbf{j}$  
   $\iint_Rx\dfrac{\sqrt{4x^2 + 1}}{1}A$  
   $= \int_0^2\int_0^3x\sqrt{4x^2 + 1}dzdx$  
   $= \int_0^23x\sqrt{4x^2 + 1}dx$  
   Let $4x^2 + 1 = u,\dfrac{du}{dx} = 8x$  
   $= \int_1^{17}\sqrt{u}\dfrac{3}{8}du$  
   $=\dfrac{1}{4}u^{\frac{3}{2}}]_1^{17}=\dfrac{17\sqrt{17}-1}{4}$
#### Finding Flux or Surface Integrals of Vector Fields
In Exercises 19–28, use a parametrization to find the flux $\iint\limits_S\mathbf{F}\cdot\mathbf{n}d\sigma$ across the surface in the specified direction.

19. Parabolic cylinder $\mathbf{F}= z^2\mathbf{i}+ x\mathbf{j} -3z\mathbf{k}$ outward (normal away from the $x$-axis) through the surface cut from the parabolic cylinder $z = 4 -y^2$ by the planes $x = 0, x = 1,$ and $z = 0$  
    $x=x,y=y,z=4-y^2$  
    $\mathbf{r}(x,y)=x\mathbf{i}+ y\mathbf{j} +(4-y^2)\mathbf{k}$  
    $\mathbf{r}_x\times\mathbf{r}_y=$  
    $|\begin{array}{cccc}\mathbf{i}&\mathbf{j}&\mathbf{k} \\ 1& 0& 0\\0& 1& -2y\\ \end{array}|=-2y\mathbf{j} +\mathbf{k}$  
   $\iint\limits_S\mathbf{F}\cdot\mathbf{n}d\sigma$  
   $= \int_{-2}^2\int_0^1(-2xy-3z)dxdy$  
   $=\int_{-2}^2\int_0^1(-2xy-12+3y^2)dxdy$  
   $=\int_{-2}^2[3y^2-y-12]dy$  
   $=[y^3-\dfrac{1}{2}y^2-12y]_{-2}^2=-18-(-10+24)=-32$
#### Moments and Masses
43. Centroid Find the centroid of the portion of the sphere  $x^2 + y^2 + z^2 = a^2$ that lies in the first octant.  
    $M = \iint_Rd\sigma = \dfrac{1}{2}a^2\pi$  
    $M_{xy} = 2\pi a^3$  
    $C(\dfrac{a}{2},\dfrac{a}{2},\dfrac{a}{2})$
### 16.7 Stokes’ Theorem
In Exercises 1–6, find the curl of each vector field $\mathbf{F}$.
1. $\mathbf{F} = (x + y - z)\mathbf{i} + (2x - y + 3z)\mathbf{j} + (3x + 2y + z)\mathbf{k}$   
   $\nabla \cdot F = (2-3)\mathbf{i} + (-1-3)\mathbf{j} + (2-1)\mathbf{k} = -\mathbf{i} -4\mathbf{j} + \mathbf{k}$
#### Using Stokes’ Theorem to Find Line Integrals
In Exercises 7–12, use the surface integral in Stokes’ Theorem to calculate the circulation of the field $\mathbf{F}$ around the curve $C$ in the indicated direction.

7. $\mathbf{F} = x^2\mathbf{i} + 2x\mathbf{j} + z^2\mathbf{k}$  
$C$: The ellipse $4x^2 + y^2 = 4$ in the $xy$-plane, counterclockwise  when viewed from above   
    $\nabla \cdot F = 2\mathbf{k}$  
    $\mathbf{n}=\mathbf{k}$  
    $\oint\limits_C\mathbf{F}\cdot dr = \iint\limits_S(\nabla \times F)\cdot \mathbf{n}dr$  
    $=\iint_R2dxdy = 2\pi ab=4\pi$  
#### Integral of the Curl Vector Field
13. Let $\mathbf{n}$ be the outer unit normal of the elliptical shell 
    $$
    S: 4x^2 + 9y^2 + 36z^2 = 36, z \ge 0
    $$ 
    , and let
    $$
    \mathbf{F} = y\mathbf{i} + x^2\mathbf{j} +(x^2+y^4)^{\frac{3}{2}}\sin e^{\sqrt{xyz}}\mathbf{k}
    $$
    Find the value of
    $$
    \iint\limits_S(\nabla \times F)\cdot \mathbf{n}dr
    $$
    (Hint: One parametrization of the ellipse at the base of the shell is  $x = 3 \cos t, y = 2 \sin t, 0 \le t \le 2\pi.$)  
    $\mathbf{r}(t) = 3 \cos t\mathbf{i} +2 \sin t\mathbf{j}$  
    $\dfrac{d\mathbf{r}}{dt} = -3 \sin t\mathbf{i} +2 \cos t\mathbf{j}$  
    $\oint\limits_C\mathbf{F}\cdot dr = \iint\limits_S(\nabla \times F)\cdot \mathbf{n}dr$  
    $\mathbf{F}\cdot dr=-6\sin^2t\mathbf{i} +18 \cos^2 t\mathbf{j}$  
    $\oint\limits_C\mathbf{F}\cdot dr=\int_0^{2\pi}-6\sin^2t\mathbf{i} +18 \cos^2 t\mathbf{j}dt=-6\pi$  
#### Stokes’ Theorem for Parametrized Surfaces
In Exercises 19–24, use the surface integral in Stokes’ Theorem to  calculate the flux of the curl of the field $\mathbf{F}$ across the surface $S$ in the direction of the outward unit normal $\mathbf{n}.$

19. $\mathbf{F} = 2z\mathbf{i} + 3x\mathbf{j} +5y\mathbf{k}$  
$S: \mathbf{r}(r,\theta) = r\cos \theta\mathbf{i} +r \sin \theta\mathbf{j} + (4-r^2) \mathbf{k},0\le r\le 2, 0\le \theta \le 2\pi$    
$\mathbf{r}_r=\cos\theta\mathbf{i} +\sin \theta\mathbf{j} -2r\mathbf{k}$  
$\mathbf{r}_{\theta}=-r\sin\theta\mathbf{i} +r\cos \theta\mathbf{j}$   
$N = \mathbf{r}_r\times\mathbf{r}_{\theta} = 2r^2\cos\theta\mathbf{i} +2r^2\sin \theta\mathbf{j}+r\mathbf{k}$   
$\nabla \times F = 5\mathbf{i} +2\mathbf{j}+3\mathbf{k}$  
$\iint\limits_S(\nabla \times F)\cdot \mathbf{n}dr=12\pi$
#### Theory and Examples
25. Let $C$ be the smooth curve $\mathbf{r}(t)=2\cos t\mathbf{i} +2\sin t\mathbf{j} + (3-2\cos^3t)\mathbf{k}$, oriented to be traversed counterclockwise around the $z$-axis when viewed from above. Let $S$ be the piece-wise smooth cylindrical surface $x^2 + y^2 = 4,$ below the curve for $z \ge 0$, together with the base disk in the $xy$-plane. Note that $C$ lies on the cylinder $S$ and above the $xy$-plane (see the accompanying  figure). Verify Equation (4) in Stokes’ Theorem for the vector field  $\mathbf{F}=y\mathbf{i} -x\mathbf{j} + x^2\mathbf{k}$  
![](../images/Thomas%20Calculus/16-3.jpg)  
$\dfrac{d\mathbf{r}}{dt}=-2\sin t\mathbf{i} +2\cos t\mathbf{j} + 6\cos^2t\sin t\mathbf{k}$  
$\mathbf{F}\cdot d\mathbf{r}=4(6\cos^4t\sin t-1)dt$  
$\oint\mathbf{F}\cdot d\mathbf{r}=-8\pi$  
$\nabla\times \mathbf{F}=-2x\mathbf{j} +2\mathbf{k}$  
$\nabla\times \mathbf{F}\cdot \mathbf{n}=-2$  
$\iint\limits_S(\nabla \times F)\cdot \mathbf{n}dr=-8\pi$
### 16.8 The Divergence Theorem and a Unified Theory
#### Calculating Divergence
In Exercises 1–8, find the divergence of the field.
1. $\mathbf{F} = (x-y+z)\mathbf{i} + (2x + y -z)\mathbf{j} +(3x + 2y-2z)\mathbf{k}$  
   div $\mathbf{F} = 1+1-2 = 0$
#### Calculating Flux Using the Divergence Theorem
In Exercises 9–20, use the Divergence Theorem to find the outward flux of $\mathbf{F}$ across the boundary of the region $D$.

9. Cube $\mathbf{F} = (y-x)\mathbf{i} + (z-y)\mathbf{j} +(y-x)\mathbf{k}$
D: The cube bounded by the planes $x = \pm 1, y = \pm 1$, and $z = \pm 1$  
flux $=\iiint_D(-1-1+0)dV$  
$= \int_{-1}^1\int_{-1}^1\int_{-1}^1(-2)dxdydz$  
$=-16$
#### Theory and Examples
21. a. Show that the outward flux of the position vector field $\mathbf{F} = x\mathbf{i} + y\mathbf{j} +z\mathbf{k}$ through a smooth closed surface $S$ is three times the volume of the region enclosed by the surface.  
b. Let $\mathbf{n}$ be the outward unit normal vector field on $S$. Show that it is not possible for $\mathbf{F}$ to be orthogonal to $\mathbf{n}$ at every point of $S$.  
a. flux $= \iiint_D3dV = 3V$  
b. If orthogonal at every point, flux = 0, False. 
### Practice Exercises
#### Evaluating Line Integrals
1. The accompanying figure shows two polygonal paths in space joining the origin to the point $(1, 1, 1)$. Integrate $f(x, y, z) =2x - 3y^2 - 2z + 3$ over each path.
   ![](../images/Thomas%20Calculus/16-4.jpg)
    p1: $\mathbf{r}(t) = t\mathbf{i} + t\mathbf{j} +t\mathbf{k}$  
    $\int_Cfds$  
    $= \int_0^1(2t-3t^2-2t+3)\sqrt{3}dt$  
    $= \int_0^1-3\sqrt{3}t^2+3\sqrt{3}dt$  
    $= 2\sqrt{3}$  
p2: C_1 : $\mathbf{r}(t) = t\mathbf{i} + t\mathbf{j}$  
C_2 : $\mathbf{r}(t) = \mathbf{i} + \mathbf{j} +t\mathbf{k}$   
$\int_Cfds$  
$= \int_0^1(2t-3t^2+3)\sqrt{2}dt + \int_0^1(2-2t)tdt$  
$= 3\sqrt{2} +1$
#### Finding and Evaluating Surface Integrals
11. Area of an elliptical region Find the area of the elliptical region cut from the plane $x + y + z = 1$ by the cylinder $x^2 + y^2 = 1$   
    $z = 1-x-y$  
    $A = \iint\sqrt{1+1+1}dA$  
    $= \int_0^{2\pi}\int_0^1\sqrt{3}rdrd\theta$  
    $=\sqrt{3}\pi$  
#### Parametrized Surfaces
Find parametrizations for the surfaces in Exercises 19–24. (There are many ways to do these, so your answers may not be the same as those in the back of the book.)

19. Spherical band The portion of the sphere $x^2 + y^2 + z^2 = 36$ between the planes $z = -3$ and $z = 3\sqrt{3}$   
    $\mathbf{r}(\theta,\phi) = 6\sin\phi\cos\theta\mathbf{i} + 6\sin\phi\sin\theta\mathbf{j} +6\cos\theta\mathbf{k},0\le\theta\le2\pi,\dfrac{6}{\pi}\le\phi\le\dfrac{2}{3}\pi$
#### Conservative Fields
Which of the fields in Exercises 29–32 are conservative, and which are not?

29. $\mathbf{F} = x\mathbf{i} + y\mathbf{j} +z\mathbf{k}$  
    $\dfrac{\partial P}{\partial y} = \dfrac{\partial N}{\partial z} = 0$  
    $\dfrac{\partial P}{\partial X} = \dfrac{\partial M}{\partial z} = 0$  
    $\dfrac{\partial N}{\partial x} = \dfrac{\partial M}{\partial y} = 0$
#### Work and Circulation
In Exercises 35 and 36, ind the work done by each field along the paths from $(0, 0, 0)$ to $(1, 1, 1)$ in Exercise 1.

35. $\mathbf{F} = 2xy\mathbf{i} + \mathbf{j} +x^2\mathbf{k}$    
    p1: $W = \int_0^13t^2 + 1dt=2$  
    p2: $W =\int_0^12t^2+1dt+\int_0^1dt = \dfrac{8}{3}$  
#### Masses and Moments
41. Wire with different densities Find the mass of a thin wire lying along the curve $\mathbf{r}(t) = \sqrt{2}\mathbf{i} + \sqrt{2}\mathbf{j} +(4-t^2)\mathbf{k},0\le t\le1$ if the density at $t$ is (a) $\delta = 3t$ and (b) $\delta = 1.$   
   a. $M = \int_0^13t\sqrt{\dfrac{1+t^2}{t}}dt$  
   b. $M = \int_0^1\sqrt{\dfrac{1+t^2}{t}}dt$
#### Flux Across a Plane Curve or Surface
Use Green’s Theorem to find the counterclockwise circulation and outward flux for the fields and curves in Exercises 49 and 50.

49. Square $\mathbf{F} = (2xy+x)\mathbf{i} + (xy-y\mathbf{j}$  
C: The square bounded by $x = 0, x = 1, y = 0, y = 1$    
flux :$\int_0^1\int_0^1(2y+1+x-1)dxdy=\dfrac{3}{2}$  
circulation $\int_0^1\int_0^1(2y-x)dxdy=-\dfrac{1}{2}$
###  Additional and Advanced Exercises
#### Finding Areas with Green’s Theorem
Use the Green’s Theorem area formula in Exercises 16.4 to find the areas of the regions enclosed by the curves in Exercises 1–4.
1. The limaçon $x = 2 \cos t - \cos 2t, y = 2 \sin t, 0\le t \le 2\pi$  
   ![](../images/Thomas%20Calculus/16-5.jpg)  
   $dx =-2\sin t +2\sin 2t,dy = 2\cos t$  
   $A = \int_0^{2\pi}xdy-ydx=6\pi$
#### Theory and Applications
5. a. Give an example of a vector field $\mathbf{F} (x, y, z)$ that has value 0 at only one point and such that curl $\mathbf{F}$ is nonzero everywhere. Be sure to identify the point and compute the curl.  
b. Give an example of a vector field $\mathbf{F} (x, y, z)$ that has value 0 on precisely one line and such that curl $\mathbf{F}$ is nonzero everywhere. Be sure to identify the line and compute the curl.  
c. Give an example of a vector field $\mathbf{F} (x, y, z)$ that has value 0 on a surface and such that curl $\mathbf{F}$ is nonzero everywhere. Be sure to identify the surface and compute the curl.  
a. $\mathbf{F} = z\mathbf{i} + x\mathbf{j}+y\mathbf{k},(0,0,0)$  
b. $\mathbf{F} = z\mathbf{i} + y\mathbf{k},x=t,y=0,z=0$  
c. $\mathbf{F} = z\mathbf{i}z=0$