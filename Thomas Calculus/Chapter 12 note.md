# Thomas Calculus
## Chapter 12 Vectors and the Geometry of Space
### 12.1 Three-Dimensional Coordinate Systems
#### Distance and Spheres in Space
>The Distance Between $P_1(x_1,y_1,z_1)$ and $P_2(x_2,y_2,z_2)$  
>$$
>|P_1P_2| = \sqrt{(x_2-x_1)^2 + (y_2-y_1)^2 + (z_2-z_1)^2}
>$$

>The Standard Equation for the Sphere of Radius $a$ and Center $(x0, y_0, z_0)$
>$$
>(x-x_0)^2 + (y-y_0)^2 + (z-z_0)^2 = a^2
>$$
### 12.2 Vectors
#### Component Form
>**DEFINITIONS**   
The vector represented by the directed line segment $\overrightarrow{AB}$ has initial point $A$ and terminal point B and its length is denoted by $|\overrightarrow{AB}|$ . Two vectors are equal if they have the same length and direction

>**DEFINITION**   
If $\mathbf{v}$ is a two-dimensional vector in the plane equal to the vector with initial point at the origin and terminal point $(v_1 , v_2)$, then the component form of $\mathbf{v}$ is
>$$
>\mathbf{v} = <v_1,v_2>
>$$
>If $\mathbf{v}$ is a three-dimensional vector equal to the vector with initial point at the origin and terminal point $(v_1 ,v_2,v_3)$, then the component form of $\mathbf{v}$ is
>$$
>\mathbf{v} = <v_1,v_2,v_3>
>$$
#### Vector Algebra Operations
>**DEFINITIONS**   
Let $\mathbf{u} = (u_1 ,u_2,u_3)$ and $\mathbf{v} = (v_1 ,v_2,v_3)$ be vectors with $k$ a scalar.   
>Addition: 
>$$
>\mathbf{u} + \mathbf{v} = <u_1 + v_1,u_2 +v_2,u_2>
>$$
>scalar multiplication: 
>$$
>k\mathbf{u}= <ku_1,ku_2,ku_3>
>$$
#### Unit Vectors
#### Midpoint of a Line Segment
#### Applications
### 12.3 The Dot Product
#### Angle Between Vectors
>**THEOREM 1—Angle Between Two Vectors**  
The angle $\theta$ between two nonzero vectors $\mathbf{u} = (u_1 ,u_2,u_3)$ and $\mathbf{v} = (v_1 ,v_2,v_3)$ is given by
>$$
>\theta = \cos^{-1}\dfrac{u_1v_1 + u_2v_2 + u_3v_3}{|\mathbf{u}||\mathbf{v}|}
>$$

>**DEFINITION**   
The dot product $\mathbf{u}\cdot\mathbf{v}$ of vectors $\mathbf{u} = (u_1 ,u_2,u_3)$ and $\mathbf{v} = (v_1 ,v_2,v_3)$ is the scalar  
>$$
>\mathbf{u}\cdot\mathbf{v}= u_1v_1 + u_2v_2 + u_3v_3
>$$
#### Orthogonal Vectors
>**DEFINITION**   
Vectors $\mathbf{u}$ and $\mathbf{v}$ are orthogonal if $\mathbf{u}\cdot\mathbf{v} = 0$
#### Dot Product Properties and Vector Projections
#### Work
>**DEFINITION**   
The work done by a constant force $\mathbf{F}$ acting through a displacement $\mathbf{D} = \overrightarrow{PQ}$ is
>$$
>W = \mathbf{F}\cdot \mathbf{D}
>$$
### 12.4 The Cross Product
#### The Cross Product of Two Vectors in Space
>**DEFINITION** The cross product $\mathbf{u}\times\mathbf{v}$ is the vector 
>$$
>\mathbf{u}\times\mathbf{v} = |\mathbf{u}||\mathbf{v}|\sin\theta \mathbf{n}
>$$ 

>**Parallel Vectors**  
Nonzero vectors $\mathbf{u}$ and $\mathbf{u}$ are parallel if and only if $\mathbf{u}\times\mathbf{v} = 0$

>**Properties of the Cross Product**  
If $\mathbf{u}, \mathbf{v},$ and $\mathbf{w}$ are any vectors and $r, s$ are scalars, then  
>1. $(r\mathbf{u}) \times (s\mathbf{v}) = (rs)(\mathbf{u}\times\mathbf{v})$ 
>2. $\mathbf{u}\times(\mathbf{v} +\mathbf{w}) = \mathbf{u}\times\mathbf{v} + \mathbf{u}\times\mathbf{w}$
>3. $\mathbf{v}\times\mathbf{u} = -\mathbf{u}\times\mathbf{v}$ 
>4. $(\mathbf{v} +\mathbf{w})\times\mathbf{u} = \mathbf{v}\times\mathbf{u} + \mathbf{w}\times\mathbf{u}$
>5. $0 \times\mathbf{u} = 0$ 
>6. $\mathbf{u} \times (\mathbf{v} \times \mathbf{w}) = (\mathbf{u} \cdot \mathbf{w})\mathbf{v} - (\mathbf{u} \cdot \mathbf{v})\mathbf{w}$  
#### $|\mathbf{u} \times \mathbf{v}|$ Is the Area of a Parallelogram
$$
|\mathbf{u} \times \mathbf{v}| = |\mathbf{u}||\mathbf{v}||\sin\theta|| \mathbf{n}| = |\mathbf{u}||\mathbf{v}|\sin\theta 
$$
#### Determinant Formula for $\mathbf{u} \times \mathbf{v}$
>Calculating the Cross Product as a Determinant  
If $\mathbf{u} = u_1\mathbf{i} +u_2\mathbf{j}+u_3\mathbf{k}$ and $\mathbf{v} = v_1\mathbf{i} +v_2\mathbf{j}+v_3\mathbf{k}$ then
>$$
>\mathbf{u} \times \mathbf{v} = \left| \begin{array}{cccc}
>    \mathbf{i}  & \mathbf{j}   & \mathbf{k} \\\
>    u_1 & u_2 & u_3 \\
>    v_1 & v_2 & v_3
>\end{array}\right|
>$$
#### Torque
#### Triple Scalar or Box Product
>Calculating the Triple Scalar Product as a Determinant  
>$$
>(\mathbf{u} \times \mathbf{v})\cdot  \mathbf{w})= \left| \begin{array}{cccc}
>    u_1 & u_2 & u_3 \\
>    v_1 & v_2 & v_3 \\
>    w_1 & w_2 & w_3 \\
>\end{array}\right|
>$$