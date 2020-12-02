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
### 3.2 The Derivative as a Function
#### Finding Derivative Functions and Values
Using the definition, calculate the derivatives of the functions in Exercises 1–6. Then find the values of the derivatives as specified.
1. $f(x) = 4 - x^2; f'(-3), f'(0), f'(1)$
   $f'(x) = -2x, f'(-3) = 6, f'(0) = 0, f'(1) = -2$
#### Slopes and Tangent Lines
In Exercises 13–16, differentiate the functions and find the slope of the tangent line at the given value of the independent variable.

13. $f(x) = x + \dfrac{9}{x}, x = -3$  
    $f'(x) = 1 - \dfrac{9}{x^2},k = f'(-3) = 0$
#### Using the Alternative Formula for Derivatives
Use the formula
$$
f'(x) = \lim_{z\to x}\dfrac{f(z) - f(x)}{z - x}
$$
to find the derivative of the functions in Exercises 23–26.

23. $f(x) = \dfrac{1}{x + 2}$  
    $f'(x) = \lim\limits_{z\to x}\dfrac{\frac{1}{z + 2} - \frac{1}{x + 2}}{z - x}$  
    $= \lim\limits_{z\to x}\dfrac{\frac{z + 2 - x -2}{(z + 2)(x + 2)}}{z - x}$  
    $= \lim\limits_{z\to x}\dfrac{1}{(z + 2)(x + 2)} = \dfrac{1}{x^2 + 4x + 4}$ 
#### Graphs
Match the functions graphed in Exercises 27–30 with the derivatives graphed in the accompanying figures (a)–(d).   
![](../images/Thomas%20Calculus/3-6.jpg)   

27.         
    ![](../images/Thomas%20Calculus/3-7.jpg)     
    (b)
#### One-Sided Derivatives
Compute the right-hand and left-hand derivatives as limits to show that the functions in Exercises 37–40 are not differentiable at the point $P$.

37.        
    ![](../images/Thomas%20Calculus/3-8.jpg)  
    $\lim\limits_{h\to0^+}\dfrac{f(0 + h) - f(0)}{h} =1$   
    $\lim\limits_{h\to0^+}\dfrac{f(x_0 + h) - ƒ(x_0)}{h} = \lim\limits_{h\to0^+}h = 0$   
    Therefore, the function is not differentiable at $P(0,0)$
#### Differentiability and Continuity on an Interval
Each figure in Exercises 45–50 shows the graph of a function over a closed interval $D$. At what domain points does the function appear
to be  
a. differentiable?  
b. continuous but not differentiable?  
c. neither continuous nor differentiable?   
Give reasons for your answers.  

45. ![](../images/Thomas%20Calculus/39.jpg)   
    The function is differentiable over $D$ because it is differentiable at every point in $(-3,2)$ and the right hand derivative at $x = -3$ and the left hand derivative $x = 2$ exists.
#### Theory and Examples
In Exercises 51–54,  
a. Find the derivative $f'(x)$ of the given function $y = f(x)$.  
b. Graph $y = f(x)$ and $y = f'(x)$ side by side using separate sets of coordinate axes, and answer the following questions.  
c. For what values of $x$, if any, is $f'$ positive? Zero? Negative?  
d. Over what intervals of $x$-values, if any, does the function $y = f(x)$ increase as $x$ increases? Decrease as $x$ increases?How is this related to what you found in part (c)? (We will say more about this relationship in Section 4.3.)

51. $y = -x^2$   
    a. $f'(x) = -2x$  
    b. $f'(x)$ is negative when $x < 0$, zero when $x = 0$, and positive at $x > 0$  
    c. $f(x)$ increases when $x > 0$ and decreases when $x < 0$. $f(x)$ increases when $f'(x) > 0$ and decreases when $f'(x) < 0$
#### COMPUTER EXPLORATIONS
Use a CAS to perform the following steps for the functions in Exercises 65–70.  
a. Plot $y = f(x)$ to see that function’s global behavior.    
b. Define the difference quotient $q$ at a general point $x$, with general step size $h$.  
c. Take the limit as $h \to 0$. What formula does this give?   
d. Substitute the value $x = x_0$ and plot the function $y = f(x)$
together with its tangent line at that point.   
e. Substitute various values for $x$ larger and smaller than $x_0$ into the formula obtained in part (c). Do the numbers make sense with your picture?  
f. Graph the formula obtained in part (c). What does it mean when its values are negative? Zero? Positive? Does this make sense with your plot from part (a)? Give reasons for your
answer.

65. $f(x) = x^3 + x^2 - x, x_0 = 1$  
    b. $q = \dfrac{f(x + h) - f(x)}{h}$  
    $= \dfrac{(x + h)^3 + (x + h)^2 -(x + h) - (x^3 + x^2 -x)}{h}$  
    $= \dfrac{x^3 + h^3 + 3x^2h + 3xh^2 + x^2 + 2xh + h^2 -x -h -x^3 -x^2 + x}{h}$  
    $= \dfrac{h^3 + 3x^2h + 3xh^2 + 2xh + h^2 - h}{h}$  
    $= 3x^2 + (3h + 2)x + h^3 + h^2 -1$  
    c. $\lim\limits_{h\to0}q = 3x^2 + 2x -1$
#### Derivative Calculations
In Exercises 1–12, find the first and second derivatives.
1. $y = -x^2 + 3$  
   $f'(x) = -2x,f''(x) = -2$
#### Slopes and Tangent Lines
41. a. Normal line to a curve. Find an equation for the line perpendicular to the tangent line to the curve $y = x^3 - 4x + 1$ at the point $(2, 1)$.  
    b. Smallest slope. What is the smallest slope on the curve? At
    what point on the curve does the curve have this slope?  
    c. Tangent lines having specified slope. Find equations for the tangent lines to the curve at the points where the slope of the curve is 8.  
    a. $f'(x) = 3x^2 -4,f'(2) =8$  
    $y = -\dfrac{1}{8}x+\dfrac{7}{4}$  
    b. $f'(x)_{\min} = f'(0) = -4$  
    c. $f'(x) = 3x^2 -4 = 8, x = \plusmn2, P_1(-2,1),P_2(2,1)$  
#### Theory and Examples
For Exercises 55 and 56 evaluate each limit by first converting each to a derivative at a particular $x$-value.

55. $\lim\limits_{x\to1}\dfrac{x^{50 }- 1}{x - 1}$  
    $f'(1) = \lim\limits_{z\to1}\dfrac{f(z) -f(1)}{z - 1}$  
    Let $f(x)=x^{50},f'(x) = 50x^{49}$  
    $\lim\limits_{x\to1}\dfrac{x^{50 }- 1}{x - 1} = f'(1) = 50$