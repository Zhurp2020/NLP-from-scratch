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
### 2.3 The Precise Definition of a Limit
#### Centering Intervals About a Point
In Exercises 1–6, sketch the interval $(a, b)$ on the $x$-axis with the point $c$ inside. Then find a value of $\delta > 0$ such that $a < x < b$ whenever $0 < |x - c| < \delta$
1. $a = 1, b = 7, c = 5$  
   $\delta = 4$
#### Finding Deltas Graphically
In Exercises 7–14, use the graphs to find a $\delta > 0$ such that 
$$
|f(x) - L| < \varepsilon\quad\mathsf{whenever}\quad0 < |x - c| < \delta.
$$  
  
7. ![](../images/Thomas%20Calculus/2-8.jpg)  
   $\delta = 0.1$
#### Finding Deltas Algebraically
Each of Exercises 15–30 gives a function ƒ(x) and numbers $L$, $c$, and $\varepsilon > 0$. In each case, find an open interval about $c$ on which the inequality $0 < f(x) - L < \varepsilon$ holds. Then give a value for $\delta > 0$ such that for all $x$ satisfying $0 < |x - c| < \delta$ the inequality $|f(x) - L| < \varepsilon$ holds.

15. $f(x) = x + 1, L = 5, c = 4, \varepsilon = 0.01$  
    $0 < x + 1 - 5 < 0.01$  
    $4 < x < 4.01, x\in (4,4.01)$  
    $\delta = 0.01$
#### Using the Formal Definition
Each of Exercises 31–36 gives a function $f(x)$, a point $c$, and a positive number $\varepsilon$. Find $L = \lim\limits_{x\to c}f(x)$. Then find a number $\delta > 0$ such that
$$
|f(x) - L| < \varepsilon\quad\mathsf{whenever}\quad0 < |x - c| < \delta.
$$

31. $f(x) = 3 - 2x, c = 3, \varepsilon = 0.02$  
    $L = \lim\limits_{x\to c}f(x) = f(3) = -3$  
    $|3 - 2x + 3|< 0.02$  
    $-0.02 < -2x + 6 < 0.02$  
    $-3.01 < x < -2.99$  
    $\delta = 0.01$
#### Theory and Examples
51. Define what it means to say that $\lim\limits_{x\to 0}g(x) = k$
    For any given $\varepsilon > 0$, there is a $\delta > 0$ such that 
    $$
    |g(x) - k| < \varepsilon\quad\mathsf{whenever}\quad0 < |x| < \delta.
    $$
#### When Is a Number $L$ Not the Limit of $f(x)$ as $x \to c$?
Showing $L$ is not a limit We can prove that $\lim\limits_{x\to c}f(x) \ne L$ by providing an $\varepsilon > 0$ such that no possible $\delta > 0$ satisfies the condition
$$
|f(x) - L| < \varepsilon\quad\mathsf{whenever}\quad0 < |x - c| < \delta.
$$
We accomplish this for our candidate $\varepsilon$ by showing that for each $\delta > 0$ there exists a value of $x$ such that
$$
|f(x) - L| \ge \varepsilon\quad\mathsf{and}\quad0 < |x - c| < \delta.
$$
57. Let $f(x) = \left\{\begin{aligned}x &\quad x < 1\\x + 1 &\quad x > 1\end{aligned}\right.$  
    a. Let $\varepsilon = \dfrac{1}{2}$. Show that no possible $\delta > 0$ satisfies the following condition:
    $$
    |f(x) - 2| < \dfrac{1}{2}\quad\mathsf{whenever}\quad0 < |x - 1| < \delta.
    $$
    That is, for each $\delta > 0$ show that there is a value of $x$ such that
    $$
    |f(x) - 2| \ge \dfrac{1}{2}\quad\mathsf{and}\quad0 < |x - 1| < \delta.
    $$
    This will show that $\lim\limits_{x\to 1}f(x) \ne \dfrac{1}{2}$.  
    b. Show that $\lim\limits_{x\to 1}f(x) \ne 1$.  
    c. Show that $\lim\limits_{x\to 1}f(x) \ne 1.5$  
    a. $0 < |x - 1| < \delta$  
    $x \ne 1, -\delta + 1 < x < \delta + 1$    
    when $x > 1$:  
    $|f(x) - 2| = |x + 1 - 2| = x - 1 \ge \dfrac{1}{2}, x\ge \dfrac{3}{2}$   
    when $x < 1$:  
    $|f(x) - 2| = |x - 2| = 2 - x \ge \dfrac{1}{2}, x\le \dfrac{3}{2}, x < 1$  
    $x < 1$ or $x \ge \dfrac{3}{2}$ and $-\delta + 1 < x < \delta + 1$  
    For any $\delta > 0$, there is a $1 - \delta < x< 1$ such that 
    $$
    |f(x) - 2| \ge \dfrac{1}{2}\quad\mathsf{and}\quad0 < |x - 1| < \delta.
    $$
    This will show that $\lim\limits_{x\to 1}f(x) \ne \dfrac{1}{2}$.  
    b. when $x > 1$:  
    $|f(x) - 1| = |x| = x \ge \dfrac{1}{2}, x> 1$   
    when $x < 1$:  
    $|f(x) - 1| = |x - 1| = 1 - x \ge \dfrac{1}{2}, x\le \dfrac{1}{2}$  
    $x \le \dfrac{1}{2}$ or $x > 1$ and $-\delta + 1 < x < \delta + 1$  
    For any $\delta > 0$, there is a $1 < x< 1 + \delta$ such that  
    $$
    |f(x) - 1| \ge \dfrac{1}{2}\quad\mathsf{and}\quad0 < |x - 1| < \delta.
    $$
    This will show that $\lim\limits_{x\to 1}f(x) \ne 1$.   
    c. when $x > 1$:  
    $|f(x) - 1.5| = |x + 1- 1.5| = x - 0.5 \ge \dfrac{1}{2}, x> 1$   
    when $x < 1$:  
    $|f(x) - 1.5| = |x - 1.5| = 1.5 - x \ge \dfrac{1}{2}, x\le 1, x < 1$  
    $x < 1$ or $x > 1$ and $-\delta + 1 < x < \delta + 1$  
    For any $\delta > 0$, there is a $1 - \delta < x< 1$ such that  
    $$
    |f(x) - 1.5| \ge \dfrac{1}{2}\quad\mathsf{and}\quad0 < |x - 1| < \delta.
    $$
    This will show that $\lim\limits_{x\to 1}f(x) \ne 1.5$.
#### COMPUTER EXPLORATIONS
In Exercises 61–66, you will further explore finding deltas graphically. Use a CAS to perform the following steps:  
a. Plot the function $y = f(x)$ near the point $c$ being approached.  
b. Guess the value of the limit $L$ and then evaluate the limit symbolically to see if you guessed correctly.   
c. Using the value $\varepsilon = 0.2$, graph the banding lines $y_1 = L - \varepsilon$ and $y_2 = L + \varepsilon$ together with the function $f$ near $c$.  
d. From your graph in part (c), estimate a $\delta > 0$ such that
$$
|g(x) - k| < \varepsilon\quad\mathsf{whenever}\quad0 < |x| < \delta.
$$
Test your estimate by plotting $f$, $y_1$, and $y_2$ over the interval $0 < |x - c| < \delta$. For your viewing window use $c - 2\delta \le x \le c + 2\delta$ and $L - 2\varepsilon \le x \le L + 2\varepsilon$. If any function values lie outside the interval $[L - \varepsilon, L + \varepsilon]$, your choice of $\delta$ was too large. Try again with a smaller estimate.
e. Repeat parts (c) and (d) successively for $\varepsilon = 0.1, 0.05$, and $0.001$.  

61. $f(x) =\dfrac{x^4 - 81}{x - 3}, c = 3$  
    b. $\lim\limits_{x\to 3}\dfrac{x^4 - 81}{x - 3} = \dfrac{(x^2 +9)(x - 3)(x + 3)}{x - 3} = 18\cdot6 = 108$
### 2.4 One-Sided Limits
#### Finding Limits Graphically
1. Which of the following statements about the function $y = f(x)$ graphed here are true, and which are false?  
![](../images/Thomas%20Calculus/2-9.jpg)  
a. $\lim\limits_{x\to -1^+}f(x)= 1$ b. $\lim\limits_{x\to 0^-}f(x)= 0$  
c. $\lim\limits_{x\to 0^-}f(x)= 1$ d. $\lim\limits_{x\to 0^-}= \lim\limits_{x\to 0^+}f(x)$  
e. $\lim\limits_{x\to 0}f(x)$ exists. f. $\lim\limits_{x\to 0}f(x) = 0$    
g. $\lim\limits_{x\to 0}f(x) = 1$ h. $\lim\limits_{x\to 1}f(x) = 1$  
i. $\lim\limits_{x\to 1}f(x) = 0$ j. $\lim\limits_{x\to 2^-}f(x) = 2$  
k. $\lim\limits_{x\to 1^-}f(x)$ does not exist. l. $\lim\limits_{x\to 2^+}f(x) = 0$  
    True: a,b,d,e,j   
    False: c,f,g,h,i,k,l
#### Finding One-Sided Limits Algebraically
Find the limits in Exercises 11–20.

11. $\lim\limits_{x\to -0.5^-}\sqrt{\dfrac{x + 2}{x + 1}}$  
    $\lim\limits_{x\to -0.5^-}\sqrt{\dfrac{x + 2}{x + 1}} = \sqrt{\dfrac{\frac{3}{2}}{\frac{1}{2}}} = \sqrt{3}$ 
#### Using $\lim\limits_{\theta\to 0}\dfrac{\sin\theta}{\theta} = 1$
Find the limits in Exercises 23–46.

23. $\lim\limits_{\theta\to 0}\dfrac{\sin\sqrt{2}\theta}{\sqrt{2}\theta}$   
   $\lim\limits_{\theta\to 0}\dfrac{\sin\sqrt{2}\theta}{\sqrt{2}\theta} =1$
#### Theory and Examples
47. Once you know $\lim\limits_{x\to a^+}f(x)$ and $\lim\limits_{x\to a^-}f(x)$ at an interior point
of the domain of $f$, do you then know $\lim\limits_{x\to a}f(x)$? Give reasons for your answer.  
    No. The limit might not exist.
#### Formal Definitions of One-Sided Limits
51. Given $\varepsilon > 0$, find an interval $I = (5, 5 + \delta), \delta > 0$, such that if $x$ lies in $I$, then $\sqrt{x - 5} <\varepsilon$. What limit is being verified and what is its value?  
    $\lim\limits_{x\to 5^+}\sqrt{x - 5} = 0$
### 2.5 Continuity
#### Continuity from Graphs
In Exercises 1–4, say whether the function graphed is continuous on $[3-1, 3]$. If not, where does it fail to be continuous and why?
1. ![](../images/Thomas%20Calculus/2-10.jpg)   
   No. The function is not defined at $x = 2$
#### Applying the Continuity Test
At which points do the functions in Exercises 11 and 12 fail to be continuous? At which points, if any, are the discontinuities removable? Not removable? Give reasons for your answers.

11. Exercise 1, Section 2.4  
    ![](../images/Thomas%20Calculus/2-9.jpg)   
    The function has a removable discontinuity at $x = 0$ and a jump discontinuity at $x = 1$. Because $\lim\limits_{x\to 0}f(x) = 0 \ne f(0) = 1$ and $\lim\limits_{x\to 1}f(x)$ does not exist. 
#### Limits Involving Trigonometric Functions
Find the limits in Exercises 31–36. Are the functions continuous at the point being approached?

31. $\lim\limits_{x\to \pi}\sin (x - \sin x)$  
    $\lim\limits_{x\to \pi}(x - \sin x) = \lim\limits_{x\to \pi}x - \lim\limits_{x\to \pi}\sin x= \pi$  
    $\sin x$ is continuous at $x = \pi$  
    $\therefore \lim\limits_{x\to \pi}\sin (x - \sin x) = \sin\pi = 0$  
    $\lim\limits_{x\to \pi}\sin (x - \sin x) = \sin (\pi - \sin \pi) = 0$, the function is continuous at $x = \pi$
#### Continuous Extensions
37. Define $g(3)$ in a way that extends $g(x) = \dfrac{x^2 - 9}{x - 3}$ to be continuous at $x = 3$.
    $g(x) = \left\{\begin{aligned}\dfrac{x^2 - 9}{x - 3}&\quad x \ne 3 \\ 6&\quad x = 3\end{aligned}\right.$
#### Theory and Examples
47. A continuous function $y = f(x)$ is known to be negative at $x = 0$ and positive at $x = 1$. Why does the equation $f(x) = 0$ have at least one solution between $x = 0$ and $x = 1$? Illustrate with a sketch.  
    $f$ is continuous over $[0,1]$  
    $f(0) < 0 < f(1)$  
    The Intermediate Value Theorem for Continuous Functions gives that there is a $c\in [0,1]$ such that $f(c) = 0$ 
### 2.6 Limits Involving Infinity; Asymptotes of Graphs
#### Finding Limits
1. For the function $f$ whose graph is given, determine the following limits.  
   ![](../images/Thomas%20Calculus/2-11.jpg)
   a. $\lim\limits_{x\to 2}f(x)$b. $\lim\limits_{x\to -3^+}f(x)$  
   c. $\lim\limits_{x\to -3^-}f(x)$ d. $\lim\limits_{x\to -3}f(x)$  
    e. $\lim\limits_{x\to 0^+}f(x)$ f. $\lim\limits_{x\to 0^-}f(x)$  
    g. l$\lim\limits_{x\to 0}f(x)$ h. $\lim\limits_{x\to +\infty}f(x)$  
    i. $\lim\limits_{x\to -\infty}f(x)$  
    a. 0 b. -2  
    c. 2 d. does not exist  
    e. -1 f. $+\infty$  
    g. does not exist h. 1    
    i. 0
#### Limits of Rational Functions
In Exercises 13–22, find the limit of each rational function (a) as $x \to +\infty$ and (b) as $x \to -\infty$.

13. $f(x) =\dfrac{2x + 3}{5x + 7}$  
    $\lim\limits_{x\to +\infty}f(x) = \lim\limits_{x\to -\infty}f(x) =\dfrac{2}{5}$
#### Limits as $x \to +\infty$ or $x \to -\infty$
The process by which we determine limits of rational functions applies equally well to ratios containing noninteger or negative powers of $x$:  
Divide numerator and denominator by the highest power of $x$ in the denominator and proceed from there. Find the limits in Exercises 23–36.

23. $\lim\limits_{x\to +\infty}\dfrac{\sqrt{8x^2 - 3}}{\sqrt{2x^2 + x}}$  
    $\lim\limits_{x\to +\infty}\dfrac{\sqrt{8x^2 - 3}}{\sqrt{2x^2 + x}} = \lim\limits_{x\to +\infty}\sqrt{\dfrac{8 - \frac{3}{x^2}}{2 + \frac{1}{x}}} = \sqrt{4} = 2$
#### Infinite Limits
Find the limits in Exercises 37–48.

37. $\lim\limits_{x\to 0}\dfrac{1}{3x}$  
    $\lim\limits_{x\to 0}\dfrac{1}{3x} = 0$
#### Graphing Simple Rational Functions
Graph the rational functions in Exercises 63–68. Include the graphs and equations of the asymptotes and dominant terms.

63. $y = \dfrac{1}{x - 1}$
#### Domains, Ranges, and Asymptotes
Determine the domain and range of each function. Use various limits to find the asymptotes and the ranges.

69. $y = 4 + \dfrac{3x^2}{x^2 + 1}$  
    $D:R, R:[4,7)$
#### Inventing Graphs and Functions
In Exercises 73–76, sketch the graph of a function $y = f(x)$ that satisfies the given conditions. No formulas are required—just label the coordinate axes and sketch an appropriate graph. (The answers are not unique, so your graphs may not be exactly like those in the answer section.)

73. $f(0) = 0, f(1) = 2, f(-1) = -2, \lim\limits_{x\to -\infty}f(x) = -1$ and $\lim\limits_{x\to \infty}f(x) = 1$
    $f(x) = \left\{\begin{aligned}\dfrac{1}{x} - 1 &\quad x < -1 \\ 2x &\quad -1 \le x \le 1 \\ \dfrac{1}{x} + 1 &\quad x > 1 \end{aligned}\right.$
#### Finding Limits of Differences When x u tH
Find the limits in Exercises 84–90. (Hint: Try multiplying and dividing by the conjugate.)

84. $\lim\limits_{x\to \infty}(\sqrt{x + 9} - \sqrt{x + 4})$  
    $\lim\limits_{x\to \infty}(\sqrt{x + 9} - \sqrt{x + 4}) = \lim\limits_{x\to \infty}\dfrac{(x + 9) - (x + 4)}{\sqrt{x + 9} + \sqrt{x + 4}} =0$
#### Using the Formal Definitions
Use the formal definitions of limits as $x\to \plusmn\infty$ to establish the limits in Exercises 91 and 92.

91. If $f$ has the constant value $f(x) = k$, then $\lim\limits_{x\to \infty}f(x) = k$   
    Given a $\varepsilon > 0$:  
    $|f(x) - k| < \varepsilon, 0 < \varepsilon$  
    There is a $M = 1$ such that:
    $$
    |f(x) - k| < \varepsilon\quad\mathsf{whenever}\quad x > M
    $$
    $\lim\limits_{x\to \infty}f(x) = k$
#### Oblique Asymptotes
Graph the rational functions in Exercises 103–108. Include the graphs and equations of the asymptotes.

103. $y = \dfrac{x^2}{x - 1}$
#### Additional Graphing Exercises
Graph the curves in Exercises 109–112. Explain the relationship between the curve’s formula and what you see.

109. $y = \dfrac{x}{\sqrt{4 - x^2}}$
### Practice Exercises
Limits and Continuity
1. Graph the function
   $$
   f(x) = \left\{\begin{aligned}
       1&\quad x \le -1\\
       -x&\quad -1 < x < 0\\
       1&\quad x = 0\\
       -x&\quad 0 < x < 1\\
       1&\quad x \ge 1
   \end{aligned}\right.
   $$
Then discuss, in detail, limits, one-sided limits, continuity, and one-sided continuity of $f$ at $x = -1, 0$, and $1$. Are any of the discontinuities removable? Explain  
$\lim\limits_{x\to-1} = 1, \lim\limits_{x\to1^-} = -1,\lim\limits_{x\to1^+} = 1, \lim\limits_{x\to0} = 0$.  
The function has a removable discontinuity at $x = 0$ and a jump discontinuity at $x = 1$
#### Finding Limits
In Exercises 9–28, find the limit or explain why it does not exist.
 
9. $\lim\dfrac{x^2 - 4x + 4}{x^3 + 5x^2 -14x}$  
    a. as $x \to 0$ b. as $x \to 2$  
    a. $\lim\limits_{x \to 0}\dfrac{x^2 - 4x + 4}{x^3 + 5x^2 -14x} = \lim\limits_{x \to 0}\dfrac{(x - 2)^2}{x(x + 7)(x - 2)} = \lim\limits_{x \to 0}\dfrac{x - 2}{x(x + 7)}$  
    It does not exist because it grows arbitrarily large near $x = 0$.  
    b. $\lim\limits_{x \to 2}\dfrac{x^2 - 4x + 4}{x^3 + 5x^2 -14x} = \lim\limits_{x \to 2}\dfrac{x - 2}{x(x + 7)} = 0$
#### Roots
29. Let $f(x) = x^3 - x - 1$.  
    a. Use the Intermediate Value Theorem to show that $f$ has a zero between -1 and 2.  
    b. Solve the equation $f(x) = 0$ graphically with an error of magnitude at most $10^{-8}$.  
    c. It can be shown that the exact value of the solution in part (b) is
    $$
    (\dfrac{1}{2} + \dfrac{\sqrt{69}}{18})^{\dfrac{1}{3}} + (\dfrac{1}{2} - \dfrac{\sqrt{69}}{18})^{\dfrac{1}{3}}
    $$
    Evaluate this exact answer and compare it with the value you found in part (b).  
    a. $f(-1) = -1 < 0< f(2) = 5$  
    $f$ is continuous over $[-1,2]$.  
    The Intermediate Value Theorem gives that $f$ has a zero between -1 and 2.  
#### Continuous Extension
31. Can $f(x) = \dfrac{x (x^2 - 1)}{|x^2 - 1|}$ be extended to be continuous at $x = 1$ or $-1$? Give reasons for your answers. (Graph the function—you will find the graph interesting.)   
   $f(x) = \left\{\begin{aligned}x&\quad x < -1 \\-x&\quad -1 < x < 1\\ x&\quad x >1\end{aligned}\right.$  
   The function has a jump discontinuity at $x = 1$ and $-1$. It can not be extended to continuous.
#### Limits at Infinity
Find the limits in Exercises 37–46.

37. $\lim\limits_{x \to \infty}\dfrac{2x + 3}{5x + 7}$  
    $\lim\limits_{x \to \infty}\dfrac{2x + 3}{5x + 7} = \dfrac{2}{5}$
#### Horizontal and Vertical Asymptotes
47. Use limits to determine the equations for all vertical asymptotes.   
    a. $y =\dfrac{x^2 + 4}{x - 3}$ b. $f(x) =\dfrac{x^2 - x - 2}{x^2 - 2x + 1}$  
    c. $y =\dfrac{x^2 + x - 6}{x^2 + 2x - 8}$  
    a. $y =\dfrac{x^2 + 4}{x - 3} = x + 3 + \dfrac{7}{x - 3}$  
    The vertical asymptotes is $x = 3$  
    b. $f(x) =\dfrac{x^2 - x - 2}{x^2 - 2x + 1} = 1 + \dfrac{x - 3}{x^2 - 2x + 1}$.  
    The vertical asymptotes is $x = 1$  
    c. $y =\dfrac{x^2 + x - 6}{x^2 + 2x - 8} = 1-\dfrac{x - 2}{x^2 + 2x - 8} = 1-\dfrac{x -2}{(x + 4)(x - 2)} = 1 - \dfrac{1}{x + 4}$  
    The vertical asymptotes is $x = -4$ 
### Additional and Advanced Exercises
1. Lorentz contraction In relativity theory, the length of an object, say a rocket, appears to an observer to depend on the speed at which the object is traveling with respect to the observer. If the observer measures the rocket’s length as $L_0$at rest, then at speed $y$ the length will appear to be
$$
L = L_0\sqrt{1 - \dfrac{v^2}{c^2}}
$$
This equation is the Lorentz contraction formula. Here, $c$ is the speed of light in a vacuum, about $3 * 10^8 m/sec$. What happens to $L$ as $y$ increases? Find $\lim\limits_{y\to c^-} L$. Why was the left-hand limit needed?  
$\lim\limits_{y\to c^-} L = 0$
#### Precise Definition of Limit
In Exercises 5–8, use the formal definition of limit to prove that the function is continuous at $c$.   

5. $f(x) = x^2 - 7, c = 1$  
   $\lim\limits_{x\to 1} = -6$   
   Let $\varepsilon > 0$ be given  
   $|f(x) + 6| < \varepsilon$   
   $1 - \varepsilon < x^2 < 1 + \varepsilon$  
   $-\sqrt{1 + \varepsilon} < x < \sqrt{1 + \varepsilon}$ and $x < -\sqrt{1 - \varepsilon}$ or $x > \sqrt{1 - \varepsilon}$     
   $\sqrt{1 - \varepsilon} < x < \sqrt{1 + \varepsilon}$ or $-\sqrt{1 + \varepsilon} < x < -\sqrt{1 - \varepsilon}$  
   There is a $0 < \delta < \sqrt{1 + \varepsilon} -1$ such that  
   $$
    |f(x) + 6| < \varepsilon\quad\mathsf{whenever}\quad |x - 1| < \delta
   $$
   This proves that $\lim\limits_{x\to 1} = -6$  
   $\lim\limits_{x\to 1} = -6 = f(1)$  
   This proves that the function is continuous at $x = 1$
#### Generalized Limits Involving $\dfrac{\sin\theta}{\theta}$
The formula $\lim\limits_{x\to0}\dfrac{\sin\theta}{\theta} = 1$ can be generalized. If $\lim\limits_{x\to0}f(x) = 0$ and $f(x)$ is never zero in an open interval containing the point $x = c$, except possibly at $c$ itself, then
$$
\lim\limits_{x\to0}\dfrac{\sin f(x)}{f(x)} = 1
$$
Here are several examples.  
a. $\lim\limits_{x\to0}\dfrac{\sin x^2}{x^2} = 1$  
b. $\lim\limits_{x\to0}\dfrac{\sin x^2}{x} = \lim\limits_{x\to0}\dfrac{\sin x^2}{x^2}\lim\limits_{x\to0}\dfrac{x^2}{x} = 0$  
c.  $\lim\limits_{x\to-1}\dfrac{\sin (x^2 - x - 2)}{x + 1} = \lim\limits_{x\to-1}\dfrac{\sin (x^2 - x - 2)}{x^2 - x - 2}\lim\limits_{x\to-1}\dfrac{x^2 - x - 2}{x + 1} = \lim\limits_{x\to-1}\dfrac{(x - 2)(x + 1)}{x + 1} = -3$  
d. $\lim\limits_{x\to1}\dfrac{\sin (1-\sqrt{x})}{x - 1} = \lim\limits_{x\to1}\dfrac{\sin (1-\sqrt{x})}{1-\sqrt{x}}\dfrac{1-\sqrt{x}}{x - 1} =\lim\limits_{x\to1}\dfrac{-1}{1 + \sqrt{x}} = -\dfrac{1}{2}$  
Find the limits in Exercises 23–28.

23. $\lim\limits_{x\to0}\dfrac{\sin (1 - \cos x)}{x}$  
    $\lim\limits_{x\to0}\dfrac{\sin (1 - \cos x)}{x} =\lim\limits_{x\to0}\dfrac{\sin (1 - \cos x)}{1 - \cos x}\dfrac{1 - \cos x}{x} =\lim\limits_{x\to0}\dfrac{2\sin^2\frac{x}{2}}{x} = \lim\limits_{x\to0}\sin\dfrac{x}{2}\lim\limits_{x\to0}\dfrac{\sin\frac{x}{2}}{\frac{x}{2}} = 0$
#### Oblique Asymptotes
Find all possible oblique asymptotes in Exercises 29–32.

29. $y = \dfrac{2x^\frac{3}{2}+ 2x - 3}{\sqrt{x} + 1}$  
    $y = \dfrac{2x^\frac{3}{2}+ 2x - 3}{x^\frac{1}{2} + 1} =2x - \dfrac{3}{x^\frac{1}{2} + 1}$  
    The oblique asymptotes is $y = 2x$
#### Showing an Equation Is Solvable
33. Assume that $1 < a < b$ and $\dfrac{a}{x} + x = \dfrac{1}{x - b}$. Show that this equation is solvable.   
    $\dfrac{a}{x} + x = \dfrac{1}{x - b}$   
    $a(x - b) + x^2(x - b) - x= 0$  
    Let $f(x) = a(x - b) + x^2(x - b) - x$   
    $f(1) = a -ab + 1 -b -1 = a - b -ab < 0$  
    $f(a + b) = a^2 + a(a+b)^2 - a -b =a^2 + a^3 + 2a^2b + ab^2 -a-ab > a^2 + a^3 + 2a^2b + ab^2 - 2a^b = a^2 + a^3 + ab^2 > 0$  
    $f(1)<0<f(a+b)$, $f$ is continuous over $(1,a+b)$.  
    There is a $c\in(1, a+b)$ such that $f(c) = 0$. This shows that the equation is solvable.