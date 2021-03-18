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