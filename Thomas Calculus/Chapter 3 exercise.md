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
### 3.3 Differentiation Rules
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
### 3.4 The Derivative as a Rate of Change
#### Motion Along a Coordinate Line
Exercises 1–6 give the positions $s = f(t)$ of a body moving on a coordinate line, with $s$ in meters and $t$ in seconds.   
a. Find the body’s displacement and average velocity for the given time interval.   
b. Find the body’s speed and acceleration at the endpoints of the interval.  
c. When, if ever, during the interval does the body change direction?
1. $s = t^2 - 3t + 2, 0 \le t \le 2$   
   a.$d = s(2) - s(0) = 4 - 2 = 2m$  
   $v = \dfrac{2}{2} = 1m/s$  
   b. $speed = |f'(t)| = |2t - 3|,a = f''(t) = 2$  
   at $t = 0, speed = 3m/s, a = 2m/s^2$  
   at $t = 2, speed = 1m/s, a = 2m/s^2$  
   c. When $f'(t) = 2t - 3 = 0, t = \dfrac{3}{2}s$, it changes direction. 
#### Free-Fall Applications
9. Free fall on Mars and Jupiter. The equations for free fall at the surfaces of Mars and Jupiter ($s$ in meters, $t$ in seconds) are $s = 1.86t^2$ on Mars and $s = 11.44t^2$ on Jupiter. How long does it take a rock falling from rest to reach a velocity of $27.8 m/sec$ (about $100 km/h$) on each planet?   
    On Mars: When $v = s' = 3.72t = 27.8, t \approx  7.47s$     
    On Jupiter: When $v = s' = 22.88t = 27.8, t \approx  1.22s$
#### Understanding Motion from Graphs
15. The accompanying figure shows the velocity $y = \dfrac{ds}{dt} = f(t)(m/sec)$ of a body moving along a coordinate line  
    a. When does the body reverse direction?   
    b. When (approximately) is the body moving at a constant speed?  
    c. Graph the body’s speed for $0 \le t \le 10$.  
    d. Graph the acceleration, where defined.  
    ![](../images/Thomas%20Calculus/3-9.jpg)  
    a. At $t = 2$ and $t = 7s$  
    b. From $t = 3$ to $t = 6s$
#### Economics
23. Marginal cost. Suppose that the dollar cost of producing $x$ washing machines is $c(x) = 2000 + 100x - 0.1x^2$.   
a. Find the average cost per machine of producing the first 100 washing machines.   
b. Find the marginal cost when 100 washing machines are produced.   
c. Show that the marginal cost when 100 washing machines are produced is approximately the cost of producing one more washing machine after the first 100 have been made, by calculating the latter cost directly.  
a. $a = \dfrac{2000 + 10000 - 1000}{100} = 110$  
b. $m = c'(100) = 100 - 0.2 * 100 = 80$  
c. $c(101) - c(100) = 2000 + 100*101 - 0.1*101^2 -2000 -10000 + 0.1 * 10000 = 10100 -1020.1 - 10000 + 1000 = 79.9$
#### Additional Applications
25. Bacterium population. When a bactericide was added to a nutrient broth in which bacteria were growing, the bacterium population continued to grow for a while, but then stopped growing and began to decline. The size of the population at time $t$ (hours) was $b = 10^6 + 10^4t - 10^3t^2$. Find the growth rates at  
a. $t = 0$ hours.  
b. $t = 5$ hours.  
c. $t = 10$ hours.  
a. $b' = 10^4 - 2*10^3t = 10000-2000t$   
   $r_0 = 10000$    
b. $r_5 = 8000$  
c. $r_{10} = -10000$
#### Analyzing Motion Using Graphs
Exercises 33–36 give the position function $s = f(t)$ of an object moving along the $s$-axis as a function of time $t$. Graph $f$ together with the velocity function $y(t) = \dfrac{ds}{dt} = f′(t)$ and the acceleration function $a(t) = \dfrac{d^2s}{dt^2} = f''(t)$. Comment on the object’s behavior in relation to the signs and values of $y$ and $a$. Include in your commentary such topics as the following:  
a. When is the object momentarily at rest?    
b. When does it move to the left (down) or to the right (up)?      
c. When does it change direction?   
d. When does it speed up and slow down?   
e. When is it moving fastest (highest speed)? Slowest?   
f. When is it farthest from the axis origin?   

33. $s = 200t - 16t^2, 0 \le t \le 12.5$(a heavy object fired straight up from Earth’s surface at 200 ft/sec)  
a. It is never at rest.   
b. Moves up from 0 to 6.25s, and moves down from 6.25 to 12.5 s.  
c. At 6.25s  
d. Slow down from 0 to 6.25s, and speeds up from 6.25 to 12.5 s.  
e. fastest at 0s, Slowest at 6.25s  
f. At 6.25s
### 3.5 Derivatives of Trigonometric Functions
#### Derivatives
In Exercises 1–18, find $\dfrac{dy}{dx}$.
1. $y = -10x + 3 \cos x$   
   $\dfrac{dy}{dx} = -10 - 3 \sin x$
#### Tangent Lines
In Exercises 35–38, graph the curves over the given intervals, together with their tangent lines at the given values of $x$. Label each curve and tangent line with its equation.

35. $y = \sin x, \dfrac{-3\pi}{2} \le x \le 2\pi, x = -\pi, 0, \dfrac{3\pi}{2}$
#### Trigonometric Limits
Find the limits in Exercises 49–56.

49. $\lim\limits_{x\to2}\sin(\dfrac{1}{x}-\dfrac{1}{2})$  
    $\lim\limits_{x\to2}\sin(\dfrac{1}{x}-\dfrac{1}{2}) = \sin0 = 0$
#### Theory and Examples
The equations in Exercises 57 and 58 give the position $s = f(t)$ of a body moving on a coordinate line ($s$ in meters, $t$ in seconds). Find the body’s velocity, speed, acceleration, and jerk at time $t = \dfrac{\pi}{4}$ sec.

57. $s = 2 - 2 \sin t$  
    $v = f'(\dfrac{\pi}{4}) = -2\cos\dfrac{\pi}{4} = -\sqrt{2}m/s$  
    $s =|v| = 2m/s$  
    $a = f''(4) =2\sin\dfrac{\pi}{4} = \sqrt{2} m/s^2$  
    $j = f'''(4) = 2\cos\dfrac{\pi}{4} = \sqrt{2} m/s^2$  
### 3.6 The Chain Rule
#### Derivative Calculations
In Exercises 1–8, given $y = f(u)$ and $u = g(x)$, find $\dfrac{dy}{dx} = f'(g(x))g'(x).$
1. $y = 6u - 9, u = \dfrac{1}{2}x^4$  
   $\dfrac{dy}{dx} = f'(g(x))g'(x) = 6\cdot2x^4 = 12x^3$
#### Second Derivatives
Find $y''$ in Exercises 59–64.

59. $y = (1 + \dfrac{1}{x})^3$  
    $y' = f'(g(x))g'(x)$  
    $=3(1+\dfrac{1}{x})^2\cdot(-x^{-2})$  
    $=-\dfrac{3}{x^2}(1+\dfrac{1}{x})^2$  
    $=-3(\dfrac{1}{x^4}+\dfrac{2}{x^3}+\dfrac{1}{x^2})$  
    $y'' = -3(-4x^{-5}-6x^{-4}-2x^{-3})$   
    $= \dfrac{12}{x^5}+\dfrac{18}{x^4}+\dfrac{6}{x^3}$
#### Finding Derivative Values
In Exercises 67–72, find the value of $(f \circ g)'$ at the given value of $x$.

67. $f(u) = u^5 + 1, u = g(x) = \sqrt{x}, x = 1$  
    $(f \circ g)' = f'(g(x))g'(x) = 5(\sqrt{x})^4\cdot\dfrac{1}{2}x^{-\frac{1}{2}} = \dfrac{5}{2}x^\frac{3}{2}$  
    $(f \circ g)'(1) = \dfrac{5}{2}$
#### Theory and Examples
What happens if you can write a function as a composition in different ways? Do you get the same derivative each time? The Chain Rule says you should. Try it with the functions in Exercises 79 and 80.

79. Find $\dfrac{dy}{dx}$ if $y = x$ by using the Chain Rule with $y$ as a composition of  
a. $y = (\dfrac{u}{5}) + 7$ and $u = 5x - 35$  
b. $y = 1 + (\dfrac{1}{u})$ and $u = \dfrac{1}{x - 1}$.  
a. $y' = \dfrac{1}{5}\cdot5 = 1$  
a. $y' =-(\dfrac{1}{x - 1})^{-2}\dfrac{-1}{(x-1)^2} = 1$
#### COMPUTER EXPLORATIONS
#### Trigonometric Polynomials
100. As the accompanying figure shows, the trigonometric “polynomial”
$$
s = f(t) = 0.78540 - 0.63662 \cos 2t - 0.07074 \cos 6t- 0.02546\cos 10t - 0.01299\cos 14t
$$
gives a good approximation of the sawtooth function $s = g(t)$ on the interval $[-\pi, \pi]$. How well does the derivative of $f$ approximate the derivative of $g$ at the points where $\dfrac{dg}{dt}$ is defined? To find out, carry out the following steps.   
a. Graph $\dfrac{dg}{dt}$ (where defined) over $[-\pi, \pi]$.   
b. Find $\dfrac{df}{dt}$.  
c. Graph $\dfrac{df}{dt}$. Where does the approximation of $\dfrac{dg}{dt}$ by $\dfrac{dg}{dt}$ seem to be best? Least good? Approximations by trigonometric polynomials are important in the theories of heat and oscillation, but we must not expect too much of them, as we see in the next exercise.  
![](../images/Thomas%20Calculus/3-10.jpg)  
b. $\dfrac{df}{dt} = 0.63662\sin2t\cdot2 + 0.07074 \sin 6t\cdot6 + 0.02546\sin 10t\cdot10 + 0.01299\sin 14t\cdot14$   
$=1.27324\sin2t + 0.42444 \sin 6t + 0.2546\sin 10t + 0.181986\sin 14t$
### 3.7 Implicit Differentiation
#### Differentiating Implicitly
Use implicit differentiation to find $\dfrac{dy}{dx}$ in Exercises 1–14.
1. $x^2y + xy^2 = 6$  
   $\dfrac{d}{dx}x^2y + \dfrac{d}{dx}xy^2 = 0$  
   $2x\cdot y+x^2\dfrac{dy}{dx}+y^2+x\cdot2y\dfrac{dy}{dx} = 0$  
   $(x^2 + 2xy)\dfrac{dy}{dx} = -y^2-2xy$    
   $\dfrac{dy}{dx} = \dfrac{y^2+2xy}{x^2 + 2xy}$ 
#### Second Derivatives
In Exercises 19–26, use implicit differentiation to find $\dfrac{dy}{dx}$ and then $\dfrac{d^2y}{dx^2}$ . Write the solutions in terms of $x$ and $y$ only.

19. $x^2 + y^2 = 1$  
    $\dfrac{d}{dx}x^2 + \dfrac{d}{dx}y^2 = 0$  
    $2x + 2y\dfrac{dy}{dx} = 0$  
    $\dfrac{dy}{dx} = -\dfrac{x}{y}$   
    $\dfrac{d^2y}{dx^2} = \dfrac{d}{dx}(-\dfrac{x}{y})$   
    $=-\dfrac{y - x\frac{dy}{dx}}{y^2}$  
    $=-\dfrac{y- \frac{-x^2}{y}}{y^2}$  
    $=-(\dfrac{x^2}{y^3} + \dfrac{1}{y})$  
    $=-\dfrac{x^2 + y^2}{y^3} =-\dfrac{1}{y^3}$  
#### Slopes, Tangents, and Normals
In Exercises 31–40, verify that the given point is on the curve and find the lines that are (a) tangent and (b) normal to the curve at the given point.  

31. $x^2 + xy - y^2 = 1, (2, 3)$    
    $2^2 + 6 - 3^2 = 1$  
    $\dfrac{d}{dx}x^2 + \dfrac{d}{dx}xy - \dfrac{d}{dx}y^2 = 0$  
    $2x + x\dfrac{dy}{dx} + y - 2y\dfrac{dy}{dx} = 0$  
    $\dfrac{dy}{dx} = -\dfrac{2x+y}{x-2y}$  
    tangent line: $y = \dfrac{7}{4}x -\dfrac{1}{2}$  
    normal line: $y = -\dfrac{4}{7}x + \dfrac{29}{7}$
#### Theory and Examples
47. Intersecting normal. The line that is normal to the curve $x^2 +2xy - 3y^2 = 0$ at $(1, 1)$ intersects the curve at what other point?  
    $\dfrac{d}{dx}x^2 +\dfrac{d}{dx}2xy - \dfrac{d}{dx}3y^2 = 0$  
    $2x + 2x\dfrac{dy}{dx} + 2y - 6y\dfrac{dy}{dx} = 0$   
    $\dfrac{dy}{dx} = -\dfrac{x + y}{x - 3y}$  
    $k = 1$  
    normal line :$y = -x + 2$  
    $\left\{\begin{aligned}x^2 +2xy - 3y^2 &= 0 \\ y &= -x + 2\end{aligned}\right.$  
    $x^2 -2x^2 +4x - 3(4-4x + x^2) = 0$  
    $-4x^2 + 16x -12 = 0$  
    $x^2 -4x + 3 = 0$   
    $x_1 = 1, x_2 = 3$  
    The other point is $(3,-1)$
#### COMPUTER EXPLORATIONS
Use a CAS to perform the following steps in Exercises 55–62.  
a. Plot the equation with the implicit plotter of a CAS. Check to see that the given point $P$ satisfies the equation.  
b. Using implicit differentiation, find a formula for the derivative $\dfrac{dy}{dx}$ and evaluate it at the given point $P$.  
c. Use the slope found in part (b) to find an equation for the tangent line to the curve at $P$. Then plot the implicit curve and tangent line together on a single graph.

55. $x^3 - xy + y^3 = 7, P(2, 1)$  
    b. $\dfrac{d}{dx}x^3 -\dfrac{d}{dx}xy + \dfrac{d}{dx}y^3 = 0$  
    $3x^2 - x\dfrac{dy}{dx} -y +3y^2\dfrac{dy}{dx} = 0$  
    $\dfrac{dy}{dx} = \dfrac{y-3x^2}{3y^2 - x}$  
    tangent line : $y =-11x + 23$
### 3.8 Related Rates
1. Area. Suppose that the radius $r$ and area $A = \pi r^2$ of a circle are differentiable functions of $t$. Write an equation that relates $\dfrac{dA}{dt}$ to $\dfrac{dr}{dt}$.  
   $\dfrac{dA}{dt} = \dfrac{d}{dt}\pi r^2$  
   $=2r\pi\dfrac{dr}{dt}$
### 3.9 Linearization and Differentials
#### Finding Linearizations
In Exercises 1–5, find the linearization $L(x)$ of $f(x)$ at $x = a$.
1. $f(x) = x^3 - 2x + 3, a = 2$  
   $f'(x) = 3x^2 -2, f'(2) = 10$  
   $L(x) = 10x -13$
#### Linearization for Approximation
In Exercises 7–12, find a linearization at a suitably chosen integer near $a$ at which the given function and its derivative are easy to evaluate.  

7. $f(x) = x^2 + 2x, a = 0.1$  
   $f'(x) = 2x + 2, f'(0) = 2$  
   $L(x) = 2x -2$
#### Derivatives in Differential Form
In Exercises 17–28, find $dy$.

17. $y = x^3 - 3\sqrt{x}$  
    $dy = 3x^2 -\dfrac{3}{2}x^{-\frac{1}{2}}$  
    $=3x^2 - \dfrac{3}{2\sqrt{x}}$  
    $=\dfrac{6x^2\sqrt{x}-3}{2\sqrt{x}}$  
    $=\dfrac{6x^3-3\sqrt{x}}{2x}$  
#### Approximation Error
In Exercises 29–34, each function $f(x)$ changes value when $x$ changes from $x0$ to $x_0 + dx$. Find  
a. the change $\Delta f = f(x_0 + dx) - f(x_0);$  
b. the value of the estimate $df = f'(x_0) dx$; and  
c. the approximation error $|\Delta f - df |$ .   
![](../images/Thomas%20Calculus/3-11.jpg)   
29. $f(x) = x^2 + 2x, x_0 = 1, dx = 0.1$  
    a.$\Delta f = f(1.1) - f(1) = 1.1^2 + 2.2 -1-2 = 0.41$  
    b. $f'(x) = 2x + 2$  
    $df = f'(x_0) dx = 4\cdot 0.1 = 0.4$  
    c.  $|\Delta f - df | = 0.01$
#### Differential Estimates of Change
In Exercises 35–40, write a differential formula that estimates the given change in volume or surface area.

35. The change in the volume $V = \dfrac{4}{3}\pi r^3$ of a sphere when the radius changes from $r_0$ to $r_0 + dr$  
    $dV = f'(r_0)dr = 4\pi r^2dr$
#### Applications
41. The radius of a circle is increased from 2.00 to 2.02 m.    
a. Estimate the resulting change in area.  
b. Express the estimate as a percentage of the circle’s original area.  
    a. $A = 4\pi r^2,A' = 8\pi r$  
    $dA = f'(2)dr = 16\pi \cdot 0.02 = 0.32\pi$  
    b. $\dfrac{0.32\pi}{16\pi} = 2\%$
#### COMPUTER EXPLORATIONS
In Exercises 57–60, use a CAS to estimate the magnitude of the error in using the linearization in place of the function over a specified interval $I$. Perform the following steps:  
a. Plot the function $f$ over $I$.  
b. Find the linearization $L$ of the function at the point $a$.    
c. Plot $f$ and $L$ together on a single graph.    
d. Plot the absolute error $| f(x) - L(x)|$ over $I$ and find its maximum value.  
e. From your graph in part (d), estimate as large a $\delta > 0$ as you can, satisfying
$$
| x - a| < \delta \rArr | f(x) - L(x)| < \varepsilon
$$
for $\varepsilon = 0.5, 0.1$, and 0.01. Then check graphically to see if your $\delta$-estimate holds true.

57. $f(x) = x^3 + x^2 - 2x, [-1, 2], a = 1$   
    b. $f'(x) = 3x^2 + 3x -2, f'(1) = 4$   
    $L = 4x - 4$  
    c. $\max | f(x) - L(x)| = |f(-1) - L(-1) |=10$
### Practice exercise
#### Derivatives of Functions
Find the derivatives of the functions in Exercises 1–40.
1. $y = x^5 - 0.125x^2 + 0.25x$  
   $y' = 5x^4 - 0.25x + 0.25$
#### Implicit Differentiation
In Exercises 41–48, ind dy>dx by implicit differentiation.

41. $xy + 2x + 3y = 1$  
    $\dfrac{d}{dx}xy + \dfrac{d}{dx}2x + \dfrac{d}{dx}3y =0$  
    $x\dfrac{dy}{dx} + y + 2 + 3\dfrac{dy}{dx} =0$  
    $\dfrac{dy}{dx} = - \dfrac{y + 2}{x + 3}$
#### Numerical Values of Derivatives
55. Suppose that functions $f(x)$ and $g(x)$ and their first derivatives have the following values at $x = 0$ and $x = 1$.  

|  $x$  | $f(x)$ | $g(x)$ |    $f'(x)$     |    $g'(x)$     |
| :---: | :----: | :----: | :------------: | :------------: |
|   0   |   1    |   1    |       -3       | $\dfrac{1}{2}$ |
|   1   |   3    |   5    | $\dfrac{1}{2}$ |       -4       |
Find the first derivatives of the following combinations at the given value of $x$.
a. $6f(x) - g(x), x = 1$ b. $f(x)g^2(x), x = 0$  
c.$\dfrac{f(x)}{g(x) + 1}, x = 1$ d. $f(g(x)), x = 0$  
e. $g(f(x)), x = 0$ f. $(x + f(x))^\frac{3}{2}, x = 1$  
g. $f(x + g(x)), x = 0$  
a. $\dfrac{d}{dx}(6f(1) - g(1))= 6f'(1) -g'(1)= 7$    
b. $\dfrac{d}{dx}(f(0)g^2(0)) = f'(0)g^2(0) + f(0)\dfrac{d}{dx}g^2(0) =-3+2g'(0)g'(0) = -\dfrac{5}{2}$  
c.$\dfrac{d}{dx}\dfrac{f(1)}{g(1) + 1} = \dfrac{(g(1) + 1)f'(1)+f(1)g'(1)}{(g'(1)+1)^2} = \dfrac{6- 4}{9} = \dfrac{2}{9}$  
d. $\dfrac{d}{dx}f(g(0)) =f'(g(0))g'(0)= \dfrac{1}{2}f'(1) = \dfrac{3}{2}$  
e. $\dfrac{d}{dx}g(f(0)) = g'(f(0))f'(0) = -3g'(1) = 12$  
f. $\dfrac{d}{dx}(1 + f(1))^\frac{3}{2}=\dfrac{3}{2}\sqrt{1+3}f'(1) = \dfrac{3}{2}$   
g. $\dfrac{d}{dx}f(0 + g(0))= f'(1)g'(0) = \dfrac{1}{4}$  
#### applying the Derivative Definition
In Exercises 63 and 64, ind the derivative using the definition.

63. $f(t) = \dfrac{1}{2t + 1}$  
    $f'(t) = \lim\limits_{h\to0}\dfrac{f(t+h)-f(t)}{h}$    
    $= \lim\limits_{h\to0}\dfrac{\frac{1}{2t+2h+1}-\frac{1}{2t+1}}{h}$   
    $= \lim\limits_{h\to0}\dfrac{2t+1-2t-2h-1}{(2t+2h+1)(2t+1)}\dfrac{1}{h}$  
    $= \lim\limits_{h\to0}\dfrac{-2}{(2t+2h+1)(2t+1)}$   
    $= -\dfrac{2}{4t^2+4t+1}$
#### Slopes, Tangents, and Normals
69. Tangent lines with specified slope. Are there any points on the curve $y =\dfrac{x}{2} + \dfrac{1}{2x - 4}$ where the slope is $-\dfrac{3}{2}$? If so, find them.  
    $y' = \dfrac{1}{2} - \dfrac{2}{(2x-4)^2} = -\dfrac{3}{2}$  
    $(2x-4)^2 = 1$  
    $2x = 4 \plusmn 1, x_1 = \dfrac{5}{2},x_2 = \dfrac{3}{2}$  
    $P_1(\dfrac{5}{2},\dfrac{9}{4}),P_2(\dfrac{3}{2},-\dfrac{1}{4})$
#### Analyzing Graphs
Each of the figures in Exercises 89 and 90 shows two graphs, the graph of a function $y = f(x)$ together with the graph of its derivative $f'(x)$. Which graph is which? How do you know?

89. ![](../images/Thomas%20Calculus/3-12.jpg)  
    $A: f'(x),B:f(x)$
#### Trigonometric Limits
Find the limits in Exercises 95–102.

95. $\lim\limits_{x\to0}\dfrac{\sin x}{2x^2 - x}$  
    $\lim\limits_{x\to0}\dfrac{\sin x}{2x^2 - x} = \lim\limits_{x\to0}\dfrac{\sin x}{x(2x-1)} = \lim\limits_{x\to0}\dfrac{1}{2x-1} = -1$
#### Related Rates
105. Right circular cylinder. The total surface area $S$ of a right circular cylinder is related to the base radius $r$ and height $h$ by the equation $S = 2\pi r^2 + 2\pi rh$.  
a. How is $\dfrac{dS}{dt}$ related to $\dfrac{dr}{dt}$ if $h$ is constant?  
b. How is $\dfrac{dS}{dt}$ related to $\dfrac{dh}{dt}$ if $r$ is constant?  
c. How is $\dfrac{dS}{dt}$ related to $\dfrac{dr}{dt}$ and $\dfrac{dh}{dt}$ if neither $r$ nor $h$ is constant?   
d. How is $\dfrac{dr}{dt}$ related to $\dfrac{dh}{dt}$ if $S$ is constant?  
a. $\dfrac{dS}{dt} = \dfrac{d}{dt}2\pi r^2 + \dfrac{d}{dt}2\pi rh = 4\pi r \dfrac{dr}{dt} +2\pi h \dfrac{dr}{dt}$  
b. $\dfrac{dS}{dt} = \dfrac{d}{dt}2\pi r^2 + \dfrac{d}{dt}2\pi rh =2\pi r\dfrac{dh}{dt}$  
c. $\dfrac{dS}{dt} = \dfrac{d}{dt}2\pi r^2 + \dfrac{d}{dt}2\pi rh = 4\pi r \dfrac{dr}{dt} +2\pi(r\dfrac{dh}{dt} + h\dfrac{dr}{dt}) = (4\pi r + h)\dfrac{dr}{dt} + 2\pi r \dfrac{dh}{dt}$  
d. $0 = \dfrac{d}{dt}2\pi r^2 + \dfrac{d}{dt}2\pi rh$  
   $(4\pi r + h)\dfrac{dr}{dt} + 2\pi r \dfrac{dh}{dt} = 0$  
   $\dfrac{dr}{dt} = -\dfrac{2\pi r}{4\pi r + h}\dfrac{dh}{dt}$
#### Linearization
117. Find the linearizations of  
a. $\tan x$ at $x = -\dfrac{\pi}{4}$ b. $\sec x$ at $x = -\dfrac{\pi}{4}$.  
Graph the curves and linearizations together  
    a. $\dfrac{d}{dx}\tan x = \sec^2 x$  
    $L = 2x + \dfrac{\pi}{2} -1$  
    b. $\dfrac{d}{dx}\sec x = \sec x \tan x$  
    $L = -\sqrt{2}x - \dfrac{\sqrt{2}\pi}{4} + \sqrt{2}$
#### Diferential Estimates of Change
121. Surface area of a cone. Write a formula that estimates the change that occurs in the lateral surface area of a right circular cone when the height changes from $h_0$ to $h_0 + dh$ and the radius does not change.
    ![](../images/Thomas%20Calculus/3-13.jpg)   
    $dS = \dfrac{dS}{dh}(h_0)dh = \pi r\dfrac{d}{dh}\sqrt{r^2+h_0^2}dh =\dfrac{1}{2}\pi rdh\dfrac{1}{r^2+h_0^2}2h_0 = \dfrac{\pi r h_0}{r^2+h_0^2}dh$
#### Additional and Advanced Exercises
1. An equation like $\sin^2\theta + \cos^2\theta = 1$ is called an identity because it holds for all values of $\theta$. An equation like $\sin\theta = 0.5$ is not an identity because it holds only for selected values of $\theta$, not all. If you differentiate both sides of a trigonometric identity in $\theta$ with
respect to $\theta$, the resulting new equation will also be an identity.   
Differentiate the following to show that the resulting equations hold for all $\theta$.  
a. $\sin 2\theta = 2 \sin \theta \cos \theta$  
b. $\cos2\theta = \cos^2 \theta - \sin^2 \theta$   
a. $\dfrac{d}{d\theta}\sin 2\theta = 2\cos 2\theta$  
   $\dfrac{d}{d\theta}2 \sin \theta \cos \theta=2(-\sin^2\theta + \cos^2\theta) = 2\cos 2\theta$  
b. $\dfrac{d}{d\theta}\cos2\theta = -2\sin2\theta$  
   $\dfrac{d}{d\theta}(\cos^2 \theta - \sin^2 \theta) =-2\cos\theta\sin\theta-2\sin\theta\cos\theta = -2\sin2\theta$
