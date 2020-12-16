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