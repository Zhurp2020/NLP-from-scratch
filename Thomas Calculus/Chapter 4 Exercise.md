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