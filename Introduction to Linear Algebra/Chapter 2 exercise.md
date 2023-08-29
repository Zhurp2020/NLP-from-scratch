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
### 2.4 Rules for Matrix Operations
Problems 1-16 are about the laws of matrix multiplication.
1. $A$ is 3 by 5, $B$ is 5 by 3, $C$ is 5 by 1, and $D$ is 3 by 1. ,All entries are 1. Which of these matrix operations are allowed, and what are the results ?  
   $$
   BA \quad AB \quad ABD\quad DC \quad A(B+C)
   $$  
   $BA = \begin{bmatrix}3 & 3 &3&3 & 3\\ 3 & 3 &3&3 & 3 \\ 3 & 3 &3&3 & 3 \\ 3 & 3 &3&3 & 3 \end{bmatrix}$  
   $AB = \begin{bmatrix}5 & 5 & 5 \\ 5 & 5 & 5 \\ 5 & 5 & 5 \end{bmatrix}$  
   $ABD = \begin{bmatrix}15 \\ 15 \\ 15  \end{bmatrix}$  
   $DC$: not allowed  
   $A(B+C)$: not allowed

2.   For $A = \begin{bmatrix}2 & -1  \\ 3 & -2 \end{bmatrix}$  and $B =\begin{bmatrix}1 & 0 & 4  \\ 1 & 0 & 6 \end{bmatrix}$, compute these answers and nothing more:  
(a) column 2 of $AB$  
(b) row 2 of $AB$  
(c) row 2 of $AA = A^2$   
(d) row 2 of $AAA= A^3$.  
(a)$\begin{bmatrix}0  \\ 0 \end{bmatrix}$  
(b)$\begin{bmatrix}1 & 0 & 0 \end{bmatrix}$  
(c)$\begin{bmatrix}0 & 1 \end{bmatrix}$   
(d)$\begin{bmatrix}3 & -2 \end{bmatrix}$

Problems 18-20 use $a_{ij}$ for the entry in row $i$, column $j$ of $A$  

18. Write down the 3 by 3 matrix $A$ whose entries are   
    (a) $a_{ij}$ = minimum of $i$ and $j$  
    (b) $a_{ij} = (-1)^{i+j}$  
    (c) $a_{ij} = \dfrac{i}{j}$  
    (a) $\begin{bmatrix}1 & 1 & 1 \\ 1 & 2 & 2 \\ 1 & 2 & 3 \end{bmatrix}$  
    (b) $\begin{bmatrix}1 & -1 & 1 \\ -1 & 1 & -1 \\ 1 & -1 & 1 \end{bmatrix}$  
    (c) $\begin{bmatrix}1 & \dfrac{1}{2} & \dfrac{1}{3} \\ 2 & 1 & \dfrac{2}{3} \\ 3 & \dfrac{3}{2} & 1 \end{bmatrix}$   

Problems 21-24 involve powers of $A$.   

21.  Compute $A^2, A^3, A^4$ and also $A\bold{v},A^2\bold{v}, A^3\bold{v}, A^4\bold{v}$ for  
        $$
        A = \begin{bmatrix}0 & 2 & 0 &0 \\ 0 & 0 & 2 &0 \\ 0 & 0 & 0 & 2 \\ 0 & 0 & 0 &0 \end{bmatrix}, \bold{v} = \begin{bmatrix}  x \\ y \\ z\\t       \end{bmatrix}
        $$  
        $A\bold{v} = \begin{bmatrix}           2y\\2z \\2t \\0      \end{bmatrix}$  
        $A^2 = \begin{bmatrix}0 & 0 & 4 &0 \\ 0 & 0 & 0 &4 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 &0 \end{bmatrix}, A^2\bold{v}=\begin{bmatrix}     4z\\4t \\0 \\0      \end{bmatrix}$   
        $A^3 = \begin{bmatrix}0 & 0 & 0 &8 \\ 0 & 0 & 0 &0 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 &0 \end{bmatrix}, A^3\bold{v}=\begin{bmatrix}     8t\\0 \\0 \\0      \end{bmatrix}$   
        $A^4 = \begin{bmatrix}0 & 0 & 0 &0 \\ 0 & 0 & 0 &0 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 &0 \end{bmatrix}, A^4\bold{v}=\begin{bmatrix}     0\\0 \\0 \\0      \end{bmatrix}$  

Problems 25-31 use column-row multiplication and block multiplication. 

25. Multiply $A$ times $I$ using columns of $A$ (3 by 3) times rows of $I$  
    $AI = \begin{bmatrix}a & b & c \\ d & e & f \\ g & h & i \end{bmatrix}\begin{bmatrix}1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix} = \begin{bmatrix}a & b & c \\ d & e & f \\ g & h & i \end{bmatrix}$  

26. (Very important) Suppose you solve $A\bold{x} = \bold{b}$ for three special right sides $\bold{b}$:   
    $$
    A\bold{x}_1 = \begin{bmatrix}1 \\ 0 \\ 0  \end{bmatrix}, A\bold{x}_2 = \begin{bmatrix}0 \\ 1 \\ 0  \end{bmatrix}, A\bold{x}_3 = \begin{bmatrix}0 \\ 0 \\ 1  \end{bmatrix}
    $$ 
    If the three solutions $\bold{x}_1, \bold{x}_2, \bold{x}_3$ are the columns of a matrix $X$, what is $A$ times $X$?  
    $I = \begin{bmatrix}1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$
#### Challenge Problems 
36. **Practical question** Suppose $A$ is $m$ by $n$, $B$ is $n$ by $p$, and $C$ is $p$ by $q$. Then the multiplication count is $mnp$ for $AB + mpq$ for $(AB) C$. The same matrix comes from  $A$ times $BC$ with $mnq + npq$ separate multiplications. Notice $npq$ for $BC$.   
    (a): If $A$ is 2 by 4, $B$ is 4 by 7, and $C$ is 7 by 10, do you prefer $(AB) C$ or $A (BC)$?   
    (b) With $N$-component vectors, would you choose $(\bold{u}^T\bold{v})\bold{w}^T$ or $\bold{u}^T(\bold{v}\bold{w}^T)$?   
    (c) Divide by $mnpq$ to show that $(AB) C$ is faster when $n^{-1} + q^{-q} < m^{-1} + q^{-1}$  
    (a)$mnp + mpq =56 +140= 196$  
    $mnq + npq = 80 + 280 = 360$  
    $(AB)C$  is better.    
    (b)$(\bold{u}^T\bold{v})\bold{w}^T$: $2N$ multiplications  
    $\bold{u}^T(\bold{v}\bold{w}^T)$:$N+N^2$  
    use $(\bold{u}^T\bold{v})\bold{w}^T$  
    (c) $\dfrac{mnp + mpq}{mnpq} =\dfrac{1}{q} + \dfrac{1}{n}$  
    $\dfrac{mnq + npq}{mnpq} =\dfrac{1}{p} + \dfrac{1}{m}$  
    $\dfrac{1}{q} + \dfrac{1}{n} < \dfrac{1}{p} + \dfrac{1}{m}$  
    $mnp + mpq< mnq + npq$, $(AB)C$ is faster
### 2.5 Inverse Matrices
1. Find the inverses (directly or from the 2 by 2 formula) of $A, B, C$:  
   $$A = \begin{bmatrix}0 & 3  \\ 4 & 0 \end{bmatrix}, B =\begin{bmatrix}2 & 0  \\ 4 & 2 \end{bmatrix}, C = \begin{bmatrix}3 & 4  \\ 5 & 7 \end{bmatrix}$$
    $A^{-1} = -\dfrac{1}{12}\begin{bmatrix} 0 &-4\\  -& 0\ \end{bmatrix} = \begin{bmatrix} 0 &\dfrac{1}{4}\\  \dfrac{1}{3} & 0\ \end{bmatrix}$  
    $B^{-1} = \dfrac{1}{4}\begin{bmatrix}2 &-4\\ 0 & 2  \end{bmatrix} =  \begin{bmatrix}\dfrac{1}{2} & 0\\ -1 & \dfrac{1}{2}\ \end{bmatrix}$     
    $C^{-1} = \begin{bmatrix}7 & -4\\ -5 & 3 \end{bmatrix}$  

Questions 22-28 a:re about the Gauss-Jordan method for calculating $A^{-1}$  

22. Change $I$ into $A^{-1}$ as you reduce $A$ to $I$ (by row operations):   
    $$\begin{bmatrix}A &I \end{bmatrix} = \begin{bmatrix}1 & 3 & 1 & 0  \\ 2 & 7 & 0& 1 \end{bmatrix}, \begin{bmatrix}A &I \end{bmatrix} = \begin{bmatrix}1 & 4 & 1 & 0  \\ 3 & 9 & 0& 1 \end{bmatrix}$$  
    $\begin{bmatrix}1 & 3 & 1 & 0  \\ 2 & 7 & 0& 1 \end{bmatrix} \rArr \begin{bmatrix}1 & 3 & 1 & 0  \\ 0 & 1 & -2& 1 \end{bmatrix} \rArr \begin{bmatrix}1 & 0 & 7 & -3  \\ 0 & 1 & -2& 1 \end{bmatrix}$  
    $\begin{bmatrix}1 & 4 & 1 & 0  \\ 3 & 9 & 0& 1 \end{bmatrix} \rArr \begin{bmatrix}1 & 4 & 1 & 0  \\ 0 & -3 & -3& 1 \end{bmatrix} \rArr \begin{bmatrix}1 & 0 & -3& 0  \\ 0 & -3 & -3& 1 \end{bmatrix} \rArr \begin{bmatrix}1 & 0 & -3& -\dfrac{4}{3}  \\ 0 & 1 & 1& -\dfrac{1}{3} \end{bmatrix}$

29. True or false ( with a counterexample if false and a reason if true):      
    (a) A 4 by 4 matrix with a row of zeros is not invertible.  
    (b) Every matrix with l's down the main diagonal is   invertible.  
    (c) If $A$ is invertible then $A^{-1}$ and $A^2$ are invertible  
    (a): True, it does not have four pivots  
    (b): False $\begin{bmatrix}1 & 3  \\ \dfrac{1}{3} & 1 \end{bmatrix}$  
    (c): True. 
#### Challenge Problems
30. (Recommended) $A$ is a 4 by 4 matrix with 1 's on the diagonal and $-a, -b, -c$ on the diagonal above. Find $A^{-1}$ for this bidiagonal matrix.  
    $\begin{bmatrix}1 & -a & 0 &0 &1 & 0 & 0 &0 \\ 0 & 1 & -b &0 & 0 & 1 &0 &0 \\ 0 & 0 & 1 &-c & 0 & 0 & 1 &0\\ 0 & 0 & 0 &1 &  0 & 0 & 0 &1 \end{bmatrix} \rArr \begin{bmatrix}1 & 0 & 0 &0 &1 & a &ab &abc \\ 0 & 1 & 0 &0 & 0 & 1 &b &bc\\ 0 & 0 & 1 &0 & 0 & 0 & 1 &c\\ 0 & 0 & 0 &1 &  0 & 0 & 0 &1 \end{bmatrix}$
### 2.6 Elimination = Factorization: $A = LU$ 
Problems 1-14 compute the factorization $A = LU$ (and also $A = LDU$)  
1. (Important) Forward elimination changes $\begin{bmatrix}1 & 1  \\ 1 & 2 \end{bmatrix}\bold{x} = \bold{b}$ to a triangular $\begin{bmatrix}1 & 1  \\ 0 & 1 \end{bmatrix}\bold{x} = \bold{c}$
    $$\begin{alignedat}{4}x & {}+{} & y  &  & = 5\\ x  & {}+{} & 2y & & = 7\end{alignedat} \rArr \begin{alignedat}{4}x & {}+{} & y  &  & = 5\\  &  & y & & = 2\end{alignedat}，  \begin{bmatrix}1 & 1 & 5 \\ 1 & 2 & 7 \end{bmatrix} \rArr \begin{bmatrix}1 & 1 & 5 \\ 0 & 1 & 2 \end{bmatrix}$$  
    That step subtracted $l_{21} = 1$ times row 1 from row 2. The reverse step adds $l_{21}$ times row 1 to row 2. The matrix for that reverse step is $L =  \begin{bmatrix}1 & 0 \\ 1 & 1  \end{bmatrix}$. Multiply this $L$ times the triangular system $\begin{bmatrix}1 & 1  \\ 0 & 1 \end{bmatrix}\bold{x}_1 = \begin{bmatrix}5  \\2 \end{bmatrix}$ to get $\begin{bmatrix}1 & 1 \\ 1 & 2  \end{bmatrix} \bold{x}_1 = \begin{bmatrix}5  \\7 \end{bmatrix}$ . In letters, $L$ multiplies $U\bold{x} = \bold{c}$ to give $LU\bold{x} = L\bold{c}$  

Problems 15-16 use $L$ and $U$ (without needing $A$) to solve $A\bold{x} = \bold{b}$.  

15. Solve the triangular system $L\bold{c} = \bold{b}$ to find $\bold{c}$. Then solve $U\bold{x} = \bold{c}$ to find $\bold{x}$:     
    $$L = \begin{bmatrix}1 & 0  \\ 4 & 1 \end{bmatrix}, U = \begin{bmatrix}2 & 4  \\ 0 & 1 \end{bmatrix}, \bold{b} = \begin{bmatrix}2  \\ 11 \end{bmatrix}$$  
    For safety multiply $LU$ and solve $A\bold{x} = \bold{b}$ as usual. Circle $c$ when you see it.    
    $\begin{bmatrix}1 & 0  \\ 4 & 1 \end{bmatrix}\bold{c} = \begin{bmatrix}2  \\ 11 \end{bmatrix}, \bold{c} = \begin{bmatrix}2  \\ 3 \end{bmatrix}$  
    $\begin{bmatrix}2 & 4  \\ 0 & 1 \end{bmatrix}\bold{x} = \begin{bmatrix}2  \\ 3 \end{bmatrix}, \bold{x} = \begin{bmatrix}-5  \\ 3 \end{bmatrix}$   
    $\begin{bmatrix}2 & 4  \\ 8 & 17 \end{bmatrix}\bold{x} = \begin{bmatrix}2  \\ 11 \end{bmatrix}, \bold{x} = \begin{bmatrix}-5  \\ 3 \end{bmatrix}$

17. (a) When you apply the usual elimination steps to $L$, what matrix do you reach?  
    $$L = \begin{bmatrix}1 & 0 & 0 \\ l_{21} & 1 & 0 \\ l_{31} & l_{32} & 1 \end{bmatrix}$$  
    (b) When you apply the same steps to $I$, what matrix do you get?  
    (c) When you apply the same steps to $LU$, what matrix do you get?  
    (a): $I$  
    (b): $L^{-1}$  
    (c): $U$  
#### Challenge Problems
24. Which invertible matrices allow $A = LU$ (elimination without row exchanges)? Good question! Look at each of the square upper left submatrices $A_k$ of $A$.   
    All upper left $k$ by $k$ sub matrices $A_k$ must be invertible ( sizes $k = l, ... , n$ ).   
    Explain that answer: $A_k$ factors into $L_kU_k$ because $LU= \begin{bmatrix}L_k & 0  \\ * & * \end{bmatrix} \begin{bmatrix}U_k & *  \\ 0 & * \end{bmatrix}$
### 2.7 Transposes and Permutations
Questions 1-7 are about the rules for transpose matrices. 
1. Find $A^T$ and $A^{-1}$ and $(A^{-1})^T$ and $(A^T){-1}$ for  
   $$
    A = \begin{bmatrix}1 & 0  \\9 & 3 \end{bmatrix}, A = \begin{bmatrix}1 & c  \\c & 0 \end{bmatrix}
   $$  
   $A^T = \begin{bmatrix}1 & 9  \\0 & 3 \end{bmatrix}, A^{-1} = \begin{bmatrix}1 & -3  \\0 & \dfrac{1}{3} \end{bmatrix}$  
   $(A^{-1})^T = \begin{bmatrix}1 & 0  \\-3 & \dfrac{1}{3} \end{bmatrix}, (A^T)^{-1} = \begin{bmatrix}1 & 0  \\-3 & \dfrac{1}{3} \end{bmatrix}$

Questions 8-15 are about permutation matrices. 

8. Why are there $n!$ permutation matrices of order $n$?  
   $P_n^n = n!$  

Questions 16-21 are about symmetric matrices and their factorizations.  

16. If $A = A^T$ and $B = B^T$ , which of these matrices are certainly symmetric?   
    (a) $A^2 -B^2$, (b)$(A+B)(A-B)$  (c)$ABA$ (d)$ABAB$   
    $(A^2)^T =A^TA^T = A^2$  (a) and (b) are symmetric  
    $(ABA)^T = (BA)^TA^T =A^TB^TA^T = ABA$  
    $(ABAB)^T = (AB)^T (AB)^T = B^TA^TB^TA^T = BABA$, not symmetric  

Questions 22-24 are about the factorizations $PA = LU$ and $A = L_1 P_1 U_1$   

22. Find the $PA = LU$ factorizations (and check them) for  
    $$
    A = \begin{bmatrix}0 & 1 & 1 \\ 1 & 0 & 1 \\ 2 & 3 & 4 \end{bmatrix}, A = \begin{bmatrix}1 & 2 & 0 \\ 2 & 4 & 1 \\ 1 & 1 & 1 \end{bmatrix}
    $$
    $P = \begin{bmatrix}0 & 1 & 0 \\ 1 & 0 & 0 \\ 0 & 0 &1 \end{bmatrix}, PA = \begin{bmatrix}1 & 0 & 1 \\0 & 1 & 1 \\  2 & 3 & 4 \end{bmatrix} = \begin{bmatrix}1 & 0 & 0 \\ 0  & 1 & 0 \\ 2 & 3 & 1 \end{bmatrix} \begin{bmatrix}1 & 0 & 1 \\ 0 & 1 & 1 \\ 0 & 0 & -1\end{bmatrix} =LU$  
    $P = \begin{bmatrix}1 & 0 & 0 \\ 0 & 0 & 1 \\ 1 & 0 &0 \end{bmatrix}, PA = \begin{bmatrix}1 & 2 & 0 \\1 & 1 & 1 \\2 & 4 & 1  \end{bmatrix} = \begin{bmatrix}1 & 0 & 0 \\ 1 & 1 & 0 \\ 2 & 0 & 1 \end{bmatrix} \begin{bmatrix}1 & 2 & 0 \\ 0 & -1 & 1 \\  0 & 0& 1\end{bmatrix} =LU$

25. Prove that the identity matrix cannot be the product of three row exchanges (or five). It can be the product of two exchanges (or four).  
    $P = P_{12} P_{23} P_{13}$  
    Let $PA = I= A = IP^{-1} = P^{-1}$   
    $(P_{12} P_{23} P_{13})^{-1} = I$  
    $=P_{13}^{-1} P_{23}^{-1} P_{12}^{-1}$, so one of $P$ must be $I$   

The next three questions are about applications of the identity $(A\bold{x})^T\bold{y} = \bold{x}^T (A^T\bold{y})$.

29. Wires go between Boston, Chicago, and Seattle. Those cities are at voltages $x_B, x_C, x_S$. With unit resistances between cities, the currents between cities are in $\bold{y}$:  
    $$
    \bold{y} = A\bold{x}, \begin{bmatrix}
        y_{BC} \\ y_{CS} \\ y_{BS}
    \end{bmatrix} = \begin{bmatrix}
        1 & -1& 0 \\ 0 & 1 &-1 \\ 1 & 0 & -1
    \end{bmatrix} \begin{bmatrix}
        x_B \\ x_C  \\x_S
    \end{bmatrix}
    $$  
    (a) Find the total currents $A^T\bold{y}$ out of the three cities.  
    (b) Verify that $(A\bold{x})^T\bold{y}$ agrees with $\bold{x}^T (A^T\bold{y})$-six terms in both.  
    (a): $A^T = \begin{bmatrix}1 & 0& 1 \\ -1& 1 &0 \\ 0 & -1 & -1\end{bmatrix}, \bold{y} = \begin{bmatrix}x_B -x_C \\ x_C -x_S \\ x_B - x_S\end{bmatrix}A^T\bold{y} = \begin{bmatrix} 2x_B - x_C - x_S \\ 2x_C -x_B -x_S \\2x_S -x_C -x_B\end{bmatrix}$  
    (b) $(A\bold{x})^T\bold{y} = \bold{y}^T\bold{y} = (x_B -x_C) ^2 +  (x_C -x_S )^2 + (x_B - x_S) ^2$   
    $\bold{x}^T (A^T\bold{y}) =2x_B^2 + 2x_C^2 + 2x_S^2 -2x_Cx_B -2x_Cx_S -2x_Bx_S$  
#### Challenge Problems 
36. A square northwest matrix $B$ is zero in the southeast comer, below the antidiagonal that connects $(1, n)$ to $(n, 1)$. Will $B^T$ and $B^2$ be northwest matrices? Will $B^{-1}$ be northwest or southeast? What is the shape of $BC =$ northwest times southeast?    
    $B^T$ ia, $B^2$ is not, $B^{-1}$ is southeast  $BC$ only has non-zero values along the antidiagonal