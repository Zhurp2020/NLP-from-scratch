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
### 9.4 Systems of Equations and Phase Planes
1. List three important considerations that are ignored in the competitive-hunter model as presented in the text  
   Other competitors  
   Other conditions  
   The relationship between two resources
#### Lotka-Volterra Equations for a Predator-Prey Model
In 1925 Lotka and Volterra introduced the predator-prey equations, a system of equations that models the populations of two species, one of which preys on the other. Let $x(t)$ represent the number of rabbits living in a region at time $t$, and $y(t)$ the number of foxes in the same region. As time passes, the number of rabbits increases at a rate proportional to their population, and decreases at a rate proportional to the number of encounters between rabbits and foxes. The foxes, which compete for food, increase in number at a rate proportional to the number of encounters with rabbits but decrease at a rate proportional to the number of foxes. The number of encounters between rabbits and foxes is assumed to be proportional to the product of the two populations. These assumptions lead to the autonomous system  
$$
\dfrac{dx}{dt} = (a - by) x  \\
\dfrac{dy}{dt} = (-c + dx) y
$$
where $a, b, c, d$ are positive constants. The values of these constants vary according to the specific situation being modeled. We can study the nature of the population changes without setting these constants to specific values.
9. What happens to the rabbit population if there are no foxes present?   
   Increase exponentially  
### Practice Exercises
In Exercises 1–22 solve the differential equation.
1. $y' = xe^y\sqrt{x - 2}$  
   $\dfrac{1}{e^y}y' = x\sqrt{x - 2}$  
   $\int \dfrac{dy}{e^y} = \int x\sqrt{x - 2}dx$  
   Let $u(x) = x, v'(x) = \sqrt{x - 2}$  
   $u'(x) = 1, v(x) = \dfrac{2}{3}(x - 2)^{\frac{3}{2}}$  
   $\int x\sqrt{x - 2}dx$  
   $= x\dfrac{2}{3}(x - 2)^{\frac{3}{2}} - \int \dfrac{2}{3}(x - 2)^{\frac{3}{2}}dx$  
   $= x\dfrac{2}{3}(x - 2)^{\frac{3}{2}} -\dfrac{4}{15}(x - 2)^{\frac{5}{2}}$  
   $-e^{-y} = x\dfrac{2}{3}(x - 2)^{\frac{3}{2}} -\dfrac{4}{15}(x - 2)^{\frac{5}{2}}$  
#### Initial Value Problems
In Exercises 23–28 solve the initial value problem.

23. $(x + 1)\dfrac{dy}{dx} + 2y = x, x > -1, y(0) = 1$  
    $\dfrac{dy}{dx} + \dfrac{2}{x+1}y = \dfrac{x}{x+1}$  
    $v(x) = e^{\int\frac{2}{x+1}dx}$  
    $= e^{2\ln|x + 1|} = (x + 1)^2, \dfrac{dv}{dx} =2x + 2$  
    $(x + 1)^2\dfrac{dy}{dx} + \dfrac{2}{x+1}y(x + 1)^2 = \dfrac{x}{x+1}(x + 1)^2$     
    $\dfrac{d}{dx}(x + 1)^2y = x(x+1)$   
    $(x+1)^2y = \int x^2 + xdx$  
    $y = \dfrac{\frac{2}{3}x^3 + \frac{1}{2}x^2 + C}{(x + 1)^2}$  
    $y(0) =\dfrac{C}{1} = 1, C = 1$  
#### Euler’s Method
In Exercises 29 and 30, use Euler’s method to solve the initial value problem on the given interval starting at $x_0$ with $dx = 0.1$.

29. $y' = y + \cos x, y(0) = 0; 0 \le x \le 2; x_0 = 0$  
    $L(x) = 0 + (0+\cos 0)(x - 0) = x$  
    $y_1 = L(x_1) = 0.1$  
    $y_2 = 0.1 + (0.1 + \cos 0.1)0.1 \approx 0.209$  
    $y_3 = 0.209 + (0.209 + \cos 0.2)0.1 \approx 0.328$
####  Slope Fields
In Exercises 35–38, sketch part of the equation’s slope field. Then add to your sketch the solution curve that passes through the point $P(1, -1)$. Use Euler’s method with $x_0 = 1$ and $dx = 0.2$ to estimate $y(2)$. Round your answers to four decimal places. Find the exact value of $y(2)$ for comparison.

35. $y' = x$  
    $L(x) = -1 + 1(x - 1) = x-2$  
    $y_1 = L(x_1)= -0.8$  
    $y_2 = -0.8 + 1.2\cdot0.2 = -0.56$  
    $y = \dfrac{1}{2}x^2 - \dfrac{3}{2}$  
    $y_2 = -0.52$  
#### Autonomous Differential Equations and Phase Lines
In Exercises 39 and 40:  
a. Identify the equilibrium values. Which are stable and which are unstable?  
b. Construct a phase line. Identify the signs of $y'$ and $y''.$  
c. Sketch a representative selection of solution curves.

39. $\dfrac{dy}{dx} = y^2 - 1$  
    $y^2 - 1 = 0, y_1 = -1, y_2 = 1$  
    $y'' = 2y, y_3 = 0$  
    $y > 1, y' > 0, y'' > 0$  
    $0 < y < 1, y' < 0, y'' > 0$   
    $-1 < y < 0, y' < 0, y'' < 0$  
    $y < -1, y' > 0, y'' < 0$  
    1 is unstable, -1 is stable
#### applications
41. Escape velocity. The gravitational attraction $F$ exerted by an airless moon on a body of mass $m$ at a distance $s$ from the moon’s center is given by the equation $F = -mgR^2s^{-2}$ , where $g$ is the acceleration of gravity at the moon’s surface and $R$ is the moon’s radius (see accompanying figure). The force $F$ is negative because it acts in the direction of decreasing $s$.   
    ![](../images/Thomas%20Calculus/9-4.jpg)  
    a. If the body is projected vertically upward from the moon’s surface with an initial velocity $v_0$ at time $t = 0$, use Newton’s second law, $F = ma$, to show that the body’s velocity at position $s$ is given by the equation  
    $$
    v^2 = \dfrac{2gR^2}{s} + v_0^2 -2gR
    $$
    Thus, the velocity remains positive as long as $v_0 >\sqrt{2gR}$. The velocity $v_0 =\sqrt{2gR}$ is the moon’s escape velocity. A body projected upward with this velocity or a greater one will escape from the moon’s gravitational pull.  
    b. Show that if $v_0 =\sqrt{2gR}$, then 
    $$
    s = R(1 + \dfrac{3v_0}{2R}t)^{\frac{2}{3}}
    $$   
    $F = -mgR^2s^{-2} =ma$  
    $\dfrac{dv}{dt} = a = -gR^2s^{-2}$  
    $\dfrac{dv}{dt} = \dfrac{dv}{ds}\dfrac{ds}{dt} = v\dfrac{dv}{ds}$    
    $v\dfrac{dv}{ds} = -gR^2s^{-2}$  
    $\int vdv = -gR^2\int s^{-2}ds$  
    $\dfrac{1}{2}v^2 = -gR^2(-s^{-1}) + C$   
    $v^2 = \dfrac{2gR^2}{s} + C$  
    $v(0)^2 = \dfrac{2gR^2}{s} + C = v_0^2$  
    $C = v_0^2 - \dfrac{2gR^2}{s} = v_0^2 - 2gR$  
    $v^2 = \dfrac{2gR^2}{s} + v_0^2 -2gR$  
    b. $v^2 = \dfrac{2gR^2}{s}$  
    $\dfrac{ds}{dt} = v = \sqrt\dfrac{2gR^2}{s}$  
    $\sqrt{\dfrac{s}{2gR^2}}ds = dt$  
    $\sqrt{\dfrac{1}{2gR^2}}\int\sqrt{s}ds = \int dt$  
    $\sqrt{\dfrac{1}{2gR^2}}\dfrac{2}{3}s^{\frac{3}{2}}= t + C$  
    $s^{\frac{3}{2}} = \dfrac{3\sqrt{2gR^2}}{2}t + C$   
    $s = (\dfrac{3\sqrt{2gR^2}}{2}t + C)^{\frac{2}{3}}$  
    $s(0) = C^{\frac{2}{3}} = R, C = \sqrt{R^3}$  
    $s = (\dfrac{3\sqrt{2gR^2}}{2}t + \sqrt{R^3})^{\frac{2}{3}}$  
    $= (\sqrt{R^3}(\dfrac{3\sqrt{2gR^2}}{2\sqrt{R^3}}t + 1))^{\frac{2}{3}}$  
    $= R(1 + \dfrac{3v_0}{2R}t)^{\frac{2}{3}}$
#### Mixture Problems
In Exercises 43 and 44, let $S$ represent the pounds of salt in a tank at time $t$ minutes. Set up a differential equation representing the given information and the rate at which $S$ changes. Then solve for $S$ and answer the particular questions.

43. A mixture containing 12 lb of salt per gallon flows into a tank at the rate of 6 gal/min and the well-stirred mixture lows out of the tank at the rate of 4 gal/min. The tank initially holds 160 gal of solution containing 10 lb of salt.  
    a. How many gallons of solution are in the tank after 1 minute? after 10 minutes? after 1 hour?  
    b. How many pounds of salt are in the tank after 1 minute? after 10 minutes? after 1 hour?  
    a. $V(t) = 160 + 2t$  
    $V(1) = 162$ gal  
    $v(10) = 180$ gal  
    $v(60) = 280$ gal  
    b. $\dfrac{dS}{dt} = 72 - \dfrac{4S}{160+2t}$  
    $\dfrac{dS}{dt} + \dfrac{4S}{160+2t} = 72$  
    $v(t) = e^{\int\frac{4}{160+2t}dt} =e^{2\ln |2t+160|} = (2t+160)^2, \dfrac{dv}{dt} =4(2t+160)$    
    $(2t+160)^2\dfrac{dS}{dt} + \dfrac{4S}{160+2t}(2t+160)^2 = 72(2t+160)^2$    
    $\dfrac{d}{dt}v(t)S(t) = 72(2t+160)^2$   
    $S(t) = \dfrac{72(\frac{4}{3}t^3 + 320t^2 + 160^2t) + C}{(2t+160)^2}$  
    $S(0) = \dfrac{C}{25600} = 10, C = 256000$  
    $S(1) \approx11.1$ lb  
    $S(10) \approx 85.5$ lb   
    $S(60) \approx 1334.5$ lb 
### Additional and Advanced Exercises
#### Theory and Applications
1. transport through a cell membrane. Under some conditions, the result of the movement of a dissolved substance across a cell’s membrane is described by the equation  
   $$
   \dfrac{dy}{dt} = k\dfrac{A}{V}(c - y)
   $$
   In this equation, $y$ is the concentration of the substance inside the cell and $\dfrac{dy}{dt}$ is the rate at which $y$ changes over time. The letters $k, A, V,$ and $c$ stand for constants, $k$ being the permeability coefficient (a property of the membrane), $A$ the surface area of the membrane, $V$ the cell’s volume, and $c$ the concentration of the substance outside the cell. The equation says that the rate at which the concentration changes within the cell is proportional to the difference between it and the outside concentration.  
   a. Solve the equation for $y(t)$, using $y_0$ to denote $y(0)$.  
   b. Find the steady-state concentration, $\lim\limits_{t\to\infty} y(t)$.   
   $\dfrac{dy}{dt} + \dfrac{kA}{v}y = \dfrac{kAc}{V}$  
   $v(t) = e^{\int\frac{kA}{V}dt} = e^{\frac{kA}{V}t}, \dfrac{dv}{dt} = \dfrac{kA}{V}e^{\frac{kA}{V}t}$  
   $\dfrac{dy}{dt}e^{\frac{kA}{V}t} + \dfrac{kA}{V}ye^{\frac{kA}{V}t} = \dfrac{kAc}{V}e^{\frac{kA}{V}t}$  
   $\dfrac{d}{dt}v(t)y(t) = \dfrac{kAc}{V}e^{\frac{kA}{V}t}$  
   $v(t)y(t) = \dfrac{kAc}{V}\int e^{\frac{kA}{V}t}dt$  
   $y(t) = \dfrac{kAc}{Ve^{\frac{kA}{v}t}}(\dfrac{V}{kA}e^{\frac{kA}{V}t} + C)$   
   $y(0) =\dfrac{kAc}{V}(\dfrac{V}{kA} + C) = y_0$  
   $\dfrac{kAc}{V}C = y_0 - c, C = \dfrac{V(y_0-c)}{kAc}$  
   $y = c + \dfrac{y_0 - c}{e^{\frac{kA}{V}t}}$  
   b. $\lim\limits_{t\to\infty} y(t) = c$
#### Homogeneous Equations
A first-order differential equation of the form  
$$
\dfrac{dy}{dx} = F(\dfrac{y}{x})
$$
is called homogeneous. It can be transformed into an equation whose variables are separable by defining the new variable $v = \dfrac{y}{x}$. Then, $y = vx$ and
$$
\dfrac{dy}{dx} = v + x\dfrac{dv}{dx}
$$
Substitution into the original differential equation and collecting terms with like variables then gives the separable equation
$$
\dfrac{dx}{x} + \dfrac{dv}{v-F(v)} = 0  
$$
After solving this separable equation, the solution of the original equation is obtained when we replace $v$ by $\dfrac{y}{x}$ .
Solve the homogeneous equations in Exercises 5–10. First put the equation in the form of a homogeneous equation.

5. $(x^2+y^2)dx + xydy = 0$  
   $\dfrac{x^2 +y^2}{xy} = -\dfrac{dy}{dx}$  
   $\dfrac{dy}{dx} = -(\dfrac{x}{y} + \dfrac{y}{x})$  
   Let $v = \dfrac{y}{x}, y = vx, \dfrac{dy}{dx} = v + x\dfrac{dv}{dx}$   
   $v + x\dfrac{dv}{dx} =-(v + \dfrac{1}{v})$   
   $x\dfrac{dv}{dx} = -2v - \dfrac{1}{v}$  
   $\dfrac{1}{2v +\frac{1}{v}}dv = -\dfrac{1}{x}dx$  
   $\int\dfrac{v}{2v^2 + 1}dv = -\int\dfrac{1}{x}dx$  
   Let $u(v) = 2v^2 + 1, \dfrac{du}{dv} = 4v$  
   $\int\dfrac{v}{2v^2 + 1}dv$  
   $= \dfrac{1}{4}\int\dfrac{1}{u}du$  
   $=\dfrac{1}{4}\ln (2v^2 +1)$  
   $\dfrac{1}{4}\ln (2v^2 +1) = -\ln|x| + C$  
   $\dfrac{1}{4}\ln(2\dfrac{y^2}{x^2} + 1) = -\ln |x| + C$
