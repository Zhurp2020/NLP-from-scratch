# Thomas Calculus
## Chapter 1 Functions
### 1.1 Functions and their graphs
#### Functions
In Exercises 1–6, find the domain and range of each function.  
In Exercises 7 and 8, which of the graphs are graphs of functions of $x$, and which are not? Give reasons for your answers. 
1. $f(x) = 1 + x^2$  
   $D: R$  
   $R: [1,+\infty)$
2. $f(x) = 1 - \sqrt{x}$  
   $\sqrt{x} \ge 0,-\sqrt{x} \le 0$  
   $1 - \sqrt{x} = -\sqrt{x} +1 \le 1$  
   $D: [0,+\infty]$  
   $R: (-\infty,1]$
3. $F(x) = \sqrt{5x + 10}$   
   $5x + 10 \ge 0, x \ge -2$  
   $D: [-2,+\infty]$  
   $R: [0,+\infty)$
4. $g(x) = \sqrt{x^2 - 3x}$  
   $x^2 - 3x \ge 0, x(x-3) \ge 0$  
   $x \le 0$ or $x \ge 3$  
   $D: (-\infty,0] \cup [3,+\infty)$  
   $R: [0,+\infty)$
5. $f(t) = \dfrac{4}{3-t}$  
   $3-t \ne 0, t \ne 3$   
   $D: (-\infty,3) \cup (3,+\infty)$  
   $R: (-\infty,0) \cup (0,+\infty)$
6. $G(t) = \dfrac{2}{t^2 - 16}$  
   $t^2 -16 \ne 0, t \ne 4$ and $t \ne -4$   
   $t^2 -16 \ge -16$  
   $\dfrac{2}{t^2 - 16} \le -\dfrac{1}{8}$ or $\dfrac{2}{t^2 - 16} \ge 0$  
   $D: (-\infty,-4) \cup (-4,4) \cup (4,+\infty)$  
   $R: (-\infty,-\dfrac{1}{8}] \cup (0,+\infty)$     
7. graph:   
   ![](../images/Thomas%20Calculus/1-7.jpg)  
   a. A vertical line will intersect with the b graph twice.     
8. graph:   
   ![](../images/Thomas%20Calculus/1-9.jpg)    
   Neither a nor b.  
#### Finding Formulas for Functions
9. Express the area and perimeter of an equilateral triangle as a function of the triangle’s side length $x$.  
   $S=\dfrac{\sqrt{3}}{4}x$
10. Express the side length of a square as a function of the length $d$ of the square’s diagonal. Then express the area as a function of the diagonal length.  
   $l=\dfrac{\sqrt{2}}{2}d$   
   $S=l^2=\dfrac{1}{2}d^2$
11. Express the edge length of a cube as a function of the cube’s diagonal length $d$. Then express the surface area and volume of the cube as a function of the diagonal length.  
   $3l^2 = d^2$  
   $l = \dfrac{\sqrt{3}}{3}d$  
   $S = l^2 = \dfrac{3}{9}d^2 = \dfrac{1}{3}d^2$   
   $V = l^3 = \dfrac{3\sqrt{3}}{27}d^3 = \dfrac{1}{9}d^3$
12. A point $P$ in the first quadrant lies on the graph of the function $f(x) = \sqrt{x}$. Express the coordinates of $P$ as functions of the slope of the line joining $P$ to the origin.  
   $k = \dfrac{\sqrt{x}}{x}$  
   $k^2 = \dfrac{1}{x}$  
   $x = \dfrac{1}{k^2}$  
   $y = \sqrt{x} = \dfrac{1}{k}$
13. Consider the point $(x, y)$ lying on the graph of the line $2x + 4y = 5$. Let $L$ be the distance from the point $(x, y)$ to the origin $(0, 0)$. Write $L$ as a function of $x$.   
   $2x + 4y = 5, y = \dfrac{5-2x}{4}$  
   $L = \sqrt{x^2 + y^2}$   
   &emsp;$= \sqrt{x^2 + \dfrac{25 - 20x + 4x^2}{16}}$  
   &emsp;$= \sqrt{\dfrac{5x^2 - 20x + 25}{16}}$  
   &emsp;$= \dfrac{\sqrt{5x^2 - 20x + 25}}{4}$
14. Consider the point $(x, y)$ lying on the graph of $y = 2x - 3$. Let $L$ be the distance between the points $(x, y)$ and $(4, 0)$. Write $L$ as a function of $y$.  
   $y = 2x - 3, x = \dfrac{y + 3}{2}$  
   $L = \sqrt{(x - 4)^2 + y^2}$   
   &emsp;$= \sqrt{(\dfrac{y + 3}{2} - 4)^2 + y^2}$   
   &emsp;$= \sqrt{(\dfrac{y}{2}-\dfrac{5}{2})^2 + y^2}$   
   &emsp;$= \sqrt{\dfrac{y^2}{4} - \dfrac{5}{2}y + \dfrac{25}{4} + y^2}$    
   &emsp;$= \sqrt{\dfrac{5y^2 -10y + 25}{4}}$   
   &emsp;$= \dfrac{\sqrt{5y^2 -10y + 25}}{2}$  
#### Functions and Graphs
Find the natural domain and graph the functions in Exercises 15–20.  

15. $f(x) = 5 - 2x$  
   $D: R$
16. $f(x) = 1 - 2x - x^2$  
   $D: R$
17. $g(x) = \sqrt{|x|}$   
   $D: R$
18. $g(x) = \sqrt{-x}$  
   $D: (-\infty,0]$
19. $F(t) = \dfrac{t}{|t|}$  
   $D: (-\infin,0)\cup(0,+\infty)$
20. $G(t) = \dfrac{1}{|t|}$  
   $D: (-\infin,0)\cup(0,+\infty)$
21. Find the domain of $y =\dfrac{x + 3}{4 - \sqrt{x^2 - 9}}$.    
   $\left\{\begin{aligned}4 - \sqrt{x^2 - 9} \ne 0 \\ x^2 - 9 \ge 0\end{aligned}\right.$  
   $\left\{\begin{aligned} {x^2 - 9} &\ne 16 \\ x^2 &\ge 9\end{aligned}\right.$   
   $\left\{\begin{aligned} x &\ne \plusmn 5 \\ x \ge 3 \quad &or \quad  x \le -3\end{aligned}\right.$  
   $D: (-\infty,-5)\cup(5,-3]\cup[3,5)\cup(5,+\infty)$  
22. Find the range of $y = 2 + \sqrt{9 + x^2}$.   
   $9 + x^2 \ge 9, \sqrt{9 + x^2} \ge 3$   
   $R: [5,+\infty$
23. Graph the following equations and explain why they are not
graphs of functions of $x$.   
   a. $|y| = x$ b. $y^2 = x^2$
24. Graph the following equations and explain why they are not
graphs of functions of $x$.       
   a. $|x| + |y| = 1$ b. $|x + y| = 1$
#### Piecewise-Defined Functions
Graph the functions in Exercises 25–28.    

25. $f(x) = \left\{\begin{aligned} x &, 0 \le x \le 1\\ 2 - x &, 1 < x \le 2\end{aligned}\right.$  
26. $g(x) = \left\{\begin{aligned} 1 - x &, 0 \le x \le 1\\ 2 - x &, 1 < x \le 2\end{aligned}\right.$  
27. $F(x) = \left\{\begin{aligned} 4 - x &, x \le 1\\ x^2 + 2x &, x > 1\end{aligned}\right.$   
28. $G(x) = \left\{\begin{aligned} \dfrac{1}{x} &, x < 0\\ x &, x \ge 0\end{aligned}\right.$   
    
Find a formula for each function graphed in Exercises 29–32.    
![](../images/Thomas%20Calculus/1-11.jpg)  
![](../images/Thomas%20Calculus/1-12.jpg)  

29. a. $f(x) = \left\{\begin{aligned}x &, 0 \le x \le 1\\ 2 - x &, 1 < x \le 2\end{aligned}\right.$   
    b. $f(x) = \left\{\begin{aligned}2 &, 0 \le x < 1\quad or\quad 2 \le x < 3\\ 0 &, 1 \le x < 2 \quad or\quad 3 \le x \le 4\end{aligned}\right.$    
30. a. $\left\{\begin{aligned} 5k + b = 0 \\ 2k + b = 1\end{aligned}\right.$   
    &emsp;$\left\{\begin{aligned} k &= -\dfrac{1}{3} \\ b &= \dfrac{5}{3}\end{aligned}\right.$   
    $f(x) = \left\{\begin{aligned}2 - x &, 0 < x \le 2\\ -\dfrac{1}{3}x + \dfrac{5}{3}&, 2 < x \le 5\end{aligned}\right.$   
    b. $f(x) = \left\{\begin{aligned}-3x -3 &, -1 < x \le 0\\ -2x + 3&, 0 < x \le 1\end{aligned}\right.$  
31. a. $\left\{\begin{aligned} 3k + b = 0 \\ k + b = 1\end{aligned}\right.$   
    &emsp;$\left\{\begin{aligned} k &= -\dfrac{1}{2} \\ b &= \dfrac{3}{2}\end{aligned}\right.$   
    $f(x) = \left\{\begin{aligned} -x &, -1 \le x < 0\\ 1&, 0 < x \le 1 \\ -\dfrac{1}{2}x + \dfrac{3}{2} &, 1 \le x < 3\end{aligned}\right.$   
    b. $f(x) = \left\{\begin{aligned} -\dfrac{1}{2}x &, -2 \le x \le 0\\ -2x + 2&, 0 < x \le 1 \\ -1 &, 1 < x \le 3\end{aligned}\right.$  
32. a. $\left\{\begin{aligned} 3k + b = 0 \\ k + b = 1\end{aligned}\right.$   
    &emsp;$\left\{\begin{aligned} k &= -\dfrac{1}{2} \\ b &= \dfrac{3}{2}\end{aligned}\right.$  
    $f(x) = \left\{\begin{aligned} 0 &, 0 \le x < \dfrac{T}{2}\\ 2Tx - 2T^2 + 1&, \dfrac{T}{2} < x \le T \end{aligned}\right.$   
    b. $f(x) = \left\{\begin{aligned}A &, 0 \le x < \dfrac{T}{2}\quad or\quad T \le x < \dfrac{3}{2}T\\ -A &, \dfrac{T}{2} \le x < T \quad or\quad \dfrac{3}{2}T \le x \le 2T\end{aligned}\right.$  
#### The Greatest and Least Integer Functions
33. For what values of $x$ is  
   a. $\lfloor x\rfloor = 0$ b. $\lceil x\rceil = 0$  
   a. $x \in [0,1)$ b. $x \in (-1,0]$
34. What real numbers $x$ satisfy the equation $\lfloor x\rfloor = \lceil x\rceil$    
   $x \in Z$
35. Does $\lceil -x\rceil = -\lfloor x\rfloor$; for all real $x$? Give reasons for your answer.  
   $x = a + b, -x = -a - b$  
   $\lceil -x\rceil = -a,-\lfloor x\rfloor = -a$  
   $\therefore \lceil -x\rceil = -\lfloor x\rfloor$ 
36. Graph the function, Why is $f(x)$ called the integer part of x?  
$$
f(x) = \left\{\begin{aligned}
   \lfloor x \rfloor , x \ge 0  \\
   \lceil  x \rceil  , x <   0
\end{aligned}
\right.
$$ 
#### Increasing and Decreasing Functions
Graph the functions in Exercises 37–46. What symmetries, if any, do the graphs have? Specify the intervals over which the function is increasing and the intervals where it is decreasing.  

37. $y = -x^3$    
    Decreasing: $R$
38. $y = -\dfrac{1}{x^2}$  
    Decreasing: $(-\infty,0)$   
    Increasing: $(0,+\infty)$    
39. $y = -\dfrac{1}{x}$  
    Increasing: $(-\infty,0),(0,+\infty)$
40. $y = \dfrac{1}{|x|}$  
    Decreasing: $(-\infty,0)$   
    Increasing: $(0,+\infty)$
41. $y = \sqrt{|x|}$  
    Decreasing: $(-\infty,0]$   
    Increasing: $[0,+\infty)$
42. $y = \sqrt{-x}$  
    Decreasing: $(-\infty,0]$ 
43. $y = \dfrac{x^3}{8}$  
    Increasing: $R$
44. $y = -4\sqrt{x}$   
    Decreasing: $[0,+\infty)$  
45. $y = -x^\frac{3}{2}$   
    Decreasing: $[0,+\infty)$
46. $y = (-x)^\frac{3}{2}$  
    Decreasing: $(-\infty,0]$  
#### Even and Odd Functions
In Exercises 47–58, say whether the function is even, odd, or neither. Give reasons for your answer.  

47. $f(x) = 3$   
    even, $f(x) = f(-x) = 3$
48. $f(x) = x^{-5}$  
    odd, $-f(x) = f(-x) = x$
49. $f(x) = x^2 + 1$  
    even, $f(x) = f(-x) = x^2 + 1$
50. $f(x) = x^2 + x$  
    neither  
    $-f(x) = -x^2 - x,f(-x) = x^2 - x$
51. $g(x) = x^3 + x$    
    odd, $-g(x) = g(-x) = -x^3 - x$
52. $g(x) = x^4 + 3x - 1$  
    even, $g(x) = g(-x) = x^4 + 3x - 1$
53. $g(x) = \dfrac{1}{x^2 - 1}$  
    even, $g(x) = g(-x) = \dfrac{1}{x^2 - 1}$
54. $g(x) = \dfrac{x}{x^2 - 1}$   
    odd  
    $-g(x) = g(-x) = -\dfrac{x}{x^2 - 1}$
55. $h(t) = -\dfrac{1}{t - 1}$  
    neither  
    $-h(t) = \dfrac{1}{t - 1},h(-t) = -\dfrac{1}{-t - 1} = \dfrac{1}{t + 1}$
56. $h(t) = -|t^3|$    
    even, $h(t) = h(-t) = -|t^3|$
57. $h(t) = 2t + 1$   
    neither  
    $-h(t) = -2t - 1,h(-t) = -2t + 1$  
58. $h(t) = 2|t| + 1$    
    even, $h(t) = h(-t) = 2|t| + 1$
59. $\sin 2x$    
    odd, $-f(x) = f(-x) = -\sin2x$
60. $\sin x^2$   
    even, $f(x) = f(-x) = \sin x^2$
61. $\cos 3x$   
    even, $f(x) = f(-x) = \cos 3x$
62. $1 + \cos x$  
    even, $f(x) = f(-x) = 1 + \cos x$
#### Theory and Examples
63. The variable $s$ is proportional to $t$, and $s = 25$ when $t = 75$.Determine $t$ when $s = 60$.  
    $s = \dfrac{1}{3}t$   
    $s = 60, t = 180$
64. **Kinetic energy** The kinetic energy $K$ of a mass is proportional to the square of its velocity $y$. If $K = 12,960 joules$ when $y = 18 m/sec$, what is $K$ when $y = 10 m/sec$?  
    $K = 40y^2$  
    $K = 4,000 joules$
65. The variables $r$ and $s$ are inversely proportional, and $r = 6$ when $s = 4$. Determine $s$ when $r = 10$.   
    $s = \dfrac{24}{r}$  
    $s = \dfrac{12}{5}$
66. **Boyle’s Law** Boyle’s Law says that the volume $V$ of a gas at constant temperature increases whenever the pressure $P$ decreases, so that $V$ and $P$ are inversely proportional. If $P = 14.7 lb/in^2$ when $V = 1000 in^3$, then what is $V$ when $P = 23.4 lb/in^2$?  
    $V = \dfrac{14700}{P}$  
    $V = \dfrac{14700}{P} = 628.2in^3$
67. A box with an open top is to be constructed from a rectangular piece of cardboard with dimensions $14 in$. by $22 in$. by cutting out equal squares of side $x$ at each corner and then folding up the sides as in the figure. Express the volume $V$ of the box as a function of $x$.  
    ![](../images/Thomas%20Calculus/1-13.jpg)   
    $V = (22 - 2x)(14 - 2x)x$     
    &emsp;$= (4x^2 - 72x + 308)x$  
    &emsp;$= 4x^3 - 72x^2 + 308x$
68. The accompanying figure shows a rectangle inscribed in an isosceles right triangle whose hypotenuse is $2$ units long.   
    ![](../images/Thomas%20Calculus/1-14.jpg)   
    a. Express the $y$-coordinate of $P$ in terms of $x$. (You might start by writing an equation for the line $AB$.)     
    $\dfrac{y}{OB} = \dfrac{AP}{AB}$   
    $\dfrac{y}{1} = \dfrac{\sqrt{2}(1 - x)}{\sqrt{2}}$   
    $y = 1 - x$  
    b. Express the area of the rectangle in terms of $x$.    
    $S = 2xy$  
    
In Exercises 69 and 70, match each equation with its graph. Do not use a graphing device, and give reasons for your answer.

69. a. $y = x^4$ b. $y = x^7$ c. $y = x^{10}$    
    ![](../images/Thomas%20Calculus/1-15.jpg)    
    a-$h$, b-$f$, c-$g$   
70. a. $y = 5x$ b. $y = 5^x$ c. $y = x^5$   
    ![](../images/Thomas%20Calculus/1-16.jpg)    
    a-$f$, b-$g$, c-$h$    
71. a. Graph the functions $f(x) = \dfrac{x}{2}$ and $g(x) = 1 + \dfrac{4}{x}$ together to identify the values of $x$ for which
    $$
    \dfrac{x}{2} > 1 + \dfrac{4}{x}.
    $$
    b. Confirm your findings in part (a) algebraically.  
    if $x>0$:  
    $x^2 -2x -8 > 0$  
    $(x - 4)(x + 2) > 0$  
    $x < -2$ or $x > 4$ and $x > 0$,$x > 4$  
    if $x>0$:  
    $x^2 -2x -8 < 0$    
    $(x - 4)(x + 2) < 0$    
    $-2 < x < 4$ and $x < 0$,$-2 < x < 0$  
    $\therefore x\in (-2,0) \cup(4,+\infty)$
72. a. Graph the functions $f(x) = \dfrac{3}{x - 1}$ and $g(x) = \dfrac{2}{x + 1}$ together to identify the values of $x$ for which
    $$
    \dfrac{3}{x - 1} > \dfrac{2}{x + 1}.
    $$
    b. Confirm your findings in part (a) algebraically.  
    $\dfrac{3}{x - 1} - \dfrac{2}{x + 1} > 0$  
    $\dfrac{3x + 3 - (2x - 2)}{(x + 1)(x - 1)} > 0$   
    $\dfrac{x + 5}{(x + 1)(x - 1)} > 0$  
    $x\in (-5,-1)\cup(1,+\infty)$
73. For a curve to be symmetric about the $x$-axis, the point $(x, y)$ must lie on the curve if and only if the point $(x, -y)$ lies on the curve. Explain why a curve that is symmetric about the $x$-axis is not the graph of a function, unless the function is $y = 0$.   
    The line $x = x_1,x_1\in D$ will intersect the curve at $(x_1,y)$ and $(x_1,y)$ unless the curve is $y = 0$.  
74. Three hundred books sell for $40 each, resulting in a revenue of (300)($40) = $12,000. For each $5 increase in the price, 25 fewer books are sold. Write the revenue $R$ as a function of the number $x$ of \$5 increases.    
    $R = (40 + 5x)(300 -25x)$    
    $R = -125x^2 + 500x + 12000$
75. A pen in the shape of an isosceles right triangle with legs of length $x$ ft and hypotenuse of length $h$ ft is to be built. If fencing costs $5/ft for the legs and $10/ft for the hypotenuse, write the total cost $C$ of construction as a function of $h$.   
    $C = 10h + 2\dfrac{\sqrt{2}}{2}h$  
    $C = (10 + \sqrt{2})h$
76. **Industrial costs** A power plant sits next to a river where the river is 800 ft wide. To lay a new cable from the plant to a location in the city 2 mi downstream on the opposite side costs $180 per foot across the river and $100 per foot along the land.   
    ![](../images/Thomas%20Calculus/1-17.jpg)  
    a. Suppose that the cable goes from the plant to a point $Q$ on the opposite side that is $x$ ft from the point $P$ directly opposite the plant. Write a function $C(x)$ that gives the cost of laying the cable in terms of the distance $x$.    
    $C(x) = 100(10560-x) + 180\sqrt{x^2 + 800^2}$  
    $C(x) = 180\sqrt{x^2 + 640000} -100x + 1056000$   
    b. Generate a table of values to determine if the least expensive location for point $Q$ is less than 2000 ft or greater than 2000ft from point $P$.
### 1.2 Combining Functions; Shifting and Scaling Graphs
#### Algebraic Combinations
In Exercises 1 and 2, find the domains and ranges of $f$, $g$, $f + g$, and
$f \cdot g$.
1. $f(x) = x, g(x) = 2x - 1$  
   $f\quad D:R\quad R:R$   
   $g\quad D:R\quad R:R$    
   $f + g\quad D:R\quad R:R$   
   $f\cdot g\quad D:R\quad R:R$
2. $f(x) = 2x + 1, g(x) = 2x - 1$
#### Compositions of Functions
5. If $f(x) = x + 5$ and $g(x) = x^2 - 3$, find the following.     
a. $f(g(0))$ b. $g(f(0))$  
c. $f(g(x))$ d. $g(f(x))$  
e. $f(f(-5))$ f. $g(g(2))$  
g. $f(f(x))$ h. $g(g(x))$  
a. $f(g(0)) = g(0) + 5 = -3 + 5 = 2$  
b. $g(f(0)) = f(0)^2 - 3 = 5^2 - 3 = 22$  
c. $f(g(x)) = g(x) + 5 = x^2 - 3 + 5 = x^2 + 2$  
d. $g(f(x)) = f(x)^2 - 3 = (x + 5)^2 - 3 = x^2 + 10x + 22$  
e. $f(f(-2)) = f(-5) + 5 = 0 + 5 = 5$   
f. $g(g(2)) = g(2)^2 - 3 = 2^2 -3 - 3 = -2$   
g. $f(f(x)) = f(x) + 5 = x + 5 + 5 = x + 10$   
h. $g(g(x)) = g(x)^2 - 3 = (x^2 - 3)^2 -3= x^4 -6x^2 + 6$
#### Shifting Graphs
23. The accompanying figure shows the graph of $y = -x^2$ shifted to two new positions. Write equations for the new graphs.    
![](../images/Thomas%20Calculus/1-4.jpg)
a. $y = -(x+7)^2 = -x^2 -14x - 49$  
b. $y = -(x-4)^2 = -x^2 +8x - 16$
#### Vertical and Horizontal Scaling
Exercises 59–68 tell by what factor and direction the graphs of the given functions are to be stretched or compressed. Give an equation
for the stretched or compressed graph.   

59. $y = x^2 - 1$, stretched vertically by a factor of 3     
    $y = 3x^2 -3$
#### graphing
In Exercises 69–76, graph each function, not by plotting points, but by starting with the graph of one of the standard functions presented in Figures 1.14–1.17 and applying an appropriate transformation.  

69. $y = - \sqrt{2x + 1}$
#### Combining Functions
79. Assume that $f$ is an even function, $g$ is an odd function, and both $f$ and $g$ are defined on the entire real line $(-q, q)$. Which of the following (where defined) are even? odd?  
a. $fg$ b. $\dfrac{f}{g}$ c. $\dfrac{g}{f}$   
d. $f^2 = ff$ e. $g^2 = gg$ f. $ƒ \circ g$   
g. $g \circ f$ h. $ƒ \circ ƒ$ i. $g \circ g$   
a. odd b. odd c. odd  
d. even e. even f. even   
g. even h. even i. odd
### 1.3 Trigonometric Functions
#### Radians and Degrees
1. On a circle of radius 10 m, how long is an arc that subtends a central angle of   
   (a) $\dfrac{4\pi}{5}$ radians? (b) $110\degree$?  
   a. $l = r\theta = 10 * \dfrac{4\pi}{5} = 8\pi m$  
   a. $l = \dfrac{\theta}{360}2\pi r= \dfrac{110}{360} * 2 * 10 \pi = \dfrac{55}{9}\pi m$
#### Evaluating Trigonometric Functions
5. Copy and complete the following table of function values. If the function is undefined at a given angle, enter “UND.” Do not use a calculator or tables.  

| $\theta$     | $-\pi$ | $-\dfrac{2}{3}\pi$ |$0$| $\dfrac{1}{2}\pi$ | $\dfrac{3}{4}\pi$ |
| ------------ | ------ | ------------------ | --- | ----------------- | ----------------- |
| $\sin\theta$ |   $0$| $-\dfrac{\sqrt{3}}{2}$|$0$|$1$|$\dfrac{\sqrt{2}}{2}$     |
| $\cos\theta$ |$-1$| $-\dfrac{1}{2}$|$1$|$0$|$\dfrac{\sqrt{2}}{2}$|
| $\tan\theta$ |$0$| $\sqrt{3}$|$0$|$\mathsf{UND}$|$-1$|
| $\cot\theta$ |$\mathsf{UND}$|-$\dfrac{\sqrt{3}}{3}$|$\mathsf{UND}$|$0$|$-1$|
| $\sec\theta$ |$-1$|$-2$|$1$|$\mathsf{UND}$|$\sqrt{2}$|
| $\csc\theta$ |$\mathsf{UND}$|$-\dfrac{2\sqrt{3}}{3}$|$\mathsf{UND}$|$1$|$\sqrt{2}$|
#### Graphing Trigonometric Functions
Graph the functions in Exercises 13–22. What is the period of each function?

13. $\sin 2x$  
    period: $\pi$
#### Using the Addition Formulas
Use the addition formulas to derive the identities in Exercises 31–36.  

31. $\cos(x - \dfrac{\pi}{2}) = \sin x$  
    $\cos(x - \dfrac{\pi}{2})$   
    $= \cos x\cos\dfrac{\pi}{2} + \sin x \sin \dfrac{\pi}{2}$  
    $= \sin x$
#### Using the Half-Angle Formulas
Find the function values in Exercises 47–50.  

47. $\cos^2 \dfrac{\pi}{8}$  
    $\cos^2 \dfrac{\pi}{8}$  
    $= \dfrac{1 + \cos\dfrac{\pi}{4}}{2}$  
    $= \dfrac{1 + \dfrac{\sqrt{2}}{2}}{2}$  
    $= \dfrac{2 + \sqrt{2}}{4}$
#### Solving Trigonometric Equations
For Exercises 51–54, solve for the angle $\theta$, where $0 \le \theta \le 2\pi$.

 51. $\sin^2 \theta = \dfrac{3}{4}$  
     $\sin \theta = \plusmn\dfrac{\sqrt{3}}{2}$  
     $\theta = \plusmn \dfrac{\pi}{3},\plusmn\dfrac{2\pi}{3}$
#### Theory and Examples
55. The tangent sum formula. The standard formula for the tangent of the sum of two angles is
$$
\tan(A + B) = \dfrac{\tan A + \tan B}{1 - \tan A\tan B}.
$$
Derive the formula.  
$\tan(A + B)$  
$= \dfrac{\sin(A + B)}{\cos(A + B)}$  
$= \dfrac{\sin A\cos B + \cos A \sin B}{\cos A\cos B - \sin A \sin B}$  
$= \dfrac{\tan A + \tan B}{1 - \tan A \tan B}$
#### COMPUTER EXPLORATIONS
In Exercises 71–74, you will explore graphically the general sine function
$$
f(x) = A\sin(\dfrac{2\pi}{B}(x - C))+ D
$$
as you change the values of the constants $A$, $B$, $C$, and $D$. Use a CAS or computer grapher to perform the steps in the exercises.

71. The period $B$. Set the constants $A = 3, C = D = 0$.  
a. Plot $f(x)$ for the values $B = 1, 3, 2\pi, 5\pi$ over the interval $-4\pi \le x \le 4\pi$. Describe what happens to the graph of the general sine function as the period increases.  
b. What happens to the graph for negative values of B? Try it with $B = -3 and B = -2\pi$.
### 1.4 Graphing with software
#### Choosing a Viewing Window
In Exercises 1–4, use graphing software to determine which of the given viewing windows displays the most appropriate graph of the specified function.  
1. $f(x) = x^4 - 7x^2 + 6x$  
a. $[-1,1]$ by $[-1,1]$, b. $[-2,2]$ by $[-5,5]$  
c. $[-10,10]$ by $[-10,10]$, d. $[-5,5]$ by $[-25,15]$
#### Finding a Viewing Window
In Exercises 5–30, find an appropriate graphing software viewing window for the given function and use it to display its graph. The window should give a picture of the overall behavior of the function. There is more than one choice, but incorrect choices can miss important aspects of the function.

5. $f(x) = x^4 - 4x^3 + 15$
### Practice exercises
#### Functions and Graphs
1. Express the area and circumference of a circle as functions of the circle’s radius. Then express the area as a function of the circumference.  
   $S = \pi r^2, C = 2\pi r$  
   $r = \dfrac{C}{2\pi}$  
   $S = \pi \dfrac{C^2}{4\pi^2} = \dfrac{C^2}{4\pi}$
#### Piecewise-Defined Functions
In Exercises 35 and 36, find the (a) domain and (b) range.

35. $y = \left\{\begin{aligned} \sqrt{-x}\quad &-4 \le x \le 0 \\ \sqrt{x}\quad&0 < x \le 4\end{aligned}\right.$   
    $D: [-4,4],R:[0,2]$
#### Composition of Functions
In Exercises 39 and 40, find    
a. $(f \circ g)(-1)$. b. $(g \circ f)(2)$.  
c. $(f \circ f)(x)$. d. $(g \circ g)(x)$.  

39. $f(x) =\dfrac{1}{x},g(x) = \dfrac{1}{\sqrt{x + 2}}$  
    a. $(f \circ g)(-1) = \dfrac{1}{g(-1)} = 1$   
    b. $(g \circ f)(2) = \dfrac{1}{\sqrt{f(2) + 2}} = \dfrac{1}{\sqrt{\dfrac{5}{2}}} = \dfrac{2}{\sqrt{10}} = \dfrac{\sqrt{10}}{5}$.    
    c. $(f \circ f)(x) = \dfrac{1}{f(x)} = x$.   
    d. $(g \circ g)(x) = \dfrac{1}{\sqrt{g(x) + 2}} = \dfrac{1}{\sqrt{\dfrac{1}{x + 2}+ 2}} = \dfrac{1}{\sqrt{\dfrac{1 + 2x + 4}{x + 2}}} = \sqrt{\dfrac{x + 2}{2x + 5}} = \dfrac{\sqrt{2x^2 + 9x + 10}}{2x + 5}$.  
#### Shifting and Scaling Graphs
53. Suppose the graph of $g$ is given. Write equations for the graphs that are obtained from the graph of $g$ by shifting, scaling, or reflecting, as indicated.  
a. Up $\dfrac{1}{2}$ unit, right 3  
$g(x - 3) + \dfrac{1}{2}$  
b. Down 2 units, left $\dfrac{2}{3}$   
$g(x + \dfrac{2}{3}) - 2$  
c. Reflect about the $y$-axis  
$g(-x)$   
d. Reflect about the $x$-axis  
$-g(x)$   
e. Stretch vertically by a factor of 5  
$5g(x)$  
f. Compress horizontally by a factor of 5  
$g(5x)$ 
#### Trigonometry
In Exercises 59–62, sketch the graph of the given function. What is the period of the function?

59. $y = \cos 2x$   
    period: $\pi$
### Additional and Advanced Exercises
#### Functions and Graphs
1. Are there two functions $f$ and $g$ such that $f \circ g = g \circ f$? Give reasons for your answer.  
   Yes. $f(x) = x, g(x) = 2x, f \circ g = g \circ f = 2x$
#### Derivations and Proofs
7. Prove the following identities.  
a. $\dfrac{1 - \cos x}{\sin x} = \dfrac{\sin x}{1 + \cos x}$  
b. $\dfrac{1 - \cos x}{1 + \cos x}= \tan^2\dfrac{x}{2}$  
a. $\dfrac{1 - \cos x}{\sin x} - \dfrac{\sin x}{1 + \cos x}$  
$= \dfrac{1 - \cos^2x - \sin^2x}{\sin x + \cos x} = 0$  
$\therefore, \dfrac{1 - \cos x}{\sin x} = \dfrac{\sin x}{1 + \cos x}$  
b. $\dfrac{1 - \cos x}{1 + \cos x}$  
$= \dfrac{\dfrac{1- \cos x}{2}}{\dfrac{1 + \cos x}{2}}$   
$= \dfrac{\sin^2 \dfrac{x}{2}}{\cos^2 \dfrac{x}{2}}$  
$= \tan^2 \dfrac{x}{2}$
#### Effects of Parameters on Graphs
13. What happens to the graph of $y = ax^2 + bx + c$ as   
a. $a$ changes while $b$ and $c$ remain fixed?  
b. $b$ changes ($a$ and $c$ fixed, $a$ ≠ 0)?  
c. $c$ changes ($a$ and $b$ fixed, $a$ ≠ 0)?  
a. The opening of the graph becomes bigger or smaller  
b. The symmetry axis moves left or right, the vertex moves up or down.  
c. The graph moves up or down.
#### Geometry
15. An object’s center of mass moves at a constant velocity $v$ along a straight line past the origin. The accompanying figure shows the coordinate system and the line of motion. The dots show positions that are 1 sec apart. Why are the areas $A_1, A_2, \cdots, A_5$ in the figure all equal? As in Kepler’s equal area law (see Section 13.6), the line that joins the object’s center of mass to the origin sweeps out equal areas in equal times.   
![](../images/Thomas%20Calculus/1-5.jpg)
The distance traveled per second $d = v\Delta t$ is the same.   
The distance from the origin to the line is $h$.   
The area of the triangles: $S = \dfrac{1}{2}v\Delta t h$ remains the same.