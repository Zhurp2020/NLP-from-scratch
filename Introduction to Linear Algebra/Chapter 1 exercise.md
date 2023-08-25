# Introduction to Linear Algebra
## Chapter 1 Introduction to Vectors
### 1.1 Vectors and Linear Combinations
Problems 1-9 are about addition of vectors and linear combinations. 
1. Describe geometrically (line, plane, or all of $\bold{R}^3$) all linear combinations of  
a) $\begin{bmatrix}1 \\2 \\3 \end{bmatrix}$ and $\begin{bmatrix}3 \\6 \\9 \end{bmatrix}$: a line  
b) $\begin{bmatrix}1 \\0 \\0 \end{bmatrix}$ and $\begin{bmatrix}0 \\2 \\3 \end{bmatrix}$: a plane  
c) $\begin{bmatrix}2 \\0 \\0 \end{bmatrix}$ and $\begin{bmatrix}0 \\2 \\2 \end{bmatrix}$ and $\begin{bmatrix}0 \\2 \\3 \end{bmatrix}$: all of $\bold{R}^3$  

Problems 10-14 are about special vectors on cubes and clocks in Figure 1.4.   
![](/images/linear%20algebra/1.1.4.png)  

10. Which point of the cube is $\bold{i} + \bold{j}$? Which point is the vector sum of $\bold{i} = (1, 0, 0)$ and $\bold{j} = (0, 1, 0)$ and $\bold{k} = (0, 0, 1)$? Describe all points $(x, y, z)$ in the cube.    
    $(1,1,0)$; $(1,1,1,)$; $0 \le x, y, z \le 1$   

Problems 15-19 go further with linear combinations of $\bold{v}$ and $\bold{w}$ (Figure 1.5a).  

15. Figure 1.5a shows $\bold{v} + \bold{w}$ . Mark the points $\dfrac{3}{4}\bold{v} + \dfrac{1}{4}\bold{w}$ and $\dfrac{1}{4}\bold{v} + \dfrac{1}{4}\bold{w}$ and $\bold{v} + \bold{w}$
   ![](/images/linear%20algebra/1.1.5.png)

Problems 20-25 deal with $\bold{u}$, $\bold{v}$, $\bold{w}$ in three-dimensional space (see Figure L5b).

20. Locate $\dfrac{1}{3}\bold{u} + \dfrac{1}{3}\bold{v} + \dfrac{1}{3}\bold{w}$ and $\dfrac{1}{2}\bold{u} + \dfrac{1}{2}\bold{w}$ in Figure 1.5b. Challenge problem: Under what restrictions on $c, d, e$, will the combinations $c\bold{u} + d\bold{v} + e\bold{w}$ fill in the dashed triangle? To stay in the triangle, one requirement is $c\ge 0, d\ge 0, e\ge 0$.   
    ![](/images/linear%20algebra/1.1.5b.png)
#### Challenge Problems
27. How many corners does a cube have in 4 dimensions? How many 3D faces?How many edges? A typical corner is $(0, 0, 1, 0)$. A typical edge goes to $(0, 1, 0, 0)$.  
    16; 8 3d faces, 24 2d faces; 32 edges
### 1.2 Lengths and Dot Products
1. Calculate the dot products $\bold{u} \cdot \bold{v}$ and $\bold{u} \cdot \bold{w}$ and $\bold{u} \cdot(\bold{v} + \bold{w})$ and $\bold{w} \cdot \bold{v}$    
   $$
   \bold{u} = \begin{bmatrix}-0.6 \\0.8 \end{bmatrix}  
   \bold{v} = \begin{bmatrix}4 \\3 \end{bmatrix}  
   \bold{w} = \begin{bmatrix}1 \\2 \end{bmatrix}
   $$  
   $\bold{u} \cdot \bold{v} = 0, \bold{u} \cdot \bold{w} = 1,\bold{u} \cdot(\bold{v} + \bold{w}) = 1, \bold{w} \cdot \bold{v} = 10$    

Problems 18-28 lead to the main facts about lengths and angles in triangles.  

18. The parallelogram with sides $\bold{v}= ( 4, 2)$ and $\bold{w}= ( -1, 2)$ is a rectangle. Check the Pythagoras formula $a^2 + b^2 = c^2$ which is for right triangles only:  
    $$
    ||\bold{v}||^2 + ||\bold{w}||^2 = ||\bold{v} + \bold{w}||^2
    $$
    $||\bold{v}|| = 2\sqrt{5}, ||\bold{w}|| = \sqrt{5}, ||\bold{v} + \bold{w}|| = \sqrt{9+16} = 5$

19. (Recommended) If $||\bold{v}||=5$ and $||\bold{w}|| = 3$, what are the smallest and largest possible values of $||\bold{v} - \bold{w}||$? What are the smallest and largest possible values of $\bold{v} \cdot \bold{w}$?  
    $2 \le ||\bold{v} - \bold{w}|| \le 8$ 
    $-15 \le \bold{v} \cdot \bold{w}\le 15$
#### Challenge Problems
1.  Can three vectors in the $xy$ plane have $\bold{u} \cdot \bold{v} < 0$ and $\bold{v} \cdot \bold{w}$ and $\bold{u} \cdot \bold{w} < 0$? I don't know how many vectors in $xyz$ space can have all negative dot products. (Four of those vectors in the plane would certainly be impossible ... ).   
    Yes. They can have $120\degree$ angle each. 
### 1.3 Matrices
1. Find the linear combination $3\bold{s_1} + 4\bold{s_2} + 5\bold{s_3} = \bold{b}$ Then write $\bold{b}$ as a matrix-vector multiplication $S\bold{x}$, with 3, 4, 5 in $\bold{x}$. Compute the three dot products (row of $S$) $\cdot \bold{x}$: 
    $$
   \bold{s_1} = \begin{bmatrix}1 \\1 \\ 1 \end{bmatrix}  
   \bold{s_2} = \begin{bmatrix}0 \\ 1\\ 1 \end{bmatrix}  
   \bold{s_3} = \begin{bmatrix}0 \\ 0 \\ 1 \end{bmatrix}
   $$ 
   go into the columns of $S$  
   $3\bold{s_1} + 4\bold{s_2} + 5\bold{s_3} = \begin{bmatrix}3 \\7 \\ 12\end{bmatrix}$  
   $\bold{b}  = \begin{bmatrix}1 & 0 &0 \\ 1& 1 & 0\\ 1 &1&1 \end{bmatrix}\begin{bmatrix}3 \\ 4 \\ 5 \end{bmatrix}$  
    $
   \begin{bmatrix}1 & 0 &0  \end{bmatrix}\cdot\bold{x} =3,
   \begin{bmatrix}1 & 1&0 \end{bmatrix}\cdot\bold{x} =7,
   \begin{bmatrix}1 & 1&1 \end{bmatrix}\cdot\bold{x} =12
   $
#### Challenge Problems
13. The very last words say that the 5 by 5 centered difference matrix is not invertible.  Write down the 5 equations $C\bold{x} = \bold{b}$. Find a combination of left sides that gives zero. What combination of $b_1, b_2 , b_3, b_4, b_5$ must be zero? (The 5 columns lie on a "4-dimensional hyperplane" in 5-dimensional space. Hard to visualize.)  
    $
     \begin{bmatrix}0 & 1 & 0 & 0 & 0 \\-1 & 0 & 1 & 0 & 0 \\0 & -1 & 0 & 1 & 0 \\0 & 0 & -1 &0 & 1 \\0 & 0 & 0 & -1 & 0 \end{bmatrix}
     \begin{bmatrix}x_1 \\x_2 \\x_3 \\x_4 \\x_5 \end{bmatrix}  
     = \begin{bmatrix}x_2 \\x_3-x_1 \\x_4-x_2 \\x_5-x_3 \\-x_4 \end{bmatrix} = 
     \begin{bmatrix}b_1 \\b_2 \\b_3 \\b_4 \\b_5 \end{bmatrix}$  
     $x_2 = b_1, x_4 = -b_5 = b_3+b_1$  
     $b_1 + b_3 + b_5 = 0$
    