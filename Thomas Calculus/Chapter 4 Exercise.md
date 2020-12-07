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