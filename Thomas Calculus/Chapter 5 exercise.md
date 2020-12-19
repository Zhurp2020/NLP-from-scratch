# Thomas Calculus
## Chapter 5 Integrals
### 5.1 Area and Estimating with Finite Sums
#### Area
In Exercises 1–4, use finite approximations to estimate the area under the graph of the function using  
a. a lower sum with two rectangles of equal width.  
b. a lower sum with four rectangles of equal width.  
c. an upper sum with two rectangles of equal width.  
d. an upper sum with four rectangles of equal width.   
1. $f(x) = x^2$ between $x = 0$ and $x = 1$  
   a. $S > \dfrac{1}{2}(f(0) + f(\dfrac{1}{2}) = \dfrac{1}{8}$  
   b. $S > \dfrac{1}{4}(f(0) + f(\dfrac{1}{4})+f(\dfrac{1}{2}) + f(\dfrac{3}{4})) = \dfrac{9}{32}$  
   c. $S < \dfrac{1}{2}(f(\dfrac{1}{2} + f(1)) = \dfrac{5}{8}$  
   c. $S < \dfrac{1}{4}(f(\dfrac{1}{4})+f(\dfrac{1}{2}) + f(\dfrac{3}{4}) + f(1)) = \dfrac{17}{32}$
#### Distance
9. Distance traveled. The accompanying table shows the velocity of a model train engine moving along a track for 10 sec. Estimate the distance traveled by the engine using 10 subintervals of length 1 with  
a. left-endpoint values.  
b. right-endpoint values  

| Time(sec) | Velocity(cm/sec) | Time(sec) | Velocity(cm/sec) |
| :-------: | :--------------: | :-------: | :--------------: |
|     0     |        0         |     6     |        28        |
|     1     |        30        |     7     |        15        |
|     2     |        56        |     8     |        5         |
|     3     |        25        |     9     |        15        |
|     4     |        38        |    10     |        0         |
|     5     |        33        |
 a. $d = 245$    
 b. $d = 245$ 
#### Average Value of a Function
In Exercises 15–18, use a finite sum to estimate the average value of $f$ on the given interval by partitioning the interval into four subintervals of equal length and evaluating $f$ at the subinterval midpoints.

15. $f(x) = x^3$ on $[0, 2]$  
    $S = \dfrac{1}{2}(f(\dfrac{1}{4}) + f(\dfrac{3}{4}) + f(\dfrac{5}{4}) +f(\dfrac{7}{4})) = \dfrac{31}{8}$  
#### Examples of Estimations
19. Water pollution. Oil is leaking out of a tanker damaged at sea. The damage to the tanker is worsening as evidenced by the increased leakage each hour, recorded in the following table.  
     
| Time(h) | Leakage (gal/h) | Time(h) | Leakage (gal/h) |
| :-----: | :-------------: | :-----: | :-------------: |
|    0    |       50        |    5    |       265       |
|    1    |       70        |    6    |       369       |
|    2    |       90        |    7    |       516       |
|    3    |       136       |    8    |       720       |
|    4    |       190       |         |
a. Give an upper and a lower estimate of the total quantity of oil that has escaped after 5 hours.  
b. Repeat part (a) for the quantity of oil that has escaped after 8 hours.  
c. The tanker continues to leak 720 gal/h after the first 8 hours. If the tanker originally contained 25,000 gal of oil, approximately how many more hours will elapse in the worst case before all the oil has spilled? In the best case?  
a. $536< Q < 751$  
b. $2253 <Q < 2357$   
c. $31.45< t < 31.59$
#### COMPUTER EXPLORATIONS
In Exercises 23–26, use a CAS to perform the following steps.  
a. Plot the functions over the given interval.   
b. Subdivide the interval into $n = 100, 200,$ and $1000$ subintervals of equal length and evaluate the function at the midpoint of each subinterval.  
c. Compute the average value of the function values generated in part (b).  
d. Solve the equation $f(x) =$ (average value) for $x$ using the average value calculated in part (c) for the $n = 1000$ partitioning.

23.  $f(x) = \sin x$ on $[0,\pi]$
### 5.2 Sigma Notation and Limits of Finite Sums
#### Sigma Notation
Write the sums in Exercises 1–6 without sigma notation. Then evaluate them.
1. $\sum\limits_{k=1}^2\dfrac{6k}{k + 1}$   
   $\sum\limits_{k=1}^2\dfrac{6k}{k + 1} = 3 + 4 =7$
#### Values of Finite Sums
17. Suppose that $\sum\limits_{k=1}^na_k = -5$ and $\sum\limits_{k=1}^nb_k = 6$. Find the values of  
    a. $\sum\limits_{k=1}^n3a_k$  b. $\sum\limits_{k=1}^n\dfrac{b_k}{6}$ c. $\sum\limits_{k=1}^n(a_k + b_k)$   
    d. $\sum\limits_{k=1}^n(a_k - b_k)$ e. $\sum\limits_{k=1}^n( b_k-2a_k )$   
    a. $\sum\limits_{k=1}^n3a_k = -15$    
    b. $\sum\limits_{k=1}^n\dfrac{b_k}{6}=1$   
    c. $\sum\limits_{k=1}^n(a_k + b_k) = 1$     
    d. $\sum\limits_{k=1}^n(a_k - b_k) = -11$    
    e. $\sum\limits_{k=1}^n( b_k-2a_k ) = 16$  
#### Riemann Sums
In Exercises 37–42, graph each function $f(x)$ over the given interval. Partition the interval into four subintervals of equal length. Then add to your sketch the rectangles associated with the Riemann sum $\sum\limits_{k=1}^4f(c_k)\Delta x_k$ , given that $c_k$
is the (a) left-hand endpoint, (b) righthand endpoint, (c) midpoint of the $k$th subinterval. (Make a separate sketch for each set of rectangles.)

37.  $f(x) = x^2 - 1, [0, 2]$
#### Limits of Riemann Sums
For the functions in Exercises 43–50, find a formula for the Riemann sum obtained by dividing the interval $[a, b]$ into $n$ equal subintervals and using the right-hand endpoint for each $c_k$. Then take a limit of these sums as $n \to\infty$ to calculate the area under the curve over $[a, b]$ .

43.  $f(x) = 1 - x^2$ over the interval $[0, 1]$ .   
     $S = \sum\limits_{k = 1}^nf(c_k)\Delta x_k$   
     $= \sum\limits_{k = 1}^n(1-c_k^2)\dfrac{1}{n}$  
     $= \sum\limits_{k = 1}^n(1-(\dfrac{k}{n})^2)\dfrac{1}{n}$  
     $= \sum\limits_{k = 1}^n\dfrac{1}{n} - \dfrac{k^2}{n^3}$  
     $= 1 - \dfrac{1}{n^3}\sum\limits_{k = 1}^nk^2$  
     $= 1-\dfrac{1}{n^3}\dfrac{n(n + 1)(2n + 1)}{6}$    
     $\lim\limits_{n\to\infty}S = 1-\dfrac{1}{3} = \dfrac{2}{3}$
### 5.3 The Definite Integral
#### Interpreting Limits of Sums as Integrals
Express the limits in Exercises 1–8 as definite integrals
1. $\lim\limits_{||P||\to0}\sum\limits_{k=1}^nc_k^2\Delta x_k$, where $P$ is a partition of $[0, 2]$  
   $\int_0^2x^2dx$
#### Using the Definite Integral Rules
9. Suppose that $f$ and $g$ are integrable and that
   $$
   \int_1^2 f(x) dx = -4, \\
   \int_1^5 f(x) dx = 6, \\  
   \int_1^5 g(x) dx = 8, \\
   $$
   Use the rules in Table 5.6 to find   
   a. $\int_2^2 g(x) dx$ b. $\int_5^1 g(x) dx$  
   c. $\int_1^2 3f(x) dx$ d. $\int_2^5 f(x) dx$  
   e. $\int_1^5 [f(x) - g(x)] dx$ f. $\int_1^5 [4f(x) - g(x)] dx$   
   a. $\int_2^2 g(x) dx = 0$    
   b. $\int_5^1 g(x) dx = -6$  
   c. $\int_1^2 3f(x) d = -12x$   
   d. $\int_2^5 f(x) dx = 10$     
   e. $\int_1^5 [f(x) - g(x)] dx = -2$   
   f. $\int_1^5 [4f(x) - g(x)] dx = 16$ 
#### Using Known Areas to Find Integrals
In Exercises 15–22, graph the integrands and use known area formulas to evaluate the integrals.

15. $\int_{-2}^4 (\dfrac{x}{2} + 3)dx$  
    $S = \dfrac{1}{2}(5 + 2)\cdot6 = 21$
#### Evaluating Definite Integrals
Use the results of Equations (2) and (4) to evaluate the integrals in Exercises 29–40.

29. $\int_1^{\sqrt{2}} xdx$  
    $S = \dfrac{2}{2} - \dfrac{1}{2} = \dfrac{1}{2}$  
#### Finding Area by Definite Integrals
In Exercises 51–54, use a definite integral to find the area of the region between the given curve and the $x$-axis on the interval $[0, b]$ .

51. $y = 3x^2$  
    $S = \int_0^b3x^2dx = 3\dfrac{b^3}{3} =  b^3$
#### Finding Average Value
In Exercises 55–62, graph the function and find its average value over the given interval.

55. $f(x) = x^2 - 1$ on $[0,\sqrt{3}]$  
    $a = \dfrac{\int_0^{\sqrt{3}}(x^2 - 1)dx}{\sqrt{3}} = \dfrac{\frac{3\sqrt{3}}{3} - \sqrt{3}}{\sqrt{3}} =0$
### 5.4 The Fundamental Theorem of Calculus
#### Evaluating Integrals
Evaluate the integrals in Exercises 1–28.
1. $\int_2^0x(x - 3) dx$  
   $\int_2^0x(x - 3) dx = -\int_0^2x(x - 3) dx = -[\dfrac{1}{3}x^3 - \dfrac{3}{2}x^2]_0^2 = \dfrac{10}{3}$
#### Derivatives of Integrals
Find the derivatives in Exercises 33–38.  
a. by evaluating the integral and differentiating the result.  
b. by differentiating the integral directly.

33. $\dfrac{d}{dx} \int_0^{\sqrt{x}} \cos t dt$  
    a. $\dfrac{d}{dx} \int_0^{\sqrt{x}} \cos t dt = \dfrac{d}{dx}[\sin t]_0^{\sqrt{x}} = \dfrac{d}{dx}\sin \sqrt{x} = \dfrac{\cos\sqrt{x}}{2\sqrt{x}}$   
    b. $\dfrac{d}{dx} \int_0^{\sqrt{x}} \cos t dt = \dfrac{d}{dx}\int_0^u\cos tdt\cdot\dfrac{d}{dx}\sqrt{x} = \dfrac{\cos \sqrt{x}}{2\sqrt{x}}$
#### Area
In Exercises 47–50, find the total area between the region and the $x$-axis.

47. $y = -x^2 - 2x, -3 \le x \le 2$  
    $x^2 + 2x = 0, x_1 = 0, x_2 = -2$   
    $S = |\int_{-3}^{-2}(-x^2 - 2x)| + |\int_{-2}^{0}(-x^2 - 2x)| + |\int_{0}^{2}(-x^2 - 2x)|$  
    $= |[-\dfrac{1}{3}x^3 - x^2]_{-3}^{-2}| + |[-\dfrac{1}{3}x^3 - x^2]_{-2}^{0}| + |[-\dfrac{1}{3}x^3 - x^2]_{0}^{2}|$  
    $= |-\dfrac{4}{3}| + |-\dfrac{4}{3}| + |-\dfrac{20}{3}|$  
    $= \dfrac{28}{3}$
#### Initial Value Problems
Each of the following functions solves one of the initial value problems in Exercises 55–58. Which function solves which problem? Give brief reasons for your answers.  
a. $y =\int_1^x\dfrac{1}{t}dt - 3$ b. $y =\int_0^x\sec tdt + 4$  
c. $y =\int_{-1}^x\sec tdt + 4$ d. $y =\int_\pi^x\dfrac{1}{t}dt - 3$

55. $\dfrac{dy}{dx} =\dfrac{1}{x}, y(\pi) = -3$  
    d. 
#### Theory and Examples
61. Archimedes’ area formula for parabolic arches.Archimedes(287–212 b.c.), inventor, military engineer, physicist, and the greatest mathematician of classical times in the Western world, discovered that the area under a parabolic arch is two-thirds the base times the height. Sketch the parabolic arch $y = h - (\dfrac{4h}{b^2})x^2,-\dfrac{b}{2} \le x \le \dfrac{b}{2}$, assuming that $h$ and $b$ are positive. Then use calculus to find the area of the region enclosed between the arch and the $x$-axis   
    zeros:$-\dfrac{b}{2},\dfrac{b}{2}$    
    $S = \int_{-\frac{b}{2}}^{\frac{b}{2}}h - (\dfrac{4h}{b^2})x^2dx = [hx - \dfrac{4h}{3b^2}x^3]_{-\frac{b}{2}}^{\frac{b}{2}} = \dfrac{hb}{2} - \dfrac{4h}{3b^2}\dfrac{b^3}{8} - (-\dfrac{hb}{2}+ \dfrac{4h}{3b^2}\dfrac{b^3}{8}) = hb -\dfrac{hb}{3} = \dfrac{2}{3}hb$
#### COMPUTER EXPLORATIONS
In Exercises 75–78, let $F(x) = \int^x_af(t) dt$ for the specified function $f$ and interval $[a, b]$ . Use a CAS to perform the following steps and answer the questions posed.    
a. Plot the functions $f$ and $F$ together over $[a, b]$.  
b. Solve the equation $F'(x) = 0$. What can you see to be true about the graphs of $f$ and $F$ at points where $F'(x) = 0$? Is your observation borne out by Part 1 of the Fundamental Theorem coupled with information provided by the first derivative? Explain your answer.   
c. Over what intervals (approximately) is the function $F$ increasing and decreasing? What is true about $f$ over those intervals?   
d. Calculate the derivative $f'$ and plot it together with $F$. What can you see to be true about the graph of $F$ at points where $f'(x) = 0$? Is your observation borne out by Part 1 of the Fundamental Theorem? Explain your answer.

75. $f(x) = x^3 - 4x^2 + 3x, [0, 4]$   
    a. $F(x) = \int_0^x t^3 - 4t^2 + 3tdt =[\dfrac{1}{4}t^4 -\dfrac{4}{3}t^3 + \dfrac{3}{2}t^2]_0^x = \dfrac{1}{4}x^4 -\dfrac{4}{3}x^3 + \dfrac{3}{2}x^2$   
    b. $F'(x) = x^3 - 4x^2 + 3x = 0$  
    $x(x^2-4x+3) = 0$  
    $x_1 = 0, x_2 = 3, x_3 = 1$  
    c. Increasing:$[0,1],[3,\infty)$  
    Decreasing:$(1,3)$   
    d.$f'(x) = 3x^2 -8x + 3$
### 5.5 Indefinite Integrals and the Substitution Method
#### Evaluating Indefinite Integrals
Evaluate the indefinite integrals in Exercises 1–16 by using the given substitutions to reduce the integrals to standard form.
1. $\int2(2x + 4)^5 dx, u = 2x + 4$  
   $\dfrac{du}{dx} = 2, du = 2dx$    
   $\int2(2x + 4)^5 dx = \int u^5du = \dfrac{1}{6}u^6 + C= \dfrac{1}{6}(2x + 4)^6 + C$    
#### Initial Value Problems
Solve the initial value problems in Exercises 55–60.

55. $\dfrac{ds}{dt}= 12t (3t^2 - 1)^3, s(1) = 3$  
    $s = \int12t (3t^2 - 1)^3dt$  
    $u = 3t^2 - 1\dfrac{du}{dt} = 6t, 12tdt = 2du$   
    $s = \int 2u^3du = \dfrac{1}{2}u^4 + C= \dfrac{1}{2}(3t^2 - 1)^4+ C$  
    $s(1) = C = 3$  
    $s = \dfrac{1}{2}(3t^2 - 1)^4+3$
### 5.6 Definite Integral Substitutions and the Area Between Curves
#### Evaluating Definite Integrals
Use the Substitution Formula in Theorem 7 to evaluate the integrals in Exercises 1–24.

1. a. $\int^3_0\sqrt{y + 1} dy$  b. $\int^0_{-1}\sqrt{y + 1} dy$   
   a. $u = y + 1,\dfrac{du}{dy} =1,du = dy$  
   $\int^3_0\sqrt{y + 1} dy = \int_1^4\sqrt{u}du = [\dfrac{2}{3}u^{\frac{3}{2}}]_1^4 = \dfrac{16}{3} - \dfrac{2}{3} = \dfrac{14}{3}$  
   b. $\int^0_{-1}\sqrt{y + 1} dy = \int^1_0\sqrt{u}du = [\dfrac{2}{3}u^{\frac{3}{2}}]^1_0 = \dfrac{2}{3}$
#### Area
Find the total areas of the shaded regions in Exercises 25–40

25. ![](../images/Thomas%20Calculus/5-1.jpg)    
    $y$ is an odd function  
    $S = 2|\int_0^2x\sqrt{4-x^2}dx|$  
    $u = 4 - x^2, \dfrac{du}{dx} =-2x, du = -2xdx$  
    $S = 2 |\int_0^4-\dfrac{1}{2}\sqrt{u}du|$  
    $= 2|[\dfrac{1}{3}u^{\frac{3}{2}}]_0^4|=\dfrac{16}{3}$
#### Area Between Curves
71. Find the area of the propeller-shaped region enclosed by the curve $x - y^3 = 0$ and the line $x - y = 0.$   
    $y^3 = y, y(y^2 - 1) = 0, y_1 = 0, y_2 = -1, y_3 = 1$   
    $S = 2\int_0^1(y-y^3)dy = 2[\dfrac{1}{2}y^2-\dfrac{1}{4}y^4]_0^1 = \dfrac{1}{2}$
#### Theory and Examples
83. Suppose that $F(x)$ is an antiderivative of $f(x) = \dfrac{\sin x}{x}, x > 0.$Express
    $$
    \int^3_1\dfrac{\sin 2x}{x}dx
    $$
    in terms of $F$  
    $u = 2x,\dfrac{du}{dx} = 2$   
    $\int^3_1\dfrac{\sin 2x}{x}dx = \int^6_2\dfrac{\sin u}{\frac{u}{2}}dx = \int^6_22\dfrac{\sin u}{u}dx= \int^6_2\dfrac{\sin u}{u}du$  
    $F'(u) = \dfrac{\sin u}{u}$  
    $\int^3_1\dfrac{\sin 2x}{x}dx= \int^6_2Fdu = F(6)-F(2)$
### COMPUTER EXPLORATIONS
In Exercises 91–94, you will find the area between curves in the plane when you cannot find their points of intersection using simple algebra. Use a CAS to perform the following steps:   
a. Plot the curves together to see what they look like and how many points of intersection they have.   
b. Use the numerical equation solver in your CAS to ind all the points of intersection.
c. Integrate $|f(x) - g(x)|$ over consecutive pairs of intersection values.   
d. Sum together the integrals found in part (c)   

91. $f(x) = \dfrac{x^3}{3}-\dfrac{x^2}{2}-2x+\dfrac{1}{3},g(x) = x - 1$    
    $|f(x) - g(x)| = |\dfrac{x^3}{3}-\dfrac{x^2}{2}-3x+\dfrac{4}{3}|$  
    $S = |\int_{-2.6}^{0.4}\dfrac{x^3}{3}-\dfrac{x^2}{2}-3x+\dfrac{4}{3}dx| + |\int_{0.4}^{3.6}\dfrac{x^3}{3}-\dfrac{x^2}{2}-3x+\dfrac{4}{3}dx|$  
    Let $F(x) = \dfrac{1}{12}x^4-\dfrac{1}{6}x^3-\dfrac{3}{2}x^2 + \dfrac{4}{3}x$  
    $S = F(0.4)-F(-2.6)+F(0.4)-F(3.6)$  
    $\approx 15.8$
### Practice Exercises
#### Finite Sums and Estimates
1. The accompanying figure shows the graph of the velocity (ft/sec) of a model rocket for the first 8 sec after launch. The rocket accelerated straight up for the first 2 sec and then coasted to reach its maximum height at t = 8 sec.  
   ![](../images/Thomas%20Calculus/5-2.jpg)  
a. Assuming that the rocket was launched from ground level, about how high did it go? (This is the rocket in Section 3.4, Exercise 17, but you do not need to do Exercise 17 to do the exercise here.)   
b. Sketch a graph of the rocket’s height above ground as a function of time for $0 \le t \le 8$.
a. 800 ft
#### Definite Integrals
In Exercises 5–8, express each limit as a definite integral. Then evaluate the integral to find the value of the limit. In each case, $P$ is a partition of the given interval and the numbers $c_k$ are chosen from the subintervals of P.  

5. $\lim\limits_{||P||\to0}\sum\limits_{k=1}^n(2c_k - 1)^{-\frac{1}{2}}\Delta x_k$, where $P$ is a partition of $[1, 5]$  
   $\int_0^5\dfrac{1}{\sqrt{2x-1}}dx$   
   $u = 2x-1, \dfrac{du}{dx} = 2,du=2dx$  
   $\int_0^5\dfrac{1}{\sqrt{2x-1}}dx = \int_{-1}^9\dfrac{1}{2}u^{-\frac{1}{2}}du =[u]_{-1}^9=10$
#### Area
In Exercises 11–14, find the total area of the region between the graph of $ƒ$ and the $x$-axis.

11. $f(x) = x^2 - 4x + 3, 0 \le x \le 3$  
    zero:$1,3$  
    $F(x) = \int f(x)dx = \dfrac{1}{3}x^3-2x^2+3x + C$    
    $S = |F(1)-f(0)|+|F(3)-f(1)|$  
    $=\dfrac{4}{3}+\dfrac{4}{3} = \dfrac{8}{3}$
#### Initial Value Problems
33. Show that $y = x^2 +\int_1^x \dfrac{1}{t}dt$ solves the initial value problem
    $$
    \dfrac{d^2y}{dx^2} = 2-\dfrac{1}{x^2},y'(1)=3,y(1)=1
    $$
    $y(1) = 1+0=1$  
    $y' = 2x+\dfrac{d}{dx}\int_1^x \dfrac{1}{t}dt = 2x +\dfrac{1}{x}$  
    $y'(1) = 3$  
    $y'' = 2-\dfrac{1}{x^2}$  
#### Evaluating Indefinite Integrals
Evaluate the integrals in Exercises 37–46.

37. $\int2(\cos x)^{-\frac{1}{2}} \sin x dx$  
    $u = \cos x, \dfrac{du}{dx} = -\sin x$  
    $\int2(\cos x)^{-\frac{1}{2}} \sin x dx = \int-2u^{-\frac{1}{2}} du=-4u^{\frac{1}{2}} = -4\sqrt{\cos x}$
#### Evaluating Definite Integrals
Evaluate the integrals in Exercises 47–68.

47. $\int^1_{-1}(3x^2 - 4x + 7) dx$  
    $\int^1_{-1}(3x^2 - 4x + 7) dx = [x^3-2x^2+7x]^1_{-1} =16$
#### average Values
69. Find the average value of $f(x) = mx + b$  
a. over $[-1, 1]$   
b. over $[-k, k]$   
a. $\int mx + bdx = \dfrac{m}{2}x^2+bx + C$  
$a = \dfrac{\int_{-1}^1 mx + bdx}{2} = 0$  
b. $0$
#### Diferentiating Integrals
In Exercises 75–78, ind dy>dx.

75. $y =\int_2^x\sqrt{2 + cos^3t} dt$  
    $\dfrac{dy}{dx} = \sqrt{2 + cos^3x}$
#### Theory and Examples
79. Is it true that every function $y = f(x)$ that is differentiable on $[a, b]$ is itself the derivative of some function on $[a, b]$ ? Give reasons for your answer   
    Yes
### Additional and Advanced Exercises
#### Theory and Examples
1. a. If $\int^1_07f(x) dx = 7$, does $\int^1_0f(x) dx = 1$?    
   b. If $\int^1_0f(x) dx = 4$, and $f(x) \ge 0$ does $\int^1_0\sqrt{f(x)} dx = \sqrt{4} = 2$?Give reasons for your answers.  
   a. Yes.  
   b. $f(x) = 8x,\int^1_0f(x) dx = [4x^2]^1_0 = 4$  
   $\int^1_0\sqrt{f(x)} dx= \int^1_02\sqrt{2}\sqrt{x} dx = [\dfrac{4}{3}\sqrt{2}x^{\frac{3}{2}}]^1_0 = \dfrac{4}{3}\sqrt{2} \ne 2$
#### Piecewise Continuous Functions
Although we are mainly interested in continuous functions, many functions in applications are piecewise continuous. A function $f(x)$ is piecewise continuous on a closed interval $I$ if $f$ has only finitely many discontinuities in $I$, the limits
$$
\lim_{x\to c^-}f(x)\quad\mathsf{and}\quad\lim_{x\to c^+}f(x)
$$
exist and are finite at every interior point of $I$, and the appropriate onesided limits exist and are finite at the endpoints of $I$. All piecewise continuous functions are integrable. The points of discontinuity subdivide $I$ into open and half-open subintervals on which $f$ is continuous, and the limit criteria above guarantee that $f$ has a continuous extension to the closure of each subinterval. To integrate a piecewise continuous function, we integrate the individual extensions and add the results. The integral of
$$
f(x) = \left\{\begin{aligned}
    x-1\quad&-1\le x<0\\
    x^2\quad&0 \le x<2\\
    -1 \quad&2 \le x\le3
\end{aligned}\right.
$$
(Figure 5.33) over $[-1, 3]$ is
$$
\int_{-1}^3f(x)dx = \int_{-1}^0x-1dx+\int_{0}^2x^2dx+\int_{2}^3-1dx  \\
= [x-\dfrac{1}{2}x^2]_{-1}^0 + [\dfrac{x^3}{3}]_{0}^2+[-x]_{2}^3   \\
= \dfrac{16}{9}
$$
![](../images/Thomas%20Calculus/5-3.jpg)  
The Fundamental Theorem applies to piecewise continuous functions with the restriction that $\dfrac{d}{dx}\int^x_af(t) dt$ is expected to equal $f(x)$ only at values of $x$ at which $f$ is continuous. There is a similar restriction on Leibniz’s Rule (see Exercises 27–30).     
Graph the functions in Exercises 11–16 and integrate them over their domains

11. $f(x) = \left\{\begin{aligned}x^{\frac{2}{3}}\quad&-8\le x<0 \\-4\quad&0\le x\le3\end{aligned}\right.$   
    $\int_{-8}^3f(x)dx = \int_{-8}^0x^{\frac{2}{3}}dx + \int_0^3-4dx$   
    $= [\dfrac{3}{5}x^{\frac{5}{3}}]_{-8}^0 + [-4x]_0^3$  
    $=\dfrac{32}{5}-12 = -\dfrac{28}{5}$
#### Approximating Finite Sums with Integrals
In many applications of calculus, integrals are used to approximate finite sums—the reverse of the usual procedure of using finite sums to approximate integrals.   
For example, let’s estimate the sum of the square roots of the first $n$ positive integers, $\sqrt{1}+\sqrt{2}+\cdots+\sqrt{n}$ The integral
$$
\int_0^1\sqrt{x}dx = [\dfrac{2}{3}x^{\frac{3}{2}}]_0^1 = \dfrac{2}{3}
$$
is the limit of the upper sums
$$
S_n = \sqrt{\dfrac{1}{n}}\dfrac{1}{n}+\sqrt{\dfrac{2}{n}}\dfrac{1}{n}+\cdots+\sqrt{\dfrac{n}{n}}\dfrac{1}{n} \\
= \dfrac{\sqrt{1}+\sqrt{2}+\cdots+\sqrt{n}}{n^{\frac{3}{2}}}
$$
![](../images/Thomas%20Calculus/5-4.jpg)   
Therefore, when $n$ is large, $S_n$ will be close to $\dfrac{2}{3}$ and we will have    
$$
\sqrt{1}+\sqrt{2}+\cdots+\sqrt{n} = S_n\cdot n^{\frac{3}{2}} \approx \dfrac{3}{2}n^{\frac{3}{2}}
$$
The following table shows how good the approximation can be. 

|  $n$  | Root sum | $\dfrac{3}{2}n^{\frac{3}{2}}$ |           Relative error           |
| :---: | :------: | :---------------------------: | :--------------------------------: |
|  10   |  22.468  |            21.082             | $\dfrac{1.386}{22.468 }\approx$ 6% |
|  50   |  239.04  |            235.70             |                1.4%                |
|  100  |  671.46  |            666.67             |                0.7%                |
| 1000  |  21,097  |            21,082             |               0.07%                |

19. Evaluate
    $$
    \lim_{n\to\infty}\dfrac{1^5+2^5+3^5+\cdots +n^5}{n^6}
    $$
    by showing that the limit is
    $$
    \int_0^1x^5dx
    $$ 
    and evaluating the integral.   
    $\lim\limits_{n\to\infty}\dfrac{1^5+2^5+3^5+\cdots +n^5}{n^6}$   
    $= \dfrac{1}{n}(\dfrac{1}{n})^5 + \dfrac{1}{n}(\dfrac{2}{n})^5 + \dfrac{1}{n}(\dfrac{3}{n})^5+\cdots + \dfrac{1}{n}(\dfrac{n}{n})^5$  
    $= \int_0^1x^5dx= [\dfrac{1}{6}x^6]_0^1 = \dfrac{1}{6}$
#### Defining Functions Using the Fundamental Theorem
25. A function defined by an integral. The graph of a function $f$ consists of a semicircle and two line segments as shown. Let $g(x) = \int^x_1f(t) dt$   
![](../images/Thomas%20Calculus/5-5.jpg)  
a. Find $g(1)$. b. Find $g(3)$. c. Find $g(-1)$.  
d. Find all values of $x$ on the open interval $(-3, 4)$ at which $g$ has a relative maximum.    
e. Write an equation for the line tangent to the graph of $g$ at $x = -1.$   
f. Find the $x$-coordinate of each point of inflection of the graph of $g$ on the open interval $(-3, 4)$.    
g. Find the range of $g$.  
a. $f(x) = \left\{\begin{aligned}\sqrt{4-(x+1)^2}\quad&-3< x<1 \\-x+1\quad&0\le x<2\\ x-3\quad&2\le x<4\end{aligned}\right.$  
$g(x) = \left\{\begin{aligned}\int^x_1\sqrt{4-(t+1)^2}dt\quad&-3< x<1 \\\int^x_1-t+1dt\quad&1\le x<2\\ -\dfrac{1}{2}+\int^x_2t-3dt\quad&2\le x<4\end{aligned}\right.$   
$g(1) = 0$  
b. $g(3) = -1$  
c. $g(-1) = -\pi$  
d. $g(1) = 0$  
e. $g'(x) = \left\{\begin{aligned}\sqrt{4-(x+1)^2}\quad&-3< x<1 \\-x+1\quad&0\le x<2\\ x-3\quad&2\le x<4\end{aligned}\right.$   
$g'(-1) = 2$  
$f(x) = 2x+2-\pi$  
f. $g''(x) = \left\{\begin{aligned}-\dfrac{x+1}{\sqrt{-x^2-2x+5}}\quad&-3< x<1 \\-1\quad&0\le x<2\\ 1\quad&2\le x<4\end{aligned}\right. =0$  
$x = -1$  
g. $[-2\pi,0]$