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
      