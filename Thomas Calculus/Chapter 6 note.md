# Thomas Calculus
## Chapter 6 Applications of Definite Integrals
### 6.1 Volumes Using Cross-Sections
#### Slicing by Parallel Planes
>**DEFINITION**   
The volume of a solid of integrable cross-sectional area $A(x)$ from $x = a$ to $x = b$ is the integral of $A$ from $a$ to $b$,
>$$
>V = \int_a^bA(x)dx
>$$
#### Solids of Revolution: The Disk Method
>Volume by Disks for Rotation About the $x$-Axis  
>$$
>V = \int_a^bA(x)dx = \int_a^b\pi [R(x)^2]dx
>$$
#### Solids of Revolution: The Washer Method
### 6.2 Volumes Using Cylindrical Shells
#### Slicing with Cylinders
#### The Shell Method
### 6.3 Arc Length
>**DEFINITION**   
>If $f'$ is continuous on $[a, b]$ , then the length (arc length) of the curve $y = f(x)$ from the point $A = (a, f(a))$ to the point $B = (b, f(b))$ is the value of the integral
>$$
>L = \int_a^b\sqrt{1+[f'(x)]^2}dx
>$$
#### Dealing with Discontinuities in $\dfrac{dx}{dy}$
#### The Differential Formula for Arc Length
### 6.4 Areas of Surfaces of Revolution
#### Defining Surface Area
>**DEFINITION**     
If the function $f(x) \ge 0$ is continuously differentiable on $[a, b]$ , the area of the surface generated by revolving the graph of $y = f(x)$ about the $x$-axis is
>$$
>S = \int_a^b2\pi y\sqrt{1+[f'(x)]^2}dx
>$$
#### Revolution About the y-Axis
### 6.5 Work and Fluid Forces
#### Work Done by a Constant Force
#### Work Done by a Variable Force Along a Line
>**DEFINITION**    
The work done by a variable force $F(x)$ in moving an object along the $x$-axis from $x = a$ to $x = b$ is
>$$
>W = \int_a^bF(x)dx
>$$
#### Hooke’s Law for Springs: $F =kx$
#### Lifting Objects and Pumping Liquids from Containers
#### Fluid Pressure and Forces
>The Pressure-Depth Equation   
In a fluid that is standing still, the pressure $\rho$ at depth $h$ is the luid’s weightdensity $w$ times $h$:  
>$$
>\rho = wh
>$$

>Fluid Force on a Constant-Depth Surface
>$$
>F = \rho A = whA 
>$$
### 6.6 Moments and Centers of Mass
#### Masses Along a Line
#### Thin Wires
$$
\delta(x) = \dfrac{\Delta m_k}{\Delta x_k}  \\
M = \int_a^b\delta(x)dx  \\
M_0 =  \int_a^bx\delta(x)dx  \\
\bar{x} = \dfrac{M}{M_0} = \dfrac{\int_a^b\delta(x)dx}{\int_a^bx\delta(x)dx}
$$
#### Masses Distributed over a Plane Region
#### Thin, Flat Plates
#### Plates Bounded by Two Curves
#### Centroids
#### Fluid Forces and Centroids
#### The Theorems of Pappus
>THEOREM 1—Pappus’s Theorem for Volumes  
If a plane region is revolved once about a line in the plane that does not cut through the region’s interior, then the volume of the solid it generates is equal to the region’s area times the distance traveled by the region’s centroid during the revolution. If $\rho$ is the distance from the axis of revolution to the centroid, then  
>$$
>V = 2\pi\rho A.  
>$$

>THEOREM 2—Pappus’s Theorem for Surface Areas  
If an arc of a smooth plane curve is revolved once about a line in the plane that does not cut through the arc’s interior, then the area of the surface generated by the arc equals the length L of the arc times the distance traveled by the arc’s centroid during the revolution. If $\rho$ is the distance from the axis of revolution to the
centroid, then
>$$
>S = 2\pi\rho L.  
>$$