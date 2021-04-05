# Thomas Calculus
## Chapter 15 Multiple Integrals
### 15.1  Double and Iterated Integrals over Rectangles     
#### Double Integrals
#### Double Integrals as Volumes
#### Fubini’s Theorem for Calculating Double Integrals
>THEOREM 1—Fubini’s Theorem (First Form)  
If $f(x, y)$ is continuous throughout the rectangular region $R: a \le x \le b,c \le y \le d$, then  
>$$
>\iint\limits_Rf(x,y)dA = \int_c^d\int_a^bf(x,y)dxdy = \int_a^b\int_c^df(x,y)dydx
>$$
### 15.2 Double Integrals over General Regions
#### Double Integrals over Bounded, Nonrectangular Regions
#### Volumes
>THEOREM 2—Fubini’s Theorem (Stronger Form)  
Let $f(x, y)$ be continuous on a region $R$.
>1. If $R$ is defined by $a \le x \le b,g_1(x) \le y\le g_2(x)$, with $g_1$ and $g_2$ continuous on $[a, b]$ , then
>$$
>\iint\limits_Rf(x,y)dA = \int_a^b\int_{g_1(x)}^{g_2(x)}f(x,y)dydx
>$$
>2. If $R$ is defined by  $c \le y \le d,h_1(y) \le x\le h_2(y)$, with $h_1$ and $h_2$ continuous on $[a, b]$ , then
>$$
>\iint\limits_Rf(x,y)dA = \int_c^d\int_{h_1(y)}^{h_2(y)}f(x,y)dxdy 
>$$
#### Finding Limits of Integration
#### Properties of Double Integrals
### 15.3 Area by Double Integration
#### Areas of Bounded Regions in the Plane
>DEFINITION   
The area of a closed, bounded plane region $R$ is
>$$
>A = \iint\limits_RdA
>$$
#### Average Value
### 15.4 Double Integrals in Polar Form
#### Integrals in Polar Coordinates
#### Finding Limits of Integration
>Area in Polar Coordinates
The area of a closed and bounded region $R$ in the polar coordinate plane is
>$$
>A = \iint\limits_Rrdrd\theta
>$$
#### Changing Cartesian Integrals into Polar Integrals
$$
\iint\limits_Rf(x,y)dxdy = \iint\limits_Rf(r\cos\theta,r\sin\theta)rdrd\theta
$$
### 15.5 Triple Integrals in Rectangular Coordinates
#### Triple Integrals
#### Volume of a Region in Space
>DEFINITION   
The volume of a closed, bounded region $D$ in space is
>$$
>V = \iiint\limits_DdV
>$$
#### Finding Limits of Integration in the Order $dz, dy, dx$
#### Average Value of a Function in Space
$$
\dfrac{1}{V}\iiint\limits_DF(x,y,z)dV
$$
#### Properties of Triple Integrals
### 15.6 Applications
#### Masses and First Moments
#### Moments of Inertia
#### Probability
>DEFINITION 
A joint probability density function $f$ is a function that satisfies three conditions:
>1. $f(x, y) \ge 0$
>2. $\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}f(x, y) dx dy = 1$
>3. $P((X, Y)\in R) = \iint\limits_Rf(x, y) dx dy$
#### Means and Expected Values
### 15.7 Triple Integrals in Cylindrical and Spherical Coordinates
#### Integration in Cylindrical Coordinates
>DEFINITION cylindrical coordinates represent a point $P$ in space by ordered triples $(r, \theta, z)$ in which $r \ge 0$,
>1. $r$ and $\theta$ are polar coordinates for the vertical projection of $P$ on the $xy$-plane
>2. $z$ is the rectangular vertical coordinate.

>Equations Relating Rectangular $(x, y, z)$ and Cylindrical $(r, \theta, z)$ Coordinates  
>$$
>x = r\cos\theta, y=r\sin\theta , z = z\\
>r^2 = x^2 + y^2, \tan\theta = \dfrac{y}{x}
>$$
#### How to Integrate in Cylindrical Coordinates
#### Spherical Coordinates and Integration
>DEFINITION   
spherical coordinates represent a point $P$ in space by ordered triples $(\rho, \phi, \theta)$ in which  
>1. $\rho$ is the distance from $P$ to the origin $(\rho \ge 0)$.  
>2. $\phi$ is the angle $\overrightarrow{OP}$ makes with the positive $z$-axis $(0 \le \phi \le \pi)$.
>3. $\theta$ is the angle from cylindrical coordinates.

>Equations Relating Spherical Coordinates to Cartesian and Cylindrical Coordinates  
>$$
>r = \rho\sin\phi, x = r\cos\theta  \\
>z = \rho\cos\phi, y = r\sin\theta  \\
>\rho = \sqrt{x^2 + y^2 + z^2} = \sqrt{r^2 + z^2}
>$$
#### How to Integrate in Spherical Coordinates
### 15.8 Substitutions in Multiple Integrals
#### Substitutions in Double Integrals
>DEFINITION   
The Jacobian determinant or Jacobian of the coordinate transformation $x = g(u, v), y = h(u, v)$ is
>$$
>J(u,v) = \left |\begin{array}{cccc}
>   \dfrac{\partial x}{\partial u}&\dfrac{\partial x}{\partial v} \\    
>   \dfrac{\partial y}{\partial u}&\dfrac{\partial y}{\partial v}
>\end{array}\right | = \dfrac{\partial x}{\partial u}\dfrac{\partial y}{\partial v}-\dfrac{\partial x}{\partial v}\dfrac{\partial y}{\partial u}
>$$

> THEOREM 3—Substitution for Double Integrals  
Suppose that $f(x, y)$ is continuous over the region $R$. Let $G$ be the preimage of $R$ under the transformation $x = g(u, v), y = h(u, v)$, which is assumed to be one-to-one on the interior of $G$. If the functions $g$ and $h$ have continuous first partial derivatives within the interior of $G$, then
>$$
>\iint\limits_Rf(x,y)dxdy = \iint\limits_Gf(g(u,v),h(u,v))|\dfrac{\partial(x,y)}{\partial(u,v)}|dudv
>$$
#### Substitutions in Triple Integrals
