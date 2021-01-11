# Thomas Calculus
## Chapter 7 Transcendental Functions
### 7.1 Inverse Functions and Their Derivatives
#### Identifying One-to-One Functions Graphically
Which of the functions graphed in Exercises 1–6 are one-to-one, and which are not?
1. ![](../images/Thomas%20Calculus/7-5.jpg)   
   One to one
#### Graphing Inverse Functions
Each of Exercises 11–16 shows the graph of a function $y = f(x).$ Copy the graph and draw in the line $y = x$. Then use symmetry with respect to the line $y = x$ to add the graph of $f^{-1}$ to your sketch. (It is not necessary to find a formula for $f^{-1}$) Identify the domain and range of $f^{-1}$

11. ![](../images/Thomas%20Calculus/7-6.jpg)
    D: $(0,1]$R:$[0,\infty)$
#### Formulas for Inverse Functions
Each of Exercises 19–24 gives a formula for a function $y = f(x)$ and shows the graphs of $f$ and $f^{-1}$ . Find a formula for $f^{-1}$ in each case.

19. $f(x) = x^2 + 1, x \ge 0$  
    ![](../images/Thomas%20Calculus/7-7.jpg)   
    $x^2 = y - 1$  
    $x\ge 0, x = \sqrt{y - 1}$  
    $f^{-1}(x) = \sqrt{x - 1}, x\ge 1$
#### Derivatives of Inverse Functions
Each of Exercises 25–34 gives a formula for a function $y = f(x)$. In each case, find $f^{-1}(x)$ and identify the domain and range of $f^{-1}$. As a check, show that $f(f^{-1}(x)) = f^{-1}(f(x)) = x$

25. $f(x) = x^5$  
    $f^{-1}(x) = \sqrt[5]{x}$  
    $f(f^{-1}(x)) = (\sqrt[5]{x})^5 = x$  
    $f^{-1}(f(x)) = \sqrt[5]{x^5}= x$
#### Inverses of Lines
45. a. Find the inverse of the function $f(x) = mx$, where $m$ is a constant different from zero.  
b. What can you conclude about the inverse of a function $y = f(x)$ whose graph is a line through the origin with a nonzero slope $m$?  
a. $f^{-1}(x) = \dfrac{1}{m}x$
#### Increasing and Decreasing Functions
49. Show that increasing functions and decreasing functions are one-to-one. That is, show that for any $x_1$ and $x_2$ in $I, x_2 \le x_1$ implies $f(x_2) \ne f(x_1).$  
    If for some $x_1$ and $x_2$ in $I, x_2 \le x_1$ implies $f(x_2) = f(x_1),$ the function is neither decreasing nor increasing in $I$
#### Theory and Applications
55. If $f(x)$ is one-to-one, can anything be said about $g(x) = -f(x)$? Is it also one-to-one? Give reasons for your answer
    It is also one-to-one
#### COMPUTER EXPLORATIONS
In Exercises 61–66, you will explore some functions and their inverses together with their derivatives and linear approximating functions at specified points. Perform the following steps using your CAS:  
a. Plot the function $y = f(x)$  together with its derivative over the given interval. Explain why you know that $f$ is one-to-one over the interval.   
b. Solve the equation $y = f(x)$ for $x$ as a function of $y$, and name the resulting inverse function $g$.  
c. Find the equation for the tangent line to $f$ at the specified point $(x0, f(x_0)).$  
d. Find the equation for the tangent line to $g$ at the point $(f(x_0), x_0)$ located symmetrically across the 45° line $y = x$ (which is the graph of the identity function). Use Theorem 1 to find the slope of this tangent line.  
e. Plot the functions $f$ and $g$, the identity, the two tangent lines, and the line segment joining the points $(x0, f(x_0)).$ and $(f(x_0), x_0)$ Discuss the symmetries you see across the main diagonal.

61. $y = \sqrt{3x - 2},\dfrac{2}{3} \le x \le 4, x_0 = 3$  
    a. $\dfrac{dy}{dx} = \dfrac{1}{2\sqrt{3x-2}}\cdot3 = \dfrac{3}{2\sqrt{3x-2}}$  
    b. $3x - 2=y^2$  
    $x = \dfrac{y^2+2}{3}$  
    $g(x) = \dfrac{x^2+2}{3}$  
    c. $f(3) = \sqrt{7}$   
    $f'(3) = \dfrac{3}{2\sqrt{7}} = \dfrac{3}{14}\sqrt{7}$  
    $y = \dfrac{3}{14}\sqrt{7}x+\dfrac{5}{14}\sqrt{7}$  
    d. $g'(\sqrt{7}) = \dfrac{1}{f'(g(\sqrt{7}))} = \dfrac{2}{3}\sqrt{7}$   
    $y = \dfrac{2}{3}\sqrt{7}x-\dfrac{5}{3}$
