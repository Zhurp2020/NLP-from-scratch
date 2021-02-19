# Thomas Calculus
## Chapter 12 Vectors and the Geometry of Space
### 12.1 Three-Dimensional Coordinate Systems
#### Geometric Interpretations of Equations
In Exercises 1–16, give a geometric description of the set of points in space whose coordinates satisfy the given pairs of equations.
1. $x = 2, y = 3$  
   Two planes
#### Geometric Interpretations of Inequalities and Equations
In Exercises 17–24, describe the sets of points in space whose coordinates satisfy the given inequalities or combinations of equations and inequalities.

17. a. $x \ge 0, y \ge 0, z = 0$ b. $x \ge 0, y \le 0, z = 0$  
    First/Fourth quadrant
#### Distance
In Exercises 25–30, find the distance between points $P_1$ and $P_2$.

25. $P_1(1, 1, 1), P_2(3, 3, 0)$  
    $d = \sqrt{4 + 4 + 1} = 3$
#### Inequalities to Describe Sets of Points
Write inequalities to describe the sets in Exercises 45–50.

45. The slab bounded by the planes $z = 0$ and $z = 1$ (planes included)
    $0 \le z \le 1$
#### Spheres
Find the center $C$ and the radius $a$ for the spheres in Exercises 51–60.

51. $(x + 2)^2 + y^2 + (z - 2)^2 = 8$   
    $C(-2,0,2), a = 2\sqrt{2}$  
#### Theory and Examples
65. Find a formula for the distance from the point $P(x, y, z)$ to the
a. $x$-axis. b. $y$-axis. c. $z$-axis.  
a. $d = \sqrt{y^2 + z^2}$  
b. $d = \sqrt{x^2 + z^2}$   
c. $d = \sqrt{y^2 + x^2}$
### 12.2 Vectors
#### Vectors in the Plane
In Exercises 1–8, let $\mathbf{u} = <3,-2>$ and $\mathbf{u} = <-2,5>$,  Find the (a) component form and (b) magnitude (length) of the vector.

1. $3\mathbf{u}$  
   $3\mathbf{u} = <9,-6>, |3\mathbf{u}| = 3\sqrt{13}$
#### Vectors in Space
In Exercises 17–22, express each vector in the form $\mathbf{v} = v_1\mathbf{i} +v_2\mathbf{j} + v_3\mathbf{k}.$

17. $\overrightarrow{P_1P_2}$ if $P_1$ is the point $(5, 7, -1)$ and $P_2$ is the point $(2, 9, -2)$  
    $\overrightarrow{P_1P_2} = (-3,2,-1) = -3\mathbf{i} +2\mathbf{j} -\mathbf{k}$
#### Geometric Representations
In Exercises 23 and 24, copy vectors $\mathbf{u}, \mathbf{v},$ and $\mathbf{w}$ head to tail as needed to sketch the indicated vector.  

23. a. $\mathbf{u} + \mathbf{v}$  
    b. $\mathbf{u} + \mathbf{v} + \mathbf{w}$  
    c. $\mathbf{u} - \mathbf{v}$   
    d. $\mathbf{u} - \mathbf{w}$  
    ![](../images/Thomas%20Calculus/12-1.jpg)  
#### Length and Direction
In Exercises 25–30, express each vector as a product of its length and direction.

25. $2\mathbf{i} +\mathbf{j} - 2\mathbf{k}.$  
    $3\dfrac{2\mathbf{i} +\mathbf{j} - 2\mathbf{k}.}{3}$
#### Direction and Midpoints
In Exercises 35–38, find a. the direction of $\overrightarrow{P_1P_2}$ and b. the midpoint of line segment $P_1P_2$ .

35. $P_1(-1, 1, 5), P_2(2, 5, 0)$  
    $\dfrac{\overrightarrow{P_1P_2}}{5\sqrt{2}},(\dfrac{3}{2},2,-\dfrac{5}{2})$  
#### Theory and Applications
41. Linear combination Let $\mathbf{u} = 2\mathbf{i} + \mathbf{j}, v = \mathbf{i} + \mathbf{j}$, and $\mathbf{w} = \mathbf{i} - \mathbf{j}$. Find scalars $a$ and $b$ such that $\mathbf{u} = a\mathbf{v} + b\mathbf{w}$  
    $a = 2,b=-3$
### 12.3 The Dot Product
#### Dot Product and Projections
In Exercises 1–8, find  
a. $\mathbf{u} \cdot \mathbf{v}, |\mathbf{u}|,|\mathbf{v}|$  
b. the cosine of the angle between $\mathbf{v}$ and $\mathbf{u}$  
c. the scalar component of $\mathbf{u}$ in the direction of $\mathbf{v}$
d. the vector $proj_v\mathbf{u}$.    
1. $\mathbf{v} = 2\mathbf{i} - 4\mathbf{j} + \sqrt{5}\mathbf{k}, \mathbf{u} = -2\mathbf{i} + 4\mathbf{j} - \sqrt{5}\mathbf{k}$   
   $\mathbf{u} \cdot \mathbf{v} = -4 - 16 -5 = -25$  
   $|\mathbf{u}| = \sqrt{4 + 16 + 5} = 5, |\mathbf{v}| = 5$  
   $\cos\theta = \dfrac{-25}{25} = -1$  
   $|\mathbf{u}|\cos\theta = -5$  
   $proj_v\mathbf{u} = \dfrac{-25}{5}(\dfrac{\mathbf{v}}{|\mathbf{v}|})$  
   $=-2\mathbf{i} + 4\mathbf{j} - \sqrt{5}\mathbf{k}$
#### Angle Between Vectors
Find the angles between the vectors in Exercises 9–12 to the nearest hundredth of a radian.

9. $\mathbf{u} = 2\mathbf{i} + \mathbf{j}, \mathbf{v} = \mathbf{i} + 2\mathbf{j} - \mathbf{k}$  
    $\cos\theta = \dfrac{2 + 2}{\sqrt{5}\sqrt{6}} = \dfrac{4}{\sqrt{30}}$
#### Theory and Examples
19. sums and differences In the accompanying figure, it looks as if $\mathbf{v}_1 + \mathbf{v}_2$ and $\mathbf{v}_1 + \mathbf{v}_2$  are orthogonal. Is this mere coincidence, or are there circumstances under which we may expect the sum of two vectors to be orthogonal to their difference? Give reasons for your answer.  
    ![](../images/Thomas%20Calculus/12-2.jpg)  
    $|\mathbf{v}_1| = |\mathbf{v}_2|$  
#### Equations for Lines in the Plane
33. Line perpendicular to a vector Show that $\mathbf{v} = a\mathbf{i} + b\mathbf{j}$ is perpendicular to the line $ax + by = c$ by establishing that the slope of the vector $\mathbf{v}$ is the negative reciprocal of the slope of the given line.  
    $k_v = \dfrac{b}{a}$  
    $y = c-\dfrac{a}{b}x, k_l = -\dfrac{a}{b}$
#### Work
43. Work along a line Find the work done by a force $\mathbf{F} = 5\mathbf{i}$ (magnitude 5 N) in moving an object along the line from the origin to the point $(1, 1)$ (distance in meters).    
    $W = 5$  
#### Angles Between Lines in the Plane
The acute angle between intersecting lines that do not cross at right angles is the same as the angle determined by vectors normal to the lines or by the vectors parallel to the lines  
![](../images/Thomas%20Calculus/12-3.jpg)  
Use this fact and the results of Exercise 33 or 34 to find the acute angles between the lines in Exercises 47–52.

47. $3x + y = 5, 2x - y = 4$  
    $\cos\theta = \dfrac{6-1}{\sqrt{10}\sqrt{5}} = \dfrac{\sqrt{2}}{2}$
### 12.4 The Cross Product
#### Cross Product Calculations
In Exercises 1–8, find the length and direction (when defined) of $\mathbf{u} \times \mathbf{v}$ and $\mathbf{v} \times \mathbf{u}$

1. $\mathbf{u} = 2\mathbf{i} - 2\mathbf{j} - \mathbf{k}, \mathbf{v} = \mathbf{i} - \mathbf{k}$   
   $\mathbf{u} \times \mathbf{v}= \left| \begin{array}{cccc} \mathbf{i}  & \mathbf{j}   & \mathbf{k} \\2 & -2 & -1 \\1 & 0 & -1\end{array}\right|$  
   $= 3\mathbf{i} - \mathbf{j} + 2\mathbf{k}$  
   $l = \sqrt{14}, d = \dfrac{3}{\sqrt{14}}\mathbf{i} - \dfrac{1}{\sqrt{14}}\mathbf{j} + \dfrac{2}{\sqrt{14}}\mathbf{k}$  
   $\mathbf{v} \times \mathbf{u}= -3\mathbf{i} + \mathbf{j} - 2\mathbf{k}$   
#### Triangles in Space
In Exercises 15–18,
a. Find the area of the triangle determined by the points $P, Q,$ and $R.$  
b. Find a unit vector perpendicular to plane $PQR$.

15. $P(1, -1, 2), Q(2, 0, -1), R(0, 2, 1)$  
    $\overrightarrow{PQ} = (1,1,-3),\overrightarrow{PR} = (-1,3,-1)$  
    $S = \dfrac{1}{2}|\overrightarrow{PQ}\times \overrightarrow{PR}|$  
    $= \dfrac{1}{2}|\left| \begin{array}{cccc} \mathbf{i}  & \mathbf{j}   & \mathbf{k} \\1 & 1 & -3 \\-1 & 3 & -1\end{array}\right||$  
    $= \dfrac{1}{2}|10\mathbf{i} +2 \mathbf{j} +4\mathbf{k}|$  
    $= \sqrt{30}$  
    $\mathbf{n} = \dfrac{5}{\sqrt{30}}\mathbf{i} +\dfrac{1}{\sqrt{30}} \mathbf{j} +\dfrac{2}{\sqrt{30}}\mathbf{k}$
#### Triple Scalar Products
In Exercises 19–22, verify that $(\mathbf{u} \times \mathbf{v})\cdot  \mathbf{w} = (\mathbf{v} \times \mathbf{w})\cdot  \mathbf{u} = (\mathbf{w} \times \mathbf{u})\cdot  \mathbf{v}$ and find the volume of the parallelepiped (box) determined by $\mathbf{u}, \mathbf{v}$ and $\mathbf{w}$.  

|$\mathbf{u}$|$\mathbf{v}$|$\mathbf{w}$|
|:-:|:-:|:-:|
|19. $2\mathbf{i}$|$2\mathbf{j}$|$2\mathbf{k}$|  

$(\mathbf{u} \times \mathbf{v})\cdot  \mathbf{w} = \left| \begin{array}{cccc} \mathbf{i}  & \mathbf{j}   & \mathbf{k} \\2 & 0 & 0 \\0 & 2 & 0\end{array}\right|\cdot \mathbf{w}$  
$= 4\mathbf{k}\cdot2\mathbf{k} = 8$  
$(\mathbf{v} \times \mathbf{w})\cdot  \mathbf{u} = \left| \begin{array}{cccc} \mathbf{i}  & \mathbf{j}   & \mathbf{k} \\0 & 2 & 0 \\0 & 0 & 2\end{array}\right|\cdot \mathbf{u}$  
$= 4\mathbf{i}\cdot2\mathbf{i} = 8$   
$(\mathbf{w} \times \mathbf{u})\cdot  \mathbf{v} = \left| \begin{array}{cccc} \mathbf{i}  & \mathbf{j}   & \mathbf{k} \\0 & 0 & 2 \\2 & 0 & 0\end{array}\right|\cdot \mathbf{v}$  
$= 4\mathbf{j}\cdot2\mathbf{j} = 8$   
$V = 8$ 
#### Theory and Examples
23. parallel and perpendicular vectors Let $\mathbf{u} = 5\mathbf{i} -1 \mathbf{j} +1 \mathbf{k}, \mathbf{v} =  \mathbf{j} -5\mathbf{k}, \mathbf{w} = -15\mathbf{i} +3 \mathbf{j} -3\mathbf{k}$ Which vectors, if any, are (a) perpendicular? (b) Parallel? Give reasons for your answers.  
    $\mathbf{u}\cdot \mathbf{v} = 0$  
    $\mathbf{w} = 3\mathbf{u}$  
#### Area of a Parallelogram
Find the areas of the parallelograms whose vertices are given inExercises 35–40.

35. $A(1, 0), B(0, 1), C(-1, 0), D(0, -1)$  
    $S = 2$  
#### Area of a Triangle
Find the areas of the triangles whose vertices are given in Exercises 41–47.

41. $A(0, 0), B(-2, 3), C(3, 1)$  
    $S = \dfrac{1}{2}| \left| \begin{array}{cccc} \mathbf{i}  & \mathbf{j}   & \mathbf{k} \\-2 & 3 & 0\\3 & 1 & 0\end{array}\right||$  
    $= \dfrac{1}{2}|-11\mathbf{k}|$  
    $= \dfrac{11}{2}$
#### Volume of a Tetrahedron
Using the methods of Section 6.1, where volume is computed by integrating cross-sectional area, it can be shown that the volume of a tetrahedron formed by three vectors is equal to $\dfrac{1}{6}$ the volume of the parallelipiped formed by the three vectors. Find the volumes of the tetrahedra whose vertices are given in Exercises 51–54.

51. $A(0, 0, 0), B(2, 0, 0), C(0, 3, 0), D(0, 0, 4)$  
    $V = \dfrac{1}{6}|\left| \begin{array}{cccc}  2 & 0 & 0\\0 & 3 & 0 \\ 0 & 0 &4\end{array}\right||$  
    $= \dfrac{1}{6}\cdot48 = 8$
### 12.6   Cylinders and Quadric Surfaces
#### Matching Equations with Surfaces
In Exercises 1–12, match the equation with the surface it defines. Also, identify each surface by type (paraboloid, ellipsoid, etc.). The surfaces are labeled (a)–(1).
1. $x^2 + y^2 + 4z^2 = 10$    
   ![](../images/Thomas%20Calculus/12-5.jpg)  
   d, ellipsoid   
#### Drawing
Sketch the surfaces in Exercises 13–44.
##### CYLINDERS
13. $x^2 + y^2 = 4$  
#### Theory and Examples
45. a. Express the area $A$ of the cross-section cut from the ellipsoid
    $$
    x^2 + \dfrac{y^2}{4} + \dfrac{z^2}{9} = 1
    $$
    by the plane $z = c$ as a function of $c$. (The area of an ellipse with semiaxes $a$ and $b$ is $\pi ab$.)  
    b. Use slices perpendicular to the $z$-axis to find the volume of the ellipsoid in part (a).
    c. Now find the volume of the ellipsoid
    $$
    \dfrac{x^2}{a^2} + \dfrac{y^2}{b^2} + \dfrac{z^2}{c^2} = 1
    $$
    Does your formula give the volume of a sphere of radius $a$ if $a = b = c$?  
    a. $x^2 + \dfrac{y^2}{4} = 1-\dfrac{c^2}{9}$  
    $\dfrac{x^2}{1-\frac{c^2}{9}} +\dfrac{y^2}{4(1-\frac{c^2}{9})} = 1$  
    $S = \pi \sqrt{1-\dfrac{c^2}{9}}\sqrt{4(1-\dfrac{c^2}{9})}$  
    $= 2\pi(1-\dfrac{c^2}{9})$   
    b. $V = \int_{-3}^32\pi(1-\dfrac{c^2}{9})dc$  
    $=4\pi\int_0^31 - \dfrac{c^2}{9}dc$  
    $=4\pi[c - \dfrac{c^3}{27}]_0^3$  
    $= 8\pi$  
    c. $\dfrac{x^2}{a^2} + \dfrac{y^2}{b^2} = 1 - \dfrac{z^2}{c^2}$  
    $\dfrac{x^2}{a^2(1 - \frac{z^2}{c^2})} +\dfrac{y^2}{b^2(1-\frac{z^2}{c^2})} = 1$  
    $S = \pi \sqrt{a^2(1 - \dfrac{z^2}{c^2})}\sqrt{b^2(1 - \dfrac{z^2}{c^2})}$  
    $= ab\pi(1-\dfrac{c^2}{z^2})$   
    $V = \int_{-c}^cab\pi(1-\dfrac{c^2}{z^2})dz$  
    $=2ab\pi\int_0^c1 - \dfrac{z^2}{c^2}dz$  
    $=2ab\pi[z - \dfrac{z^3}{3c^2}]_0^c$  
    $= \dfrac{4}{3}abc\pi$  
#### Viewing Surfaces
Plot the surfaces in Exercises 49–52 over the indicated domains. If you can, rotate the surface into different viewing positions.

49. $z = y^2, -2 \le x \le 2, -0.5 \le y \le 2$
#### COMPUTER EXPLORATIONS
Use a CAS to plot the surfaces in Exercises 53–58. Identify the type of quadric surface from your graph.

53.  $\dfrac{x^2}{9} + \dfrac{y^2}{36} = 1-\dfrac{z^2}{25}$