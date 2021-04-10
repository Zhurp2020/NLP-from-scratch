# Thomas Calculus
## Chapter 16 Integrals and Vector Fields
### 16.1 Line Integrals of Scalar Functions
>DEFINITION   
If $f$ is defined on a curve $C$ given parametrically by $\mathbf{r}(t) =g(t)\mathbf{i} + h(t)\mathbf{j} + k(t)\mathbf{k}, a \le t \le b$, then the line integral of $f$ over $C$ is  
>$$
>\int_Cf(x,y,z)ds = \lim_{n\to\infty}\sum_{k=1}^nf(x_k,y_k,z_k)\Delta k
>$$
#### Additivity
#### Mass and Moment Calculations
#### Line Integrals in the Plan
### 16.2 Vector Fields and Line Integrals: Work, Circulation, and Flux
#### Vector Fields
#### Gradient Fields
#### Line Integrals of Vector Fields
>DEFINITION  
Let $\mathbf{F}$ be a vector field with continuous components defined along a smooth curve $C$ parametrized by $\mathbf{r}(t), a \le t \le b.$ Then the line integral of $\mathbf{F}$ along $C$ is
>$$
>\int_C\mathbf{F}\cdot \mathbf{T}ds =\int_C\mathbf{F}\cdot\dfrac{d\mathbf{r}}{ds} ds = \int_C\mathbf{F}\cdot d\mathbf{r} = \int_a^b\mathbf{F}(\mathbf{r}(t))\cdot \dfrac{d\mathbf{r}}{dt}dt
>$$
#### Line Integrals with Respect to $dx, dy,$ or $dz$
#### Work Done by a Force over a Curve in Space
>DEFINITION   
Let $C$ be a smooth curve parametrized by $\mathbf{r}(t), a \le t \le b.$, and let $\mathbf{F}$ be a continuous force field over a region containing $C$. Then the work done in moving an object from the point $A = \mathbf{r}(a)$ to the point $B = \mathbf{r}(b)$ along $C$ is
>$$
>W = \int_C\mathbf{F}\cdot \mathbf{T}ds = \int_a^b\mathbf{F}(\mathbf{r}(t))\cdot \dfrac{d\mathbf{r}}{dt}dt
>$$
#### Flow Integrals and Circulation for Velocity Fields
>DEFINITION  
If $\mathbf{r}(t)$ parametrizes a smooth curve $C$ in the domain of a continuous velocity field $\mathbf{F}$, the flow along the curve from $A = \mathbf{r}(a)$ to $B = \mathbf{r}(b)$ is
>$$
>\int_C\mathbf{F}\cdot \mathbf{T}ds
>$$
>The integral is called a flow integral. If the curve starts and ends at the same point, so that $A = B$, the flow is called the circulation around the curve.
#### Flux Across a Simple Closed Plane Curve
>DEFINITION   
If $C$ is a smooth simple closed curve in the domain of a continuous vector field $\mathbf{F} = M(x, y)\mathbf{i} + N(x, y)\mathbf{j}$ in the plane, and if $\mathbf{n}$ is the outward pointing unit normal vector on $C$, the flux of $\mathbf{F}$ across $C$ is
>$$
>\int_C\mathbf{F}\cdot \mathbf{n}ds
>$$

>Calculating Flux Across a Smooth Closed Plane Curve  
Flux of $\mathbf{F} = M\mathbf{i} + N\mathbf{j}$ across $C$  
>$$
>\oint_CMdy-Ndx
>$$
### 16.3 Path Independence, Conservative Fields, and Potential Functions
#### Path Independence
>DEFINITIONS   
Let $\mathbf{F}$ be a vector field defined on an open region D in space, and suppose that for any two points $A$ and $B$ in $D$ the line integral $\int_C\mathbf{F}\cdot d\mathbf{r}$ along a path $C$ from $A$ to $B$ in $D$ is the same over all paths from $A$ to $B$. Then the integral $\int_C\mathbf{F}\cdot d\mathbf{r}$ is path independent in $D$ and the field $\mathbf{F}$ is conservative on $D$.

>DEFINITION  
If $\mathbf{F}$ is a vector field defined on $D$ and $\mathbf{F}= \nabla f$ for some scalar function $f$ on $D$, then $f$ is called a potential function for $\mathbf{F}$
#### Assumptions on Curves, Vector Fields, and Domains
#### Line Integrals in Conservative Fields
>THEOREM 1—Fundamental Theorem of Line Integrals  
Let $C$ be a smooth curve joining the point $A$ to the point $B$ in the plane or in space and parametrized by $\mathbf{r}(t)$. Let $f$ be a differentiable function with a continuous gradient vector $\mathbf{F}= \nabla f$ on a domain $D$ containing $C$. Then
>$$
>\int_C\mathbf{F}\cdot d\mathbf{r} = f(B)-f(A)
>$$

>THEOREM 2—Conservative Fields are Gradient Fields  
Let $\mathbf{F} = M\mathbf{i} + N\mathbf{j} + P\mathbf{k}$ be a vector field whose components are continuous throughout an open connected region $D$ in space. Then $\mathbf{F}$ is conservative if and only if $\mathbf{F}$ is a gradient field $\nabla f$ for a differentiable function $f$.

>THEOREM 3—Loop Property of Conservative Fields  
The following statements are equivalent.
>1. $\oint_C\mathbf{F}\cdot d\mathbf{r} = 0$ around every loop (that is, closed curve $C$ ) in $D$.
>2. The field $\mathbf{F}$ is conservative on $D$.
#### Finding Potentials for Conservative Fields
>Component Test for Conservative Fields  
Let $\mathbf{F} = M(x,y,z)\mathbf{i} + N(x,y,z)\mathbf{j} + P(x,y,z)\mathbf{k}$ be a field on an open simply connected domain whose component functions have continuous first partial derivatives. Then, $\mathbf{F}$ is conservative if and only if  
>$$
>\dfrac{\partial P}{\partial y} = \dfrac{\partial N}{\partial z},\dfrac{\partial M}{\partial z} = \dfrac{\partial P}{\partial x},\dfrac{\partial N}{\partial x} = \dfrac{\partial M}{\partial y}
>$$
#### Exact Differential Forms
>DEFINITIONS   
Any expression $M(x, y, z) dx + N(x, y, z) dy + P(x, y, z) dz$ is a differential form. A differential form is exact on a domain $D$ in space if
>$$
>Mdx + Ndy + Pdz=\dfrac{\partial F}{\partial x}dx + \dfrac{\partial f}{\partial y}dy + \dfrac{\partial f}{\partial z}dz =df
>$$
>for some scalar function $f$ throughout $D$

>Component Test for Exactness of $M dx + N dy + P dz$  
The differential form $M dx + N dy + P dz$ is exact on an open simply connected domain if and only if
>$$
>\dfrac{\partial P}{\partial y} = \dfrac{\partial N}{\partial z},\dfrac{\partial M}{\partial z} = \dfrac{\partial P}{\partial x},\dfrac{\partial N}{\partial x} = \dfrac{\partial M}{\partial y}
>$$
>This is equivalent to saying that the field $\mathbf{F} = M\mathbf{i} + N\mathbf{j} + P\mathbf{k}$ is conservative.
### 16.4 Green’s Theorem in the Plane
#### Spin Around an Axis: The $\mathbf{k}$-Component of Curl
>DEFINITION   
The circulation density of a vector field $\mathbf{F} = M\mathbf{i} + N\mathbf{j}$ at the point $(x, y)$ is the scalar expression
>$$
>\dfrac{\partial N}{\partial x} - \dfrac{\partial M}{\partial y},
>$$     
>This expression is also called the $k$-component of the curl, denoted by $(\mathsf{curl} \mathbf{F})\cdot\mathbf{k}$.
#### Divergence
>DEFINITION 
The divergence (flux density) of a vector field $\mathbf{F} = M\mathbf{i} + N\mathbf{j}$ at  the point $(x, y)$ is
>$$
>\mathsf{div}\mathbf{F} = \dfrac{\partial M}{\partial x} + \dfrac{\partial N}{\partial y},
>$$  
#### Two Forms for Green’s Theorem
>THEOREM 4—Green’s Theorem (Circulation-Curl or Tangential Form)  
Let $C$ be a piecewise smooth, simple closed curve enclosing a region $R$ in the plane. Let $\mathbf{F} = M\mathbf{i} + N\mathbf{j}$ be a vector field with $M$ and $N$ having continuous first partial derivatives in an open region containing $R$. Then the counterclockwise circulation of $\mathbf{F}$ around $C$ equals the double integral of $(\mathsf{curl} \mathbf{F})\cdot\mathbf{k}$ over $R$.
>$$
>\oint\limits_C\mathbf{F}\cdot\mathbf{T}ds = \oint\limits_C Mdx - Ndy = \iint\limits_C(\dfrac{\partial N}{\partial x} - \dfrac{\partial M}{\partial y})dxdy
>$$

>THEOREM 5—Green’s Theorem (Flux-Divergence or Normal Form)  
Let $C$ be a piecewise smooth, simple closed curve enclosing a region $R$ in the plane. Let $\mathbf{F} = M\mathbf{i} + N\mathbf{j}$ be a vector field with $M$ and $N$ having continuous first partial derivatives in an open region containing $R$. Then the outward flux of $\mathbf{F}$ across $C$ equals the double integral of $\mathsf{div}\mathbf{F}$ over the region $R$ enclosed by $C$.
>$$
>\oint\limits_C\mathbf{F}\cdot\mathbf{n}ds = \oint\limits_C Mdy + Ndx = \iint\limits_C(\dfrac{\partial M}{\partial x} + \dfrac{\partial N}{\partial y})dxdy
>$$
#### Using Green’s Theorem to Evaluate Line Integrals
#### Proof of Green’s Theorem for Special Regions
### 16.5 Surfaces and Area
#### Parametrizations of Surfaces
#### Surface Area
>DEFINITION   
A parametrized surface $\mathbf{r}(u, v) = f(u, v)\mathbf{i} + g(u, v)\mathbf{j} + h(u, v)\mathbf{k}$ is smooth if $\mathbf{r}_u$ and $\mathbf{r}_v$ are continuous and $\mathbf{r}_u \times \mathbf{r}_v$  is never zero on the interior of the parameter domain.

>DEFINITION   
The area of the smooth surface $\mathbf{r}(u, y) = f(u, v)\mathbf{i} + g(u, v)\mathbf{j} + h(u, v)\mathbf{k},a\le u \le b, c\le v\le d$ is
>$$
>A = \iint\limits_R |\mathbf{r}_u \times \mathbf{r}_v|dA = \int_c^d\int_a^b|\mathbf{r}_u \times \mathbf{r}_v|dudv
>$$

>Surface Area Differential for a Parametrized Surface
>$$
>A = \iint\limits_Sd\sigma
>$$
#### Implicit Surfaces
>Formula for the Surface Area of an Implicit Surface  
The area of the surface $F(x, y, z) = c$ over a closed and bounded plane region $R$ is  
>$$
>A = \iint\limits_R |\dfrac{\nabla F}{\nabla F \cdot \mathbf{p}}|dA
>$$
>where $\mathbf{p} = \mathbf{i}, \mathbf{j}$, or $\mathbf{k}$ is normal to $R$ and $\nabla F \cdot \mathbf{p} \ne 0$

>Formula for the Surface Area of a Graph $z = f(x, y)$  
For a graph $z = f(x, y)$ over a region $R$ in the $xy$-plane, the surface area formula is
>$$
>A = \iint\limits_R \sqrt{f_x^2 + f_y^2 + 1}dxdy
>$$