# Thomas Calculus
## Chapter 3 Derivatives
### 3.1 Tangent Lines and the Derivative at a Point
#### Slopes and Tangent Lines
In Exercises 1–4, use the grid and a straight edge to make a rough
estimate of the slope of the curve (in $y$-units per $x$-unit) at the points $P_1$ and $P_2$.    
1.   
   ![](../images/Thomas%20Calculus/3-2.jpg)  
   $k_{P_1} = 1,k_{P_2} = 2$
#### Interpreting Derivative Values
23. Growth of yeast cells. In a controlled laboratory experiment, yeast cells are grown in an automated cell culture system that counts the number $P$ of cells present at hourly intervals. The number after $t$ hours is shown in the accompanying figure.   
![](../images/Thomas%20Calculus/3-3.jpg)   
a. Explain what is meant by the derivative $P'(5)$. What are its
units?  
b. Which is larger, $P'(2)$ or $P'(3)$? Give a reason for your answer.  
c. The quadratic curve capturing the trend of the data points (see Section 1.4) is given by $P(t) = 6.10t^2 - 9.28t + 16.43$. Find the instantaneous rate of growth when $t = 5$ hours.   
    a. The instantaneous rate or growth when $t = 5$ hours.  
    b. $P'(3)$ is larger. Because the curve is steeper at $t = 3$.  
    c. $P'(t) = 12.2t - 9.28, P'(5) = 51.72$  
#### Rates of Change
29. Object dropped from a tower. An object is dropped from the top of a 100-m-high tower. Its height above ground after $t$ sec is $100 - 4.9t^2$m. How fast is it falling 2 sec after it is dropped?  
    $h = f(t) = - 4.9t^2 + 100$  
    $f'(t) = -9.8t$  
    $v = f'(2) = -19.6 m/sec$
#### Testing for Tangent Lines
32. Does the graph of
    $$
    f(x) = \left\{\begin{aligned}
        x^2\sin(\dfrac{1}{x})&\quad x \ne 0 \\
        0&\quad x = 0
    \end{aligned}\right.
    $$
    have a tangent line at the origin? Give reasons for your answer.    
    $f'(0) = \lim\limits_{h\to 0}\dfrac{f(h) - f(0)}{h} = \lim\limits_{h\to 0}\dfrac{h^2\sin\frac{1}{h}}{h} = 0$   
    The tangent line exists.  
#### Vertical Tangent Lines
We say that a continuous curve $y = f(x)$ has a vertical tangent line at the point where $x = x_0$ if the limit of the difference quotient is $\infty$ or $-\infty$. For example, $y = x^\frac{1}{3}$ has a vertical tangent line at $x = 0$ (see accompanying figure):
$$
\lim_{h\to 0}\dfrac{f(0 + h) - f(0)}{h} = \lim\limits_{h\to 0}\dfrac{h^\frac{1}{3}}{h} = \lim\limits_{h\to 0}\dfrac{1}{h^\frac{2}{3}} = \infty
$$  
![](../images/Thomas%20Calculus/3-4.jpg)  
However, $y = x^\frac{2}{3}$ has no vertical tangent line at $x = 0$ (see next figure):
$$
\lim_{h\to 0}\dfrac{g(0 + h) - g(0)}{h} = \lim\limits_{h\to 0}\dfrac{h^\frac{2}{3}}{h} = \lim\limits_{h\to 0}\dfrac{1}{h^\frac{1}{3}} = \infty
$$  
does not exist, because the limit is $\infty$ from the right and $-\infty$ from the left.  

37. Does the graph of
    $$
    f(x) = \left\{\begin{aligned}
        -1&\quad x < 0 \\
        0&\quad x = 0 \\
        1&\quad x > 0
    \end{aligned}\right.
    $$
    have a vertical tangent line at the origin? Give reasons for your
    answer.   
    $\lim\limits_{h\to 0}\dfrac{f(0 + h) - f(0)}{h} = \lim\limits_{h\to 0}\dfrac{1}{h} = \infty$    
    It has a vertical tangent line. 
#### COMPUTER EXPLORATIONS
Use a CAS to perform the following steps for the functions in Exercises 49–52:   
a. Plot $y = f(x)$ over the interval $(x_0 - \frac{1}{2}) < x < (x_0 + 3)$.
b. Holding $x_0$ fixed, the difference quotient
$$
q(h) = \dfrac{f(x_0 + h) - f(x_0)}{h}
$$
at $x_0$ becomes a function of the step size $h$. Enter this function into your CAS workspace.    
c. Find the limit of $q$ as $h \to 0$.  
d. Define the secant lines $y = f(x_0) + q(x - x_0)$ for $h = 3, 2,$ and 1. Graph them together with $f$ and the tangent line over the interval in part (a).

49. $f(x) = x^3 + 2x, x_0 = 0$  
    c. $q(h) = \dfrac{h^3 + 2h}{h}$  
    $\lim\limits_{h\to 0}\dfrac{h^3 + 2h}{h} = \lim\limits_{h\to 0}(h^2 + 2) = 2$ 
