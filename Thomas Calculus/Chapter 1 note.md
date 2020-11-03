# Thomas Calculus
## Chapter 1 Functions
### 1.1 Functions and their graphs
#### Functions, domain and range
$$
y = f(x)
$$
> **DEFINITION** A **function** $f$ from a set $D$ to a set $Y$ is a rule that assigns a *unique* value $f(x)$ in $Y$ to each $x$ in $D$.  

**domain** The set $D$ of all possible input values is called the **domain** of the function.    
**range** The set of all output values of $f(x)$ as $x$ varies throughout $D$ is called the **range** of the function.
#### Graphs of Functions
#### Representing a Function Numerically
#### The Vertical Line Test for a Function
A function $f$ can have only one value $f(x)$ for each $x$ in its domain, so no vertical line can intersect the graph of a function more than once.
#### Piecewise-Defined Functions
**Piecewise-Defined Functions** A function is described in pieces by using different formulas on different parts of its domain.   
$$
|x|=\left\{\begin{aligned}
    x  &, & x \geq 0 \\
    -x &, & x \le  0
\end{aligned}\right.
$$  
**Greatest integer function** $\lfloor x\rfloor$ The function whose value at any number $x$ is the greatest integer less than or equal to $x$    
**Least integer function** $\lceil x\rceil$ The function whose value at any number $x$ is the smallest integer greater than or equal to $x$
#### Increasing and Decreasing Functions
> **DEFINITIONS** Let $f$ be a function defined on an interval $I$ and let $x_1$ and $x_2$ be two distinct points in $I$.
>1. If $f(x_2) > f(x_1)$ whenever $x_1 < x_2$, then $f$ is said to be **increasing** on $I$.
>2. If $f(x_2) < f(x_1)$ whenever  $x_1 < x_2$, then $f$ is said to be **decreasing** on $I$.
#### Even Functions and Odd Functions: Symmetry
>**DEFINITIONS** A function $y = f(x)$ is an   
&emsp; **even function of** $\bm{x}$ if $f(-x) = f(x)$,    
&emsp; **odd function of** $\bm{x}$ if $f(-x) = -f(x)$,    
for every $x$ in the function’s domain.
#### Common Functions
1. **Linear Functions** $f(x) = mx+b$ 
   1. **identity function** $f(x) = x$
    > **DEFINITION** Two variables $y$ and $x$ are **proportional** (to one another) if one is always a constant multiple of the other—that is, if $y = kx$ for some nonzero constant $k$.
2. **Power Functions** $f(x) = x^a$
   1. $f(x) = x^a$ with $a=n$, a positive integer
   ![](../images/Thomas%20Calculus/1-1.jpg)
   2.  $f(x) = x^a$ with $a=-1$ or $a=-2$
   ![](../images/Thomas%20Calculus/1-2.jpg)  
   3. $f(x) = x^a$ with $a=\dfrac{1}{2},\dfrac{1}{3},\dfrac{3}{2}$ and $\dfrac{2}{3}$ 
      1. **square root function** $f(x) = \sqrt{x}$   
      2. **cube root function** $g(x) = \sqrt[3]{x}$   

        ![](../images/Thomas%20Calculus/1-3.jpg)
3. **Polynomials** $f(x) = a_nx^n + a_{n-1}x^{n-1} + \dots + a_1x + a_0$  
   1. **coefficients** $a_0,a_1,a_2\dots a_n$
   2. **degree** $n$ if $a_n \ne 0$
   3. **quadratic functions** $p(x) = ax^2 + bx + c$
   4. **cubic functions** $p(x) = ax^3 + bx^2 + cx + d$
   
   ![](../images/Thomas%20Calculus/1-4.jpg)
4. **Rational Functions** $f(x) = \dfrac{p(x)}{q(x)}$, where $p$ and $q$ are polynomials
   ![](../images/Thomas%20Calculus/1-5.jpg)
5. **Algebraic Functions** Any function constructed from polynomials using algebraic operations (addition, subtraction, multiplication, division, and taking roots)
   ![](../images/Thomas%20Calculus/1-8.jpg)
6. **Trigonometric Functions** 
   ![](../images/Thomas%20Calculus/1-6.jpg)
7. **Exponential Functions** $f(x) = a^x$ where $a>0$ and $a \ne 1$ 
8. **Logarithmic Functions** $f(x) = \log_ax$, where $a > 0$ and $a \ne 1$
9.  **Transcendental Functions** not algebraic   
   ![](../images/Thomas%20Calculus/1-10.jpg)
### 1.2 Combining Functions; Shifting and Scaling Graphs
#### Sums, Differences, Products, and Quotients
If $f$ and $g$ are functions, then for $x \in (D(f)\cap D(g))$, 
$$
(f + g)(x) = f(x) + g(x)  \\
(f - g)(x) = f(x) - g(x)  \\
(fg)(x)    = f(x)g(x).         
$$  
At any point of $D(f)\cap D(g)$ at which $g(x) \ne 0$, 
$$
\dfrac{f}{g}(x) = \dfrac{f(x)}{g(x)}
$$  
If $c$ is a real number, then
$$
(cf)(x) = cf(x).
$$
#### Composite Functions
>**DEFINITION** If $f$ and $g$ are functions, the composite function $f \circ g$ (“$f$ composed with $g$”) is defined by
>$$
(f \circ g)(x) = f(g(x)).
>$$
>The domain of $f \circ g$ consists of the numbers $x$ in the domain of $g$ for which $g(x)$ lies in the domain of $f$.
#### Shifting a Graph of a Function
>**Shift Formulas**  
Vertical Shifts   
$y = f(x) + k$   
Shifts the graph of $f$ up $k$ units if $k > 0$  
Shifts it down $|k|$ units if $k < 0$
Horizontal Shifts  
$y = f(x + h)$   
Shifts the graph of ƒ left $h$ units if $h > 0$  
Shifts it right $|h|$ units if $h < 0$
#### Scaling and Reflecting a Graph of a Function
>**Vertical and Horizontal Scaling and Reflecting Formulas**    
For $c > 1$, the graph is scaled:    
$y = cf(x)$   
Stretches the graph of $f$ vertically by a factor of $c$.  
$y = \dfrac{1}{c}f(x)$    
Compresses the graph of $f$ vertically by a factor of $c$.  
$y = f(cx)$   
Compresses the graph of $f$ horizontally by a factor of $c$.  
$y = f(\dfrac{x}{c})$    
Stretches the graph of $f$ horizontally by a factor of $c$.      
For $c = −1$, the graph is reflected:  
$y = -f(x)$    
Reflects the graph of $f$ across the $x$-axis.   
$y = f(-x)$    
Reflects the graph of $f$ across the $y$-axis.
### 1.3 Trigonometric Functions
#### Angles
**radians** The number of **radians** in the central angle $A′CB′$ within a circle of radius $r$ is defined as the number of “radius units” contained in the arc $s$ subtended by that central angle.   
![](../images/Thomas%20Calculus/1-18.jpg)  
#### The Six Basic Trigonometric Functions
For an angle in standard position in a circle of radius $r$, and the point $P(x, y)$ where the angle’s terminal ray intersects the circle:  
sine: $\sin\theta = \dfrac{y}{r}$,   cosecant: $\csc\theta = \dfrac{r}{y}$  
cosine: $\cos\theta = \dfrac{x}{r}$ ,  secant: $\sec\theta = \dfrac{r}{x}$  
tangent: $\tan\theta = \dfrac{y}{x}$, cotangent: $\cot\theta = \dfrac{x}{y}$    
![](../images/Thomas%20Calculus/1-19.jpg)  
also:
$$
\tan\theta = \dfrac{\sin\theta}{\cos\theta},\cot\theta = \dfrac{1}{\tan\theta}  \\
\sec\theta = \dfrac{1}{\cos\theta},
\csc\theta = \dfrac{1}{\sin\theta}
$$
#### Periodicity and Graphs of the Trigonometric Functions  
> **DEFINITION** A function $f(x)$ is **periodic** if there is a positive number $p$ such that $f(x + p) = f(x)$ for every value of $x$. The smallest such value of $p$ is the **period** of $f$.   

![](../images/Thomas%20Calculus/1-20.jpg)
#### Trigonometric Identities
>$$
>\cos^2\theta + \sin^2\theta = 1 \\
>1 + \tan^2\theta = \sec^2\theta \\
>1 + \cot^2\theta = \csc^2\theta \\  
>$$
>**Addition Formulas** 
>$$ 
>\cos(A + B) = \cos A\cos B - \sin A\sin B \\
>\sin(A + B) = \sin A\cos B + \cos A\sin B \\
>$$
>**Double-Angle Formulas**
>$$
>\cos 2\theta = \cos^2\theta - \sin^2\theta \\
>\sin 2\theta = 2\sin\theta\cos\theta \\
>$$
>**Half-Angle Formulas**
>$$
>\cos^2\theta = \dfrac{1 + \cos 2\theta}{2} \\
>\sin^2\theta = \dfrac{1 - \cos 2\theta}{2} \\
>$$
#### The Law of Cosines
>$$
>c^2 = a^2 + b^2 - 2ab\cos\theta. 
>$$
#### Two Special Inequalities
>$$
>-|\theta| \le \sin\theta \le |\theta| \\
>-|\theta| \le 1 - \cos\theta \le |\theta|
>$$   
$\sin^2\theta + (1 - \cos\theta)^2 = AP^2 \le \theta^2$  
$\sin^2\theta \ge 0, (1 - \cos\theta) \ge 0$  
$\sin^2\theta \le \theta^2, (1 - \cos\theta) \le \theta^2$ 
![](../images/Thomas%20Calculus/1-21.jpg)  
#### Transformations of Trigonometric Graphs
$$
f(x) = A\sin(\dfrac{2\pi}{B}(x - C)) + D
$$
![](../images/Thomas%20Calculus/1-22.jpg)
### 1.4 Graphing with Software
#### Graphing Windows
#### Obtaining a Complete Graph
