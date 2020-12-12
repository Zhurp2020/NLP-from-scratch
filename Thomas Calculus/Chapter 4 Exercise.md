# Thomas Calculus
## Chapter 4 Applications of Derivatives
### 4.1 Extreme Values of Functions on Closed Intervals
#### Finding Extrema from Graphs
In Exercises 1–6, determine from the graph whether the function has any absolute extreme values on $[a, b]$ . Then explain how your answer is consistent with Theorem 1.
1. ![](../images/Thomas%20Calculus/4-4.jpg)
   The function has a maximum value at $b$ and a minimum value at $c_2$.
#### Absolute Extrema on Finite Closed Intervals
In Exercises 21–36, find the absolute maximum and minimum values of each function on the given interval. Then graph the function. Identify the points on the graph where the absolute extrema occur, and include their coordinates.

21. $f(x) = \dfrac{2}{3}x - 5, -2 \le x \le 3$   
    $f'(x) = \dfrac{2}{3} \ne 0$  
    $f$ is continuous over the interval.   
    Therefore, the extrema occur at endpoints.    
    Minimum: $(-2,-\dfrac{19}{3})$  
    Maximum: $(3,-2)$ 
#### Finding Critical Points
In Exercises 41–50, determine all critical points for each function.

41. $y = x^2 - 6x + 7$  
    $\dfrac{dy}{dx} = 2x - 6 = 0$  
    $x = 3$  
    Critical points:$(3,-2)$
#### Local Extrema and Critical Points
In Exercises 51–58, find the critical points and domain endpoints for each function. Then find the value of the function at each of these points and identify extreme values (absolute and local).

51. $y = x^\frac{2}{3}(x + 2)$  
    Domain: $R$. The function is differentiable at every point in its domain.  
    $\dfrac{dy}{dx} = \dfrac{2}{3}x^{-\frac{1}{3}}(x + 2)+x^\frac{2}{3} = 0$  
    $\dfrac{2}{3}(x + 2) + x = 0$  
    $x = -\dfrac{2}{5}$   
    $y = \sqrt[3]{\dfrac{4}{25}}(-\dfrac{2}{5}+2) = \dfrac{8}{5}\sqrt[3]{\dfrac{4}{25}}$  
    Critical point:$(-\dfrac{2}{5},\dfrac{8}{5}\sqrt[3]{\dfrac{4}{25}})$   
    The function has no extreme values.  
#### Theory and Examples
63. A minimum with no derivative. The function $f(x) = |x|$ has an absolute minimum value at $x = 0$ even though $f$ is not diferentiable at $x = 0$. Is this consistent with Theorem 2? Give reasons for your answer.  
    Yes. $(0,0)$ is a critical point of the function. 
#### COMPUTER EXPLORATIONS
In Exercises 75–80, you will use a CAS to help find the absolute extrema of the given function over the specified closed interval.     Perform the following steps.  
a. Plot the function over the interval to see its general behavior there.  
b. Find the interior points where $f' = 0$. (In some exercises, you may have to use the numerical equation solver to approximate a solution.) You may want to plot $f'$ as well.  
c. Find the interior points where $f'$ does not exist.   
d. Evaluate the function at all points found in parts (b) and (c) and at the endpoints of the interval.   
e. Find the function’s absolute extreme values on the interval and identify where they occur.

75. $f(x) = x^4 - 8x^2 + 4x + 2,[-\dfrac{4}{5},\dfrac{64}{25}]$  
    $f'(x) = 4x^3 - 16x + 4 = 0$  
    $x_1 \approx -2.11,x_2 \approx 1.86, x_3 \approx 0.25$  
    $f(x_2) \approx -6.28, f(x_3) \approx 2.5, f(-\dfrac{4}{5}) \approx -5.91, f(\dfrac{64}{25}) \approx 2.76$  
    Maximum value : $f(\dfrac{64}{25}) \approx 2.76$  
    Minimum value : $f(x_2) \approx -6.28$  
#### 4.2 The Mean Value Theorem
#### Checking the Mean Value Theorem
Find the value or values of $c$ that satisfy the equation
$$
\dfrac{f(b) - f(a)}{b - a}= f'(c)
$$
in the conclusion of the Mean Value Theorem for the functions and intervals in Exercises 1–6.
1. $f(x) = x^2 + 2x - 1, [0, 1]$   
   $f'(x) = 2x + 2 = \dfrac{2 +1}{1}$  
   $wx = 1, x = \dfrac{1}{2}$
#### Roots (Zeros)
15. a. Plot the zeros of each polynomial on a line together with the zeros of its first derivative.  
 i) $y = x^2 - 4$  
 ii) $y = x^2 + 8x + 15$    
 iii) $y = x^3 - 3x^2 + 4 = (x + 1)(x - 2)^2$   
 iv) $y = x^3 - 33x^2 + 216x = x(x - 9)(x - 24)$    
b. Use Rolle’s Theorem to prove that between every two zeros of $x^n + a_{n-1}x^{n-1}+ \cdots + a_1x + a_0$ there lies a zero of
    $$
    nx^{n-1} + (n - 1)^a_{n-1}x^{n-2} + \cdots + a_1
    $$
    a. i)$y' = 2x$  
    ii) $y' = 2x + 8$  
    III)$y' = 3x^2- 6x$   
    iv) $y' = 3x^2 - 66x + 216$  
    b. Let $f(x) = x^n + a_{n-1}x^{n-1}+ \cdots + a_1x + a_0$   
    $f'(x) = nx^{n-1} + (n - 1)^a_{n-1}x^{n-2} + \cdots + a_1$  
    For any two zeros of $f(x), a, b$:  
    $f$ is continuous over $[a,b]$ and differentiable at every point in $(a,b)$   
    $f(a) = f(b) = 0$  
    The Rolle's Theorem gives that there is a point $c\in(a,b)$ such that $f'(c) = 0$  
    Therefore, there lies a zero of$nx^{n-1} + (n - 1)^a_{n-1}x^{n-2} + \cdots + a_1$
#### Finding Functions from Derivatives
27. Suppose that $f(-1) = 3$ and that $f'(x) = 0$ for all $x$. Must $f(x) = 3$ for all $x$? Give reasons for your answer.   
    Yes. $f'(x) = 0$ for all $x$ means that $f$ is a constant value function. Since $f(-1) = 3$, $f(x) = 3$ for all $x$.
#### Finding Position from Velocity or Acceleration
Exercises 41–44 give the velocity $y = \dfrac{ds}{dt}$ and initial position of an object moving along a coordinate line. Find the object’s position at time $t$.

41.  $y = 9.8t + 5, s(0) = 10$  
     $y = \dfrac{ds}{dt}= 9.8t + 5$  
     $s = 4.9t^2 + 5t + c$   
     $s(0) = c = 10, s(t) = 4.9t^2 + 5t + 10$   
#### Applications
49. Temperature change. It took 14 sec for a mercury thermometer to rise from -19°C to 100°C when it was taken from a freezer and placed in boiling water. Show that somewhere along the way the mercury was rising at the rate of 8.5°C/sec.     
    The temperature $T = f(t)$ is continuous and differentiable over $[a,a+14]$. The mean value theorem gives that there must be a point $t$ such that   
    $f'(t) = \dfrac{100-9}{14} =  8.5$  
    and the mercury was rising at the rate of 8.5°C/sec.
#### Theory and Examples
55. The geometric mean of $a$ and $b$. The geometric mean of two positive numbers $a$ and $b$ is the number $\sqrt{ab}$. Show that the value of $c$ in the conclusion of the Mean Value Theorem for $f(x) = \dfrac{1}{x}$ on an interval of positive numbers $[a, b]$ is $c = \sqrt{ab}$.  
    $\dfrac{f(b)-f(a)}{b-a} = f'(c)$  
    $\dfrac{\frac{1}{b}-\frac{1}{a}}{b - a} = -c^{-2}$    
    $\dfrac{\frac{a - b}{ab}}{b - a}  = -\dfrac{1}{c^2}$  
    $\dfrac{1}{ab} = \dfrac{1}{c^2}$  
    $c = \plusmn\sqrt{ab}$  
    Since $0<a<c<b, c = \sqrt{ab}$
### 4.3 Monotonic Functions and the First Derivative Test
#### Analyzing Functions from Derivatives
Answer the following questions about the functions whose derivatives are given in Exercises 1–14:  
a. What are the critical points of $f$?  
b. On what open intervals is $f$ increasing or decreasing?  
c. At what points, if any, does $f$ assume local maximum and minimum values?
1. $f'(x) = x(x - 1)$  
   a. $x(x-1) = 0, x_1 = 0, x_2 = 1$  
   Critical points:$(0,f(0)),(1,f(1)$  
   b. $x(x-1) > 0, x<0$ or $x > 1$   
   Increasing: $(-\infty,0)$ and $(0,\infty)$  
   Decreasing: $(0,1)$  
#### dentifying Extrema
In Exercises 15–40:  
a. Find the open intervals on which the function is increasing and decreasing.   
b. Identify the function’s local and absolute extreme values, if any, saying where they occur.

15. ![](../images/Thomas%20Calculus/4-5.jpg)  
    a. Increasing: $(-2,0)$ and $(2,\infty)$  
    Decreasing: $(-\infty,-2)$ and $(0,2)$   
    b. Local minimum:$x = -2$  
    Local maximum: $x = 0$  
    Absolute minimum: $x = 2$   
#### Theory and Examples
Show that the functions in Exercises 63 and 64 have local extreme values at the given values of $\theta$, and say which kind of local extreme the function has.

63. $h(u) = 3\cos\dfrac{\theta}{2},0\le \theta \le 2\pi$ at $\theta = 0$ and $\theta = 2\pi$  
    $h'(\theta) = 3\sin\dfrac{\theta}{2}\cdot\dfrac{1}{2}= \dfrac{3}{2}\sin\dfrac{\theta}{2}$  
    $h'(0) = 0, h'(2\pi) = 0$  
    When $0< \theta < 2\pi:$  
    $0< \sin\dfrac{\theta}{2} \le 1:$  
    $h'(\theta) > 0$  
    Therefore, $h(\theta)$ have local minimum at $\theta = 0$ and $\theta = 2\pi$
### 4.4 Concavity and Curve Sketching
#### Analyzing Functions from Graphs
Identify the inflection points and local maxima and minima of the functions graphed in Exercises 1–8. Identify the intervals on which the functions are concave up and concave down.
1. $y = \dfrac{x^3}{3}-\dfrac{x^2}{2}-2x + \dfrac{1}{3}$    
   ![](../images/Thomas%20Calculus/4-6.jpg)  
   $y' = x^2 - x -2 = 0, x_1 = 2, x_2 = -1$  
   $y'' = 2x -1 = 0, x = \dfrac{1}{2}$   
   Inflection point: $(\dfrac{1}{2},-\dfrac{3}{4})$   
   Local maxima: $f(-1) = \dfrac{3}{2}$   
   Local minima: $f(2) = -3$  
   Concave up: $(\dfrac{1}{2},\infty)$  
   Concave down: $(-\infty,\dfrac{1}{2})$
#### Graphing Functions
In Exercises 9–50, identify the coordinates of any local and absolute extreme points and inflection points. Graph the function.

9. $y = x^2 - 4x + 3$  
   $y' = 2x - 4 = 0, x = 2$  
   $y'' = 2 > 0$   
   Absolute minimum: $f(2) = -1$  
   There is no inflection point. 
#### Sketching the General Shape, Knowing $y'$
Each of Exercises 51–72 gives the first derivative of a continuous function $y = f(x)$. Find $y''$ and then use Steps 2–4 of the graphing procedure on page 207 to sketch the general shape of the graph of $f$.

51. $y' = 2 + x - x^2$  
    $y'' = -2x + 1$  
    $y' = 2 + x - x^2 = 0$  
    $x^2 -x - 2 = 0, x_1 = 2, x_2 = -1$   
    Critical points are at $x = 2$ and $x = -1$  
    When $x<-1$ or $x > 2,y'>0,f$  increases.  
    When $-1<x<2, y'<0, f$ decreases. 
#### Sketching $y$ from Graphs of $y'$ and $y''$
Each of Exercises 73–76 shows the graphs of the first and second derivatives of a function $y = f(x)$. Copy the picture and add to it a sketch of the approximate graph of $ƒ$, given that the graph passes through the point $P$.  

73. ![](../images/Thomas%20Calculus/4-7.jpg)  
#### Graphing Rational Functions
Graph the rational functions in Exercises 77–94 using all the steps in the graphing procedure on page 207.

77. $y = \dfrac{2x^2 + x -1}{x^2 -1}$  
    Domain: $(-\infty-1)\cup(-1,1)\cup(1,\infty)(-\infty-1)\cup(-1,1)\cup(1,\infty)$   
    The function is neither an even one nor an odd one.  
    $y = \dfrac{(2x - 1)(x + 1)}{(x + 1)(x - 1)} = \dfrac{2x - 1}{x - 1}$   
    $y' = \dfrac{2(x - 1)-(2x-1)}{x^2 - 2x + 1}$  
    $= -\dfrac{1}{x^2 - 2x + 1}$   
    $y'' = -\dfrac{0 - (2x - 2)}{(x^2 - 2x + 1)^2}$   
    $= \dfrac{2(x- 1)}{(x - 1)^4}$  
    $= \dfrac{2}{(x - 1)^3}$  
    $y' < 0$ for all $x,y'$ has no critical point.  
    $y$ decreases over $(-\infty-1)$ and $(-1,1)$ and $(1,\infty)$   
    $y'' > 0$ for $x >1, y'' < 0$ for $x < 1$ and $x \ne -1,y$ has no inflection point.   
    $y$ concaves up when $x > 1$ and concaves down when  $x < 1$ and $x \ne -1$  
    $\lim\limits_{x\to\infty}y = 2$  and $\lim\limits_{x\to1}y$ does not exist. Asymptotes: $x = 1, y = 2$
#### Theory and Examples
95. The accompanying figure shows a portion of the graph of a twicedifferentiable function $y = f(x)$. At each of the five labeled points, classify $y'$ and $y'$ as positive, negative, or zero.   
    ![](../images/Thomas%20Calculus/4-8.jpg)  
    $P, y' < 0, y'' > 0$    
    $Q, y' > 0, y'' > 0$    
    $R, y' > 0, y'' = 0$   
    $S, y' = 0, y'' < 0$   
    $T, y' < 0, y'' < 0$ 
#### COMPUTER EXPLORATIONS
In Exercises 121–126, find the inflection points (if any) on the graph of the function and the coordinates of the points on the graph where the function has a local maximum or local minimum value. Then graph the function in a region large enough to show all these points simultaneously. Add to your picture the graphs of the function’s first and second derivatives. How are the values at which these graphs intersect the $x$-axis related to the graph of the function? In what other ways are the graphs of the derivatives related to the graph of the function?

121. $y = x^5 - 5x^4 - 240$  
     $y' = 5x^4 - 20x^3 = 0$  
     $x^3(x-4) = 0, x_1 = 0, x_2 = 4$   
     Local maximum: $(0,-240)$  
     Local minimum: $(4,-496)$  
     $y'' = 20x^3 - 60x^2 = 0$  
     $x^2(x - 3) = 0, x_1 =0, x_2 = 3$  
     Inflection points$(0,-240),(3,-402)$
### 4.5 Applied Optimization
#### Mathematical Applications
Whenever you are maximizing or minimizing a function of a single variable, we urge you to graph it over the domain that is appropriate to the problem you are solving. The graph will provide insight before you calculate and will furnish a visual context for understanding your answer.
1. Minimizing perimeter. What is the smallest perimeter possible for a rectangle whose area is $16 in^2$ , and what are its dimensions?  
   $S = f(x) = x(16 - x) = -x^2 + 16x$  
   $f'(x) = -2x + 16 = 0 , x = 8$  
   $S_{\min} = f(8) = 64$
#### Physical Applications
41. Vertical motion. The height above ground of an object moving vertically is given by
$$
s = -16t^2 + 96t + 112,
$$
with $s$ in feet and $t$ in seconds. Find  
a. the object’s velocity when $t = 0$;  
b. its maximum height and when it occurs;  
c. its velocity when $s = 0$.   
a. $f(0) = 112$  
b. $\dfrac{ds}{dt} = -32t + 96 = 0, t = 3, s = 256$  
c. $\dfrac{ds}{dt}|_{s = 0} = 96$ 
#### Business and Economics
55. It costs you $c$ dollars each to manufacture and distribute backpacks. If the backpacks sell at $x$ dollars each, the number sold is given by
$$
n = \dfrac{a}{x - c}+ b(100 - x)
$$
where $a$ and $b$ are positive constants. What selling price will bring a maximum profit?        
$P = f(x) = (x- c)(\dfrac{a}{x - c}+ b(100 - x))$       
$= a + b(100 -x)(x -c) = -bx^2+b(100+c)x-100bc+a$  
$\dfrac{dP}{dx} = -2bx + 100b + bc = 0$  
$x = \dfrac{100 + c}{2}$   
#### Biology
63. Sensitivity to medicine (Continuation of Exercise 60, Section 3.3.) Find the amount of medicine to which the body is most sensitive by finding the value of $M$ that maximizes the derivative $\dfrac{dR}{dM}$, where
$$
R = M^2(\dfrac{C}{2} - \dfrac{M}{3})
$$
and $C$ is a constant.  
$\dfrac{dR}{dM} = -\dfrac{1}{3}M^2 + 2M(\dfrac{C}{2} - \dfrac{M}{3})$  
$= -M^2 + 2CM$   
$\dfrac{d^2R}{dM^2} = -2M + 3C = 0, M = C$
#### Theory and Examples
65. An inequality for positive integers. Show that if $a$, $b$, $c$, and $d$ are positive integers, then
$$
\dfrac{(a^2 + 1)(b^2 + 1)(c^2 + 1)(d^2 + 1)}{abcd}\ge 16.
$$   
Let $f(x) = \dfrac{x^2 + 1}{x} = x + \dfrac{1}{x}, x > 0, x \in Z$  
$f'(x) = 1 - \dfrac{1}{x^2} = 0, x = \plusmn 1, x > 0, x = 1$  
$f(x) \ge f(1) = 2$  
$\dfrac{(a^2 + 1)(b^2 + 1)(c^2 + 1)(d^2 + 1)}{abcd} \ge 2^4 = 16$
### 4.6 Newton’s Method
#### Root Finding
1. Use Newton’s method to estimate the solutions of the equation $x^2 + x - 1 = 0$. Start with $x_0 = -1$ for the left-hand solution and with $x_0 = 1$ for the solution on the right. Then, in each case, find $x_2$.    
   Let $f(x) = x^2 + x - 1$  
   $f'(x) = 2x + 1$  
   $x_1 = -2, x_2 = -\dfrac{5}{3}$
#### Dependence on Initial Point
8. Using the function shown in the figure, and for each initial estimate $x_0$ , determine graphically what happens to the sequence of Newton’s method approximations  
a. $x_0 = 0$ b. $x_0 = 1$  
c. $x_0 = 2$ d. $x_0 = 4$   
e. $x_0 = 5.5$  
![](../images/Thomas%20Calculus/4-9.jpg)
#### Theory and Examples
11. Oscillation. Show that if $h > 0$, applying Newton’s method to
$$
f(x) = \left\{\begin{aligned}
    \sqrt{x} &\quad,x \ge 0 \\
    \sqrt{-x}&\quad,x < 0
\end{aligned}\right.
$$
leads to $x_1 = -h$ if $x_0 = h$ and to $x_1 = h$ if $x_0 = -h$. Draw a picture that shows what is going on.     
When $x \ge 0, x_{n+1} = xn - \dfrac{\sqrt{x_n}}{\frac{1}{2\sqrt{x_n}}} = x_n -2x_n - -x_n$  
$\therefore$ if $h > 0$ leads to $x_1 = -h$ if $x_0 = h$ and to $x_1 = h$ if $x_0 = -h$