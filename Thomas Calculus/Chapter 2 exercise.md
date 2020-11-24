# Thomas Calculus
## Chapter 2 Limits and Continuity
### 2.1 Rates of Change and Tangent Lines to Curves
#### Average Rates of Change
In Exercises 1–6, find the average rate of change of the function over the given interval or intervals.
1. $f(x) = x^3 + 1$  
   a.$[2,3]$ b. $[-1,1]$  
   a. $\dfrac{f(3) - f(2)}{3 - 2} = 28 - 9 = 19$  
   b. $\dfrac{f(1) - f(-1)}{1 + 1} = \dfrac{2 - 0}{2} = 1$
#### Slope of a Curve at a Point
In Exercises 7–18, use the method in Example 3 to find (a) the slope of the curve at the given point $P$, and (b) an equation of the tangent line at $P$.

7. $y = x^2 - 5, P(2, -1)$  
   a. A nearby point $Q(2+h,(2+h)^2-5),h \ne 0$, the secant line slope  
   $k_0 = \dfrac{\Delta y}{\Delta x} = \dfrac{4 + 4h + h^2 -5 + 1}{h} = \dfrac{h^2+ 4h}{h} = h + 4$  
   $k_0$ approaches $4$ as $h$ approaches $0$. The tangent line slope is $4$.  
   b. $y = 4x -9$
#### Instantaneous Rates of Change
19. Speed of a car. The accompanying figure shows the time-to distance graph for a sports car accelerating from a standstill.   
    ![](../images/Thomas%20Calculus/2-6.jpg)  
    a. Estimate the slopes of secant lines $PQ_1,PQ_2,PQ_3,$ and $PQ_4$, arranging them in order in a table like the one in Figure 2.6. What are the appropriate units for these slopes?  
    b. Then estimate the car’s speed at time $t = 20 sec$.  
    a. 
    | $Q$        | slope of $PQ=\dfrac{\Delta t}{\Delta s},m/sec$ |
    | ---------- | ---------------------------------------------- |
    | $(10,220)$ | $\dfrac{430}{10}=43$                           |
    | $(14,380)$ | $\dfrac{270}{6}=45$                            |
    | $(17,480)$ | $\dfrac{170}{3}$                               |
    | $(18,550)$ | $\dfrac{100}{2}=50$                            |
    b. $v \approx k_{PQ_4} = 50 m/sec$
### 2.2 Limit of a Function and Limit Laws
#### Limits from Graphs
1. For the function $g(x)$ graphed here, find the following limits or explain why they do not exist.  
    a. $\lim\limits_{x\to 1}g(x)$ b. $\lim\limits_{x\to 2}g(x)$ c. $\lim\limits_{x\to 3}g(x)$ d. $\lim\limits_{x\to 2.5}g(x)$  
    ![](../images/Thomas%20Calculus/2-7.jpg)  
    a. The value of the function jumps.  
    b. $\lim\limits_{x\to 2}g(x) = 1$  
    c. The value of the function jumps.  
    d. $\lim\limits_{x\to 2.5}g(x) = \dfrac{1}{2}$
#### Existence of Limits
In Exercises 5 and 6, explain why the limits do not exist.

5. $\lim\limits_{x\to 0}\dfrac{x}{|x|}$  
   The function is $1$ when $x > 0$, $-1$ when $x < 0$, the value jumps near $x = 0$.  
#### Calculating Limits
Find the limits in Exercises 11–22.

11. $\lim\limits_{x\to 3}(x^2 - 13)$  
    $\lim\limits_{x\to 3}(x^2 - 13) = 9 - 13 = -4$
#### Using Limit Rules
51. Suppose  $\lim\limits_{x\to 0}f(x) = 1$ and  $\lim\limits_{x\to 0}g(x) = -5$. Name the rules in Theorem 1 that are used to accomplish steps (a), (b), and (c) of
the following calculation.    
    $\lim\limits_{x\to 0}\dfrac{2f(x) -g(x)}{(f(x) + 7)^\frac{2}{3}}$  
    $= \dfrac{\lim\limits_{x\to 0}(2f(x) -g(x))}{\lim\limits_{x\to 0}(f(x) + 7)^\frac{2}{3}}$   (a)  
    $= \dfrac{\lim\limits_{x\to 0}2f(x) -\lim\limits_{x\to 0}g(x)}{(\lim\limits_{x\to 0}f(x) + 7)^\frac{2}{3}}$  (b)   
    $= \dfrac{2\lim\limits_{x\to 0}f(x) -\lim\limits_{x\to 0}g(x)}{(\lim\limits_{x\to 0}f(x) + \lim\limits_{x\to 0}7)^\frac{2}{3}}$   (c)  
    $= \dfrac{(2)(1) - (-5)}{(1 + 7)^\frac{2}{3}} = \dfrac{7}{4}$  
    a. Quotient rule  
    b. Difference rule  
    c. Sum rule
#### Limits of Average Rates of Change
Because of their connection with secant lines, tangents, and instantaneous rates, limits of the form
$$
\lim_{h\to 0}\dfrac{f(x + h) - f(x)}{h}
$$
occur frequently in calculus. In Exercises 57–62, evaluate this limit for the given value of $x$ and function $f$.

57. $f(x) = x^2, x = 1$  
    $\lim\limits_{h\to 0}\dfrac{f(x + h) - f(x)}{h} = \lim\limits_{h\to 0}\dfrac{(1 + h)^2 - 1^2}{h} = \lim\limits_{h\to 0}\dfrac{h^2 + 2h}{h} = \lim\limits_{h\to 0}h + 2 = h$
#### Using the Sandwich Theorem
63. If $\sqrt{5 - 2x^2} \le f(x) \le \sqrt{5 - x^2}$ for $-1 \le x \le 1$, find $\lim\limits_{x\to 0}f(x)$.  
    $\lim\limits_{x\to 0}\sqrt{5 - x^2} = \lim\limits_{x\to 0}\sqrt{5 - 2x^2} = 0$  
    $\sqrt{5 - 2x^2} \le f(x) \le \sqrt{5 - x^2}$ for $-1 \le x \le 1$  
    The Sandwich Theorem gives:  
    $\lim\limits_{x\to 0}f(x) = 0$
#### Estimating Limits
You will find a graphing calculator useful for Exercises 67–74.

67. Let $f(x) = \dfrac{x^2 - 9}{x + 3}$.  
    a. Make a table of the values of $f$ at the points $x = -3.1,-3.01, -3.001$, and so on as far as your calculator can go.
    Then estimate $\lim\limits_{x\to -3}f(x)$. What estimate do you arrive at if
    you evaluate $f$ at $x = -2.9, -2.99, -2.999,\cdots$ instead?  
    b. Support your conclusions in part (a) by graphing $f$ near $c = -3$ and using Zoom and Trace to estimate $y$-values on the graph as $x \to -3$.  
    c. Find $\lim\limits_{x\to -3}f(x)$   algebraically, as in Example 7.  
    a. Estimate: $\lim\limits_{x\to -3}f(x) = -6$  
    c. $\lim\limits_{x\to -3}\dfrac{x^2 - 9}{x + 3} = \lim\limits_{x\to -3}\dfrac{(x - 3)(x + 3)}{x + 3} = \lim\limits_{x\to -3}x - 3 = -3$
#### Theory and Examples
75. If $x^4 \le f(x) \le x^2$ for x in $[-1, 1]$ and $x^2 \le f(x) \le x^4$ for $x < -1$ and $x > 1$, at what points $c$ do you automatically know $\lim\limits_{x\to c}f(x)$? What can you say about the value of the limit at these points?  
    $\lim\limits_{x\to 0}x^4 = \lim\limits_{x\to 0}x^4 = 0$  
    $x^4 \le f(x) \le x^2$ for $-1 \le x \le 1$  
    The Sandwich Theorem gives:  
    $\lim\limits_{x\to 0}f(x) = 0$  
    Similarly, $\lim\limits_{x\to 1}f(x) = 1,\lim\limits_{x\to -1}f(x) = 1$
#### COMPUTER EXPLORATIONS
#### Graphical Estimates of Limits
In Exercises 83–88, use a CAS to perform the following steps:  
a. Plot the function near the point $c$ being approached.  
b. From your plot guess the value of the limit.   

83. $\lim\limits_{x\to 0}\dfrac{x^4 - 16}{x - 2}$  
    $\lim\limits_{x\to 0}\dfrac{x^4 - 16}{x - 2} = 8$







