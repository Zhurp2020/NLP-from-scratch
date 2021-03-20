# Thomas Calculus
## Chapter 14 Partial Derivatives
### 14.1 Functions of Several Variables
>**DEFINITIONS**   
Suppose $D$ is a set of $n$-tuples of real numbers  $(x_1, x_2, \dots, x_n).$ A real-valued function $f$ on $D$ is a rule that assigns a unique (single) real number
>$$
>w = f(x_1, x_2, \dots, x_n).
>$$
>to each element in $D$. The set $D$is the function’s domain. The set of $w$-values
taken on by $f$ is the function’s range. The symbol $w$ is the dependent variable of $f$, and $f$ is said to be a function of the $n$ independent variables $x_1$ to $x_n$. We also call the $x_j$’s the function’s input variables and call $w$ the function’s output variable.
#### Domains and Ranges
#### Functions of Two Variables
>**DEFINITIONS**   
A point $(x_0, y_0)$ in a region (set) $R$ in the $xy$-plane is an interior point of $R$ if it is the center of a disk of positive radius that lies entirely in $R$. $(x_0, y_0)$ is a boundary point of $R$ if every disk centered at $(x_0, y_0)$ contains points that lie outside of $R$ as well as points that lie in $R$. (The boundary point itself need not belong to $R$.) The interior points of a region, as a set, make up the interior of the region. The region’s boundary points make up its boundary. A region is open if it consists entirely of interior points. A region is closed if it contains all its boundary points.

>**DEFINITIONS**  
A region in the plane is bounded if it lies inside a disk of finite radius. A region is unbounded if it is not bounded.
#### Graphs, Level Curves, and Contours of Functions of Two Variables
>**DEFINITIONS**   
The set of points in the plane where a function $f(x, y)$ has a constant value $f(x, y) = c$ is called a level curve of $f$. The set of all points $(x, y, f(x, y))$ in space, for $(x, y)$ in the domain of $ƒ$, is called the graph of $f$. The graph of $f$ is also called the surface $z = f(x, y)$.
#### Functions of Three Variables
>**DEFINITION**   
The set of points $(x, y, z)$ in space where a function of three independent variables has a constant value $f(x, y, z) = c$ is called a level surface of $f$

>**DEFINITIONS**  
A point $(x_0, y_0, z_0)$ in a region $R$ in space is an interior point of $R$ if it is the center of a solid ball that lies entirely in $R$ . A point $(x_0, y_0, z_0)$ is a boundary point of $R$ if every solid ball centered at $(x_0, y_0, z_0)$ contains points that lie outside of $R$ as well as points that lie inside $R$. The interior of $R$ is the set of interior points of $R$. The boundary of $R$ is the set of boundary points of $R$.  
A region is open if it consists entirely of interior points. A region is closed if it contains its entire boundary
#### Computer Graphing
### 14.2 Limits and Continuity in Higher Dimensions
#### Limits for Functions of Two Variables
>DEFINITION   
We say that a function $f(x, y)$ approaches the limit $L$ as $(x, y)$ approaches $(x_0, y_0)$, and write
>$$
>\lim_{(x,y) \to (x_0,y_0)} f(x,y) = L
>$$
>if, for every number $e \varepsilon 0$, there exists a corresponding number $\delta > 0$ such that for all $(x, y)$ in the domain of $f$,
>$$
>|f(x,y) - L |< \varepsilon\quad\mathsf{whenever}\quad 0 < \sqrt{(x-x_0)^2 + (y-y_0)^2} < \delta
>$$
#### Continuity
>DEFINITION   
A function $f(x, y)$ is continuous at the point $(x_0, y_0)$ if
>1. $f$ is defined at $(x_0, y_0)$,
>2. $\lim\limits_{(x,y) \to (x_0,y_0)} f(x,y)$ exists,
>3. $\lim\limits_{(x,y) \to (x_0,y_0)} f(x,y) = f(x_0,y_0)$  
A function is continuous if it is continuous at every point of its domain.  

>Two-Path Test for Nonexistence of a Limit  
If a function $f(x, y)$ has different limits along two different paths in the domain of $f$ as $(x, y)$ approaches $(x0, y_0)$, then $\lim\limits_{(x,y) \to (x_0,y_0)} f(x,y)$ does not exist.
#### Functions of More Than Two Variables
#### Extreme Values of Continuous Functions on Closed, Bounded Sets
### 14.3 Partial Derivatives
#### Partial Derivatives of a Function of Two Variables
>DEFINITION   
The partial derivative of $f(x, y)$ with respect to $x$ at the point $(x_0, y_0)$ is  
>$$
>\dfrac{\partial f}{\partial x}|_{(x_0,y_0)} = \lim\limits_{h\to0} \dfrac{f(x_0 + h,y_0)-f(x_0,y_0)}{h}
>$$
>provided the limit exists

>DEFINITION     
The partial derivative of $f(x, y)$ with respect to $y$ at the point $(x_0, y_0)$ is  
>$$
>\dfrac{\partial f}{\partial y}|_{(x_0,y_0)} = \lim\limits_{h\to0} \dfrac{f(x_0 ,y_0+ h)-f(x_0,y_0)}{h}
>$$
>provided the limit exists
#### Calculations
#### Functions of More Than Two Variables
#### Partial Derivatives and Continuity
#### Second-Order Partial Derivatives
#### The Mixed Derivative Theorem
>THEOREM 2—The Mixed Derivative Theorem  
If $f(x, y)$ and its partial derivatives $f_x, f_y, ƒ_{xy}$ and $ƒyx$ are defined throughout an open region containing a point $(a, b)$ and are all continuous at $(a, b)$, then
>$$
>f_{xy}(a,b) = f_{yx}(a,b)
>$$
#### Partial Derivatives of Still Higher Order
#### Differentiability
>DEFINITION   
A function $z = f(x, y)$ is differentiable at $(x_0, y_0)$ if $f_x(x_0, y_0)$ and $f_y(x_0, y_0)$ exist and $\Delta z = f(x_0 + \Delta x, y_0 + \Delta y) - f(x_0, y_0)$ satisfies an equation of the form
>$$
>\Delta z = f_x(x_0, y_0)\Delta x + f_y(x_0, y_0)\Delta y + \varepsilon_1\Delta x + \varepsilon_2\Delta y
>$$
>in which each of $\varepsilon_1, \varepsilon_2 \to 0$ as both $\Delta x, \Delta y \to 0$. We call $f$ differentiable if it is differentiable at every point in its domain, and say that its graph is a smooth surface

>THEOREM 3—The Increment Theorem for Functions of Two Variables
Suppose that the first partial derivatives of $f(x, y)$ are defined throughout an open region $R$ containing the point $(x_0, y_0)$ and that $f_x$ and $f_y$ are continuous at $(x_0, y_0)$. Then the change $\Delta z = f(x_0 + \Delta x, y_0 + \Delta y) - f(x_0, y_0)$ in the value of $f$ that results from moving from $(x_0, y_0)$ to another point $(x_0 + \Delta x, y_0 + \Delta y)$ in $R$ satisfies an equation of the form
>$$
>\Delta z = f_x(x_0, y_0)\Delta x + f_y(x_0, y_0)\Delta y + \varepsilon_1\Delta x + \varepsilon_2\Delta y
>$$
>in which each of $\varepsilon_1, \varepsilon_2 \to 0$ as both $\Delta x, \Delta y \to 0$.

>Corollary of Theorem 3   
If the partial derivatives $f_x$ and $f_y$  of a function $f(x, y)$ are continuous throughout an open region $R$, then $f$ is differentiable at every point of $R$

>THEOREM 4—Differentiability Implies Continuity  
If a function $f(x, y)$ is differentiable at $(x_0, y_0)$, then $f$ is continuous at  $(x_0, y_0)$
### 14.4 The Chain Rule
#### Functions of Two Variables
>THEOREM 5—Chain Rule For Functions of One Independent Variable and Two Intermediate Variables  
If $w = f(x, y)$ is differentiable and if $x = x(t), y = y(t)$ are differentiable functions of t, then the composition $w = f(x(t), y(t))$ is a differentiable function of $t$ and
>$$
>\dfrac{\partial w}{\partial t} = f_{x}(x(t),y(t))x'(t) + f_y(x(t),y(t))y'(t)
>$$
>or
>$$
>\dfrac{\partial w}{\partial t} = \dfrac{\partial f}{\partial x}\dfrac{\partial x}{\partial t} + \dfrac{\partial f}{\partial y}\dfrac{\partial y}{\partial t}
>$$
#### Functions of Three Variables
>THEOREM 6—Chain Rule for Functions of One Independent Variable and Three Intermediate Variables  
If $w = f(x, y, z)$ is differentiable and $x, y,$ and $z$ are differentiable functions of $t$, then $w$ is a differentiable function of $t$ and
>$$
>\dfrac{\partial w}{\partial t} = \dfrac{\partial w}{\partial x}\dfrac{\partial x}{\partial t} + \dfrac{\partial w}{\partial y}\dfrac{\partial y}{\partial t} + \dfrac{\partial w}{\partial z}\dfrac{\partial z}{\partial t}
>$$
#### Functions Defined on Surfaces
>THEOREM 7—Chain Rule for Two Independent Variables and Three Intermediate Variables  
Suppose that $w = f(x, y, z), x = g(r, s), y = h(r, s)$, and $z = k(r, s).$ If all four functions are differentiable, then $w$ has partial derivatives with respect to $r$ and $s$, given by the formulas
>$$
>\dfrac{\partial w}{\partial r} = \dfrac{\partial w}{\partial x}\dfrac{\partial x}{\partial r} + \dfrac{\partial w}{\partial y}\dfrac{\partial y}{\partial r} + \dfrac{\partial w}{\partial z}\dfrac{\partial z}{\partial r}  \\
>\dfrac{\partial w}{\partial s} = \dfrac{\partial w}{\partial x}\dfrac{\partial x}{\partial s} + \dfrac{\partial w}{\partial y}\dfrac{\partial y}{\partial s} + \dfrac{\partial w}{\partial z}\dfrac{\partial z}{\partial s}
>$$
#### Implicit Differentiation Revisited
>THEOREM 8—A Formula for Implicit Differentiation  
Suppose that $F(x, y)$ is differentiable and that the equation $F(x, y) = 0$ defines $y$ as a differentiable function of x. Then at any point where $F_y \ne 0$  
>$$
>\dfrac{dy}{dx}= -\dfrac{F_x}{F_y}
>$$
#### Functions of Many Variables
### 14.5 Directional Derivatives and Gradient Vectors
#### Directional Derivatives in the Plane
>DEFINITION   
The derivative of $f$ at $P_0(x_0, y_0)$ in the direction of the unit vector $\mathbf{u} = u_1\mathbf{i} + u_2\mathbf{j}$ is the number
>$$
>\dfrac{dy}{ds}_{\mathbf{u},P_0}= \lim_{s\to0}\dfrac{f(x_0 + su_1,y_0+su_2)-f(x_0,y_0)}{s}
>$$
>provided the limit exists.
#### Interpretation of the Directional Derivative
#### Calculation and Gradients
>DEFINITION   
The gradient vector (or gradient) of $f(x, y)$ is the vector  
>$$
>\nabla f = \dfrac{\partial f}{\partial x}\mathbf{i} + \dfrac{\partial f}{\partial y}\mathbf{j}
>$$
>The value of the gradient vector obtained by evaluating the partial derivatives at a point $P_0(x_0, y_0)$ is written  
>$$
>\nabla f|_{P_0}\quad\mathsf{or}\quad\nabla f(x_0,y_0)
>$$

>THEOREM 9—The Directional Derivative Is a Dot Product  
If $f(x, y)$ is differentiable in an open region containing  $P_0(x_0, y_0)$, then
>$$
>\dfrac{dy}{ds}_{\mathbf{u},P_0} = \nabla f|_{P_0}\cdot\mathbf{u}
>$$
>the dot product of the gradient $\nabla f$ at $P_0$ with the vector $\mathbf{u}$. In brief, $D_uf = \nabla f\cdot \mathbf{u}$

>Properties of the Directional Derivative $D_uf = \nabla f\cdot \mathbf{u} = |\nabla f|\cos\theta$
>1. The function $f$ increases most rapidly when $\cos\theta = 1$, which means that $\theta = 0$ and $\mathbf{u}$ is the direction of $\nabla f$. That is, at each point $P$ in its domain, $f$ increases most rapidly in the direction of the gradient vector $\nabla f$ at $P$. The derivative in this direction is 
>$$
>D_uf  = |\nabla f|\cos0 = |\nabla f|
>$$
>2. Similarly, $f$ decreases most rapidly in the direction of $-\nabla f$. The derivative in this direction is $D_uf  = |\nabla f|\cos(-\pi) = -|\nabla f|$.
>3. Any direction $\mathbf{u}$  orthogonal to a gradient $\nabla f \ne 0$ is a direction of zero change in $f$ because $\mathbf{u}$ then equals $\dfrac{\pi}{2}$ and $D_uf  = |\nabla f|\cos(\dfrac{\pi}{2}) = 0$.
#### Gradients and Tangents to Level Curves
>Tangent Line to a Level Curve
>$$
>f_x(x_0,y_0)(x-x_0) + f_y(x_0,y_0)(y-y_0) = 0
>$$
#### Functions of Three Variables
#### The Chain Rule for Paths
>The Derivative Along a Path
>$$
>\dfrac{d}{dt}f(\mathbf{r}(t)) = \nabla f(\mathbf{r}(t))\mathbf{r}'(t)
>$$