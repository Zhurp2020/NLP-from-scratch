# Thomas Calculus
## Chapter 9 First-Order Differential Equations
### 9.1 Solutions, Slope Fields, and Euler’s Method
#### Slope Fields
In Exercises 1–4, match the differential equations with their slope fields, graphed here.  
![](../images/Thomas%20Calculus/9-2.jpg)  
![](../images/Thomas%20Calculus/9-3.jpg)  

1. $y′ = x + y$  
   D 
#### Integral Equations
In Exercises 7–12, write an equivalent first-order differential equation and initial condition for $y$.

7. $y = -1 + \int_1^x(t-y(t))dt$  
   $y + 1 = \int_1^x(t-y(t))dt$  
   $y' = x - y$  
   $y(x_0) = y_0$  
#### Using Euler’s Method
In Exercises 15–20, use Euler’s method to calculate the first three approximations to the given initial value problem for the specified increment size. Calculate the exact solution and investigate the accuracy of your approximations. Round your results to four decimal places.

15. $y' = - \dfrac{2y}{x}, y(1) = -1, dx = 0.5$  
    $L(x) = -1 - \dfrac{-2}{1}(x -1)$  
    $= 2x - 3$  
    $x_1 = 1.5, y_1 = -1 - \dfrac{-2}{1}\cdot0.5 = 0$  
    $y_2 = 0 - 0 = 0$  
    $y_3 = 0$  
    $\dfrac{dy}{dx} = -\dfrac{1}{x}\cdot2y$  
    $\dfrac{1}{2y}dy = -\dfrac{1}{x}dx$  
    $\int \dfrac{1}{2y}dy = -\int \dfrac{1}{x}dx$  
    $\dfrac{1}{2}\ln |y| = -\ln |x| + C$  
    $0 = 0 + C, C = 0$  
    $\ln |y| = -2\ln |x|$  
    $|y| = \dfrac{1}{x^2}$   
    $y_1 = -\dfrac{4}{9}$  
    $y_2 = -\dfrac{1}{4}$  
    $y_3 = -\dfrac{4}{25}$
#### COMPUTER EXPLORATIONS
In Exercises 27–32, obtain a slope field and add to it graphs of the solution curves passing through the given points.

27. $y′ = y$ with  
a. $(0, 1)$ b. $(0, 2)$ c. $(0, -1)$
### 9.2 First-Order Linear Equations
#### First-Order Linear Equations
Solve the differential equations in Exercises 1–14.
1. $x\dfrac{dy}{dx} + y = e^x, x > 0$  
   $\dfrac{dy}{dx} + \dfrac{1}{x}y = \dfrac{e^x}{x}$  
   $v(x) = e^{\int\frac{1}{x}dx}, \dfrac{dv}{dx} = \dfrac{1}{x}e^{\int\frac{1}{x}dx}$  
   $\dfrac{dy}{dx}e^{\int\frac{1}{x}dx} + \dfrac{1}{x}ye^{\int\frac{1}{x}dx} = \dfrac{e^x}{x}e^{\int\frac{1}{x}dx}$  
   $\dfrac{d}{dx}e^{\int\frac{1}{x}dx}y = \dfrac{e^x}{x}e^{\int\frac{1}{x}dx}$  
   $e^{\int\frac{1}{x}dx}y = \int \dfrac{e^x}{x}e^{\int\frac{1}{x}dx}dx$  
   $x > 0, e^{\int\frac{1}{x}dx}= e^{\ln |x|} = x$   
   $y = \dfrac{1}{x}\int e^x dx = \dfrac{e^x}{x} + C$ 
#### Solving Initial Value Problems
Solve the initial value problems in Exercises 15–20.

15. $\dfrac{dy}{dt}+ 2y = 3, y(0) = 1$  
    $\dfrac{dy}{dt} = 3-2y$  
    $\dfrac{1}{3-2y}dy = dt$  
    $\int \dfrac{1}{3-2y}dy = \int dt$  
    $-\dfrac{1}{2}\ln |3-2y| = t + C$  
    $-\dfrac{1}{2}\ln 1 = 0 + C, C = 0$  
    $|3-2y|= e^{-2t}$  
    $y = \dfrac{3}{2} - \dfrac{1}{2}e^{-2t}$
#### Theory and Examples
23. Is either of the following equations correct? Give reasons for your answers.  
a. $x\int\dfrac{1}{x}dx = x\ln |x| + C$ b. $x\int\dfrac{1}{x}dx = x\ln |x| + Cx$  
b is correct
### 9.3 Applications
#### Motion Along a Line
1. coasting bicycle A 66-kg cyclist on a 7-kg bicycle starts coasting on level ground at 9 m/sec. The $k$ in Equation (1) is about 3.9 kg /sec.  
a. About how far will the cyclist coast before reaching a complete stop?  
b. How long will it take the cyclist’s speed to drop to 1 m/sec?  
a. $d = \dfrac{9\cdot73}{3.9} \approx 168$m    
b. $v = 9e^{-\frac{3.9}{73}t} = 1$  
$9e^{-\frac{3.9}{73}t} = \dfrac{1}{9}$  
$-\dfrac{3.9}{73}t = \ln\dfrac{1}{9}$  
$t = -\dfrac{73}{3.9}\ln\dfrac{1}{9} \approx 41$s  
#### Orthogonal Trajectories
In Exercises 5–10, find the orthogonal trajectories of the family of curves. Sketch several members of each family.

5. $y = mx$  
   $\dfrac{dy}{dx} = m$  
   $\dfrac{dy}{dx} = -\dfrac{1}{m}, y = -\dfrac{1}{m}x$
#### Mixture Problems
13. salt mixture. A tank initially contains 100 gal of brine in which 50 lb of salt are dissolved. A brine containing 2 lb / gal of salt runs into the tank at the rate of 5 gal/min. The mixture is kept uniform by stirring and lows out of the tank at the rate of 4 gal/min.  
a. At what rate (pounds per minute) does salt enter the tank at time $t$?  
b. What is the volume of brine in the tank at time $t$?  
c. At what rate (pounds per minute) does salt leave the tank at time $t$?  
d. Write down and solve the initial value problem describing the mixing process.  
e. Find the concentration of salt in the tank 25 min after the process start  
a. $10$ lb/min  
b. $100 - t$ gal  
c. $\dfrac{y}{100-t}\cdot4$  
d. $\dfrac{dy}{dt} = 10-\dfrac{4y}{100-t}$  
$\dfrac{dy}{dt} + \dfrac{4y}{100-t}= 10$  
$v(t) = e^{\int\frac{4}{100-t}dt} = e^{-4\ln |100 - t|} = (100 - t)^{-4}, \dfrac{dv}{dt} = -4(100 - t)^{-5}$  
$\dfrac{dy}{dt}(100 - t)^{-4} + \dfrac{4y}{100-t}(100 - t)^{-4}= 10(100 - t)^{-4}$  
$\dfrac{d}{dt}(100 - t)^{-4}y = 10(100 - t)^{-4}$  
$(100 - t)^{-4}y = \int10(100 - t)^{-4}dt$  
$y = 10(100 - t)^4(\dfrac{1}{3}(100 - t)^{-3} + C)$  
$= \dfrac{10}{3}(100 - t) + 10(100 - t)^4C$  
$y(0) = \dfrac{1000}{3} +10\cdot100^4C = 50, C = -\dfrac{-\frac{850}{3}}{10\cdot100^4}$  
d. $y(25) \approx 160$ lb  
$\dfrac{160}{75} \approx 2.13$ lb/gal
### 9.4 Graphical Solutions of Autonomous Equations
#### Phase Lines and Solution Curves
In Exercises 1–8,  
a. Identify the equilibrium values. Which are stable and which are unstable?  
b. Construct a phase line. Identify the signs of $y'$ and $y''.$  
c. Sketch several solution curves.

1. $\dfrac{dy}{dx} = (y + 2)(y - 3)$  
   $(y + 2)(y - 3) = 0, y_1 = -2, y_2 = 3$  
   $y' = y^2 -y -6, y'' = 2y-1$  
   $y > 3, y'>0, y'' > 0$  
   $\dfrac{1}{2} < y< 3, y'<0, y'' > 0$  
   $-2 < y< \dfrac{1}{2}, y'<0, y'' < 0$  
   $y<-2, y'>0, y'' < 0$  
   $-2$ is stable, $3$ is unstable  
#### Models of Population Growth
The autonomous differential equations in Exercises 9–12 represent models for population growth. For each exercise, use a phase line analysis to sketch solution curves for $P(t),$ selecting different starting values $P(0)$. Which equilibria are stable, and which are unstable?

9. $\dfrac{dP}{dt}= 1 - 2P$  
   $P = \dfrac{1}{2}$  
   $P'' = -2 < 0$  
   $\dfrac{1}{2}$ is stable
#### Applications and Examples
15. skydiving. If a body of mass $m$ falling from rest under the action of gravity encounters an air resistance proportional to the square of velocity, then the body’s velocity $t$ seconds into the fall satisfies the equation
    $$
    m\dfrac{dv}{dt} = mg-kv^2, k>0
    $$
    where $k$ is a constant that depends on the body’s aerodynamic properties and the density of the air. (We assume that the fall is too short to be affected by changes in the air’s density.)  
    a. Draw a phase line for the equation.  
    b. Sketch a typical velocity curve.  
    c. For a 110-lb skydiver ($mg = 110$) and with time in seconds and distance in feet, a typical value of $k$ is $0.005$. What is the diver’s terminal velocity? Repeat for a 200-lb skydiver.  
    a. $m\dfrac{dv}{dt} = mg-kv^2$  
    $\dfrac{dv}{dt} = g - \dfrac{kv^2}{m}$  
    $g - \dfrac{kv^2}{m} = 0, v = \plusmn\sqrt{\dfrac{mg}{k}}$  
    $v'' = -\dfrac{2k}{m}v$  
    c. $v = \sqrt{\dfrac{110}{0.005}} \approx 145$f/s  
    $v = \sqrt{\dfrac{220}{0.005}} \approx 209$f/s
