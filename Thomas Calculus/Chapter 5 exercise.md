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
     
| Time(h) | Leakage (gal/h)  | Time(h) | Leakage (gal/h) |
| :-------: | :--------------: | :-------: | :--------------: |
|     0     |        50         |     5     |        265        |
|     1     |        70        |     6     |        369
|     2     |        90        |     7     |        516         |
|     3     |        136        |     8     |        720        |
|     4     |        190        |          |
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