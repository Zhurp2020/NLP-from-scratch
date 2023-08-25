# Introduction to Linear Algebra
## Chapter 2 Solving Linear Equations
### 2.1 Vectors and Linear Equations
Problems 1-8 are about the row and column pictures of $A\bold{x} = \bold{b}$  
1. With $A = I$ (the identity matrix) draw the planes in the row picture. Three sides of a box meet at the solution $x = (x,y,z) = (2,3,4)$: 
   $$
    \begin{array}{lcr}1x + 0y + 0z = 2 \\0x + 1y + 0z = 3 \\ 0x + 0y + 1z = 4\end{array}\quad
    \begin{bmatrix}1 &0 &0 \\0 &1 &0 \\0 &0 &1\end{bmatrix}\begin{bmatrix} x  \\ y  \\ z  \end{bmatrix} = 
    \begin{bmatrix}2  \\3  \\4  \end{bmatrix}
   $$
   Draw the vectors in the column picture. Two times column 1 plus three times column 2 plus four times column 3 equals the right side $\bold{b}$.  
   ![](images/../../images/linear%20algebra/2.1.png)   
   ![](im/../../images/linear%20algebra/2.2.png)  

Problems 9-14 are about multiplying matrices and vectors. 

9. Compute each $A\bold{x}$ by dot products of the rows with the column vector:   
   a) $\begin{bmatrix}1 & 2 & 4 \\ -2 & 3 & 1 \\ -4 & 1 & 2 \end{bmatrix}\begin{bmatrix}2 \\ 2 \\ 3 \end{bmatrix}$  
   b) $\begin{bmatrix}2 & 1 & 0 & 0 \\ 1 & 2 & 1 & 0 \\ 0 & 1 & 2 & 1 \\ 0 & 0 & 1 & 2\end{bmatrix}\begin{bmatrix}1 \\ 1 \\ 1 \\ 2 \end{bmatrix}$   
   a): $= \begin{bmatrix}(1,2,4)(2,2,3) \\ (-2,3,1)(2,2,3) \\ (-4,1,2)(2,2,3) \end{bmatrix} = \begin{bmatrix}18 \\ 5 \\ 0 \end{bmatrix}$  
   b) $= \begin{bmatrix}3 \\ 4 \\ 5 \\ 5 \end{bmatrix}$

Problems 15-22 ask for matrices that act in special ways on vectors.

15.  a) What is the 2 by 2 identity matrix? $I$ times $\begin{bmatrix}x \\ y \end{bmatrix}$ equals $\begin{bmatrix}x \\ y \end{bmatrix}$.  
   (b) What is the 2 by 2 exchange matrix? $P$ times $\begin{bmatrix}x \\ y \end{bmatrix}$ equals $\begin{bmatrix}y \\ x \end{bmatrix}$   
   $I = \begin{bmatrix}1 & 0  \\ 0 & 1\end{bmatrix}, P = \begin{bmatrix}0 & 1  \\ 1 & 0 \end{bmatrix}$  

Questions 26-28 review the row and column pictures in 2, 3, and 4 dimensions. 

26. Draw the row and column pictures for the equations $x - 2y = 0, x + y = 6$.   
    ![](../images/linear%20algebra/2.3.png)  
    ![](../images/linear%20algebra/2.4.png)
#### Challenge Problems
31. Invent a 3 by 3 magic matrix $M_3$ with entries 1, 2, ... , 9. All rows and columns and diagonals add to 15. The first row could be 8, 3, 4. What is $M_3$ times $(1, 1, 1)$? What is $M_4$ times $(1, 1, 1, 1)$ if a 4 by 4 magic matrix has entries 1, ... , 16?   
    $\begin{bmatrix}8 & 3 & 4 \\ 1 & 5 & 9 \\ 6 & 7 & 2 \end{bmatrix}\begin{bmatrix}1  \\ 1  \\ 1 \end{bmatrix} =\begin{bmatrix}15 \\ 15 \\ 15 \end{bmatrix}$  
    $\begin{bmatrix}8 & 3 & 4 & 9\\ 1 & 5 & 9 \\ 6 & 7 & 2 \end{bmatrix}\begin{bmatrix}1  \\ 1  \\ 1 \end{bmatrix} =\begin{bmatrix}15 \\ 15 \\ 15 \end{bmatrix}$  
    $M_4(1, 1, 1, 1) = (34, 34, 34, 34)$ because $1 + 2 + \cdots + 16 = 136$ which is $4\times 34$.
### 2.2 The Idea of Elimination
Problems 1-10 are about elimination on 2 by 2 systems. 
1. What multiple $l_{21}$ of equation 1 should be subtracted from equation 2?  
   $$
   \begin{array}{c} 2x + 3y = 1\\10x+ 9y = 11 \end{array}
   $$
   After elimination, write down the upper triangular system and circle the two pivots. The numbers 1 and 11 don't affect the pivots-use them now in back substitution.   
   5  
   $\begin{bmatrix}\boxed{2} & 3  \\ 0 & \boxed{-6}  \end{bmatrix}$ 

Problems 11-20 study elimination on 3 by 3 systems (and possible failure).   

11. (Recommended) A system of linear equations can't have exactly two solutions. Why?   
    (a) If $(x, y, z)$ and $(X, Y, Z)$ are two solutions, what is another solution?  
    (b) If 25 planes meet at two points, where else do they meet?  
    (a): The central point between them  
    (b): along the line

12. Find the pivots and the solution for both systems ($A\bold{x} = \bold{b}$ and $K\bold{x} = \bold{b}$ ):  
    $$
    \begin{alignedat}{4}2x & {}+{} & y  &       &    &       &    & = 0\\ x  & {}+{} & 2y & {}+{} & z  &       &    & = 0\\    &       & y  & {}+{} & 2z & {}+{} & t  & = 0\\ &       &    &       & z  & {}+{} & 2t & = 5\end{alignedat}   \quad
    \begin{alignedat}{4}2x & {}-{} &  y &       &    &       &    & = 0\\ -x & {}+{} & 2y & {}-{} & z  &       &    & = 0\\     &       & -y & {}+{} & 2z & {}-{} & t  & = 0\\   &       &    &       & -z & {}+{} & 2t & = 5
    \end{alignedat} 
    $$
    $\begin{alignedat}{4}2x & {}+{} & y  &       &    &       &    & = 0\\  &       & \frac{3}{2}y & {}+{} & z  &       &    & = 0\\    &       &    &  & \frac{4}{3}z & {}+{} & t  & = 0\\ &       &    &       &   &  & \frac{5}{4} t & = 5\end{alignedat}$     
    $\begin{alignedat}{4} x & = -1\\ y &= 2\\    z  & = -3\\ t & =\end{alignedat}$    
    $\begin{alignedat}{4}2x & {}-{} & y  &       &    &       &    & = 0\\   &       & \frac{3}{2}y & {}-{} & z  &       &    & = 0\\    &       &    &  & \frac{4}{3}z & {}-{} & t  & = 0\\  &       &    &       &   &  & \frac{5}{4} t & = 5\end{alignedat}$   
    $\begin{alignedat}{4}  x & = 1\\   y &= 2\\     z  & = 3\\  t & = 4 \end{alignedat}$  
    pivots: $2,\dfrac{3}{2},\dfrac{4}{3},\dfrac{5}{4}$  
#### Challenge Problems 
29. If the last corner entry is $A ( 5, 5) = 11$ and the last pivot of $A$ is $U ( 5, 5) = 4$, what different entry $A(5, 5)$ would have made A singular?   
    $7$  
### 2.3 Elimination Using Matrices
Problems 1-15 are about elimination matrices.
1. Write down the 3 by 3 matrices that produce these elimination steps:   
(a) $E_{21}$ subtracts 5 times row 1 from row 2.  
(b) $E_{32}$ subtracts -7 times row 2 from row 3.  
(c) $P$ exchanges rows 1 and 2, then rows 2 and 3.  
$\begin{bmatrix}1 & 0 & 0 \\ -5 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$  $\begin{bmatrix}1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 7 & 1 \end{bmatrix}$  $\begin{bmatrix}0 & 1& 0 \\ 0 & 0 & 1 \\ 1 & 0 &0 \end{bmatrix}$  

Problems 16-23 are about creating and multiplying matrices.

16.  Write these ancient problems in a 2 by 2 matrix form $A\bold{x} = \bold{b}$ and solve them:   
(a) $X$ is twice as old as $Y$ and their ages add to 33.  
(b) $(x, y) = (2, 5)$ and $(3, 7)$ lie on the line $y = mx + c$. Find $m$ and $c$.    
$\begin{bmatrix}1 & -2  \\ 1 & 1 \end{bmatrix}\begin{bmatrix}x \\ y \end{bmatrix} = \begin{bmatrix}0 \\ 33 \end{bmatrix}$  
$\begin{bmatrix}1 & -2  \\ 0 & 3 \end{bmatrix}\begin{bmatrix}x \\ y \end{bmatrix} = \begin{bmatrix}0 \\ 33 \end{bmatrix}$  
$\begin{bmatrix}2 & 1  \\ 3 & 1 \end{bmatrix}\begin{bmatrix}m \\ c \end{bmatrix} = \begin{bmatrix}5 \\ 7 \end{bmatrix}$  
$\begin{bmatrix}2 & 1 \\ 0 & -\dfrac{1}{2}\end{bmatrix}\begin{bmatrix}m \\ c \end{bmatrix} = \begin{bmatrix}0 \\ -\dfrac{1}{2} \end{bmatrix}$  
$m=2,c=1$  
Problems 24-27 include the column $\bold{b}$ in the augmented matrix $[A\quad\bold{b}]$  

24.. Apply elimination to the 2 by 3 augmented matrix $[ A\quad\bold{b}]$  . What is the triangular system $U\bold{x} = \bold{c}$? What is the solution $\bold{b}$?   
$$A\bold{x} = \begin{bmatrix}2 & 3  \\ 4 & 1 \end{bmatrix}\begin{bmatrix}x_1 \\ x_2\end{bmatrix} = \begin{bmatrix}1 \\17\end{bmatrix}$$    
$\begin{bmatrix}2 & 3 &1 \\ 4 & 1 &17\end{bmatrix}$   
$\begin{bmatrix}2 & 3 &1 \\ 0 & -5 &15\end{bmatrix}$  
$x_1 = 5, x_2 = -3$  

28. If $AB = I$ and $BC = I$ use the associative law to prove $A = C$.  
    $A(BC) =A = (AB)C = C$  
#### Challenge Problems 
29.  Find the triangular matrix $E$ that reduces "Pascal's matrix" to a smaller Pascal:   
     $$E \begin{bmatrix}1 & 0 &0&0 \\ 1 & 1 & 0 &0 \\ 1 & 2 & 1 &0 \\ 1 & 3 & 3 &1 \end{bmatrix} = \begin{bmatrix}1 & 0 &0&0 \\ 0 & 1 & 0 &0 \\0 & 1 & 1 &0 \\ 0 & 1 & 2 &1 \end{bmatrix}$$  
     Which matrix $M$ (multiplying several $E$'s) reduces Pascal all the way to $I$? Pascal's triangular matrix is exceptional, all of its multipliers are $l_{ij} = 1$  

     $E = \begin{bmatrix}1 & 0 &0&0 \\ -1 & 1 & 0 &0 \\ 0 & -1 & 1 &0 \\ 0 & 0 & -1 &1 \end{bmatrix}$  
     $E' = \begin{bmatrix}1 & 0 &0&0 \\ 0 & 1 & 0 &0 \\ 0 & -1 & 1 &0 \\ 0 & 0 & -1 &1 \end{bmatrix},P' = \begin{bmatrix}1 & 0 &0&0 \\ 0 & 1 & 0 &0 \\ 0 & 0 & 1 &0 \\ 0 & 0 & 1 &1 \end{bmatrix}$   
     $E'' = \begin{bmatrix}1 & 0 &0&0 \\ 0 & 1 & 0 &0 \\ 0 & 0 & 1 &0 \\ 0 & 0 & -1 &1 \end{bmatrix}$  
     $M = E'''E'E = \begin{bmatrix}1 & 0 &0&0 \\ 0 & 1 & 0 &0 \\ 0 & 0 & 1 &0 \\ 0 & 0 & -1 &1 \end{bmatrix}\begin{bmatrix}1 & 0 &0&0 \\ -1 & 1 & 0 &0 \\ 1 & -2 & 1 &0 \\ 0 & 1 & -2 &1 \end{bmatrix}$  
     $= \begin{bmatrix}1 & 0 &0&0 \\ -1 & 1 & 0 &0 \\ 1 & -2 & 1 &0 \\ -1 & 3 & -3 &1 \end{bmatrix}$