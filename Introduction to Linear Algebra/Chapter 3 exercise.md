# Introduction to Linear Algebra
## Chapter 3 Vector Spaces and Subspaces
### 3.1 Spaces of Vectors
The first problems 1-8 are about vector spaces in general. The vectors in those spaces are not necessarily column vectors. In the definition of a vector space, vector addition $\bold{x} + \bold{y}$ and scalar multiplication ex must obey the following eight rules:   
(1) $\bold{x} + \bold{y} = \bold{y} + \bold{x}$  
(2) $\bold{x} + (\bold{y} + \bold{z}) = (\bold{x} + \bold{y}) + \bold{z}$  
(3) There is a unique "zero vector" such that $\bold{x} + 0 = \bold{x}$ for all $\bold{x}$  
(4) For each $\bold{x}$ there is a unique vector -x such that $\bold{x} + ( -\bold{x}) = 0$  
(5) 1 times $\bold{x}$ equals $\bold{x}$   
(6) $(c_1c_2)\bold{x} = c_1(c_2\bold{x})$  
(7) $c(\bold{x} + \bold{y})  = c\bold{x} + c\bold{y}$  
(8) $(c_1 + c_2 )\bold{x} = c_1\bold{x} + c_2\bold{x}$   

1. Suppose $(x_1,x_2) + (y_1,y_2)$ is defined to be $(x_1 + y_2 ,x_2 + y_1)$. With the usual multiplication $c\bold{x} = ( cx_1, cx_2)$, which of the eight conditions are not satisfied?   
   (1) $\bold{x} + \bold{y} = (x_1 + y_2 ,x_2 + y_1), \bold{y} + \bold{x} = (y_1 + x_2 ,y_2 + x_1)$  
   (2) $\bold{x} + (\bold{y} + \bold{z}) = (x_1 + y_2 + z_1, x_2 + y_1 + z_2), (\bold{x} + \bold{y}) + \bold{z} = (x_1 + y_2 + z_2, x_2 + y_1 + z_1)$   

Questions 9-18 are about the "subspace requirements": $\bold{x} + \bold{y}$ and $cx$ (and then all linear combinations $c\bold{x} + d\bold{y}$) stay in the subspace. 

9. One requirement can be met while the other fails. Show this by finding  
(a) A set of vectors in $\bold{R}^2$ for which $\bold{x} + \bold{y}$ stays in the set but $\dfrac{1}{2}\bold{x}$ may be outside.  
(b) A set of vectors in $\bold{R}^2$ ( other than two quarter-planes) for which every $cx$ stays in the set but  $\bold{x} + \bold{y}$ may be outside.  
(a): $|x| \le 1, |y| \le 1$  
(b): $|x| <1, |y| < 1$  

Questions 19-27 are about column spaces $C (A)$ and the equation $A\bold{x} = \bold{b}$.   

18. Describe the column spaces (lines or planes) of these particular matrices  
    $$A = \begin{bmatrix}1 & 2 \\ 0 & 0 \\ 0 & 0 \end{bmatrix}, B = \begin{bmatrix}1 & 0 \\ 0 & 2 \\ 0 & 0 \end{bmatrix}, C = \begin{bmatrix}1 & 2 \\ 2 & 0 \\ 0 & 0 \end{bmatrix}$$   
    $A$ the $x$ axis, $B$ is the $xz$ plane, $C$ is the $xy$ plane  

28. Construct a 3 by 3 matrix whose column space contains $( 1, 1, 0)$ and $( 1, 0, 1)$ but not $(1, 1, 1)$. Construct a 3 by 3 matrix whose column space is only a line   
    $\begin{bmatrix}1 & 1 & 2 \\ 1 & 0 & 2 \\ 0 & 1 & 0 \end{bmatrix}$  
    $\begin{bmatrix}1 & 2 & 3 \\ 2 & 4 & 6 \\ 3 & 6 & 9 \end{bmatrix}$ 
#### Challenge Problems
30. Suppose $S$ and $T$ are two subspaces of a vector space $V$.   
(a) Definition: The sum $S + T$ contains all sums $\bold{s} + \bold{t}$ of a vector $\bold{s}$ in $S$ and a vector $\bold{t}$ in $T$. Show that $S + T$ satisfies the requirements (addition and scalar multiplication) for a vector space.   
(b) If $S$ and $T$ are lines in $\bold{R}^m$, what is the difference between $S + T$ and $S \cup T$? That union contains all vectors from $S$ or $T$ or both. Explain this statement: The span of $S \cup T$ is $S + T$. (Section 3.5 returns to this word "span".)  
(a) Let $\bold{v}$, $\bold{w}$ be two vectors in $S + T$   
$\bold{v} + \bold{w} = \bold{s}_1 + \bold{t}_1 + \bold{s}_2 + \bold{t}_2 = \bold{s}_1 + \bold{s}_2 + \bold{t}_1 + \bold{t}_1$, also in $S + T$  
(b) $S + T$ is the plane, $S \cup T$ is the two lines    
### 3.2 The Nullspace of $A$: Solving $A\bold{x} = \bold{0}$ and $R\bold{x} = \bold{0}$    
1. Reduce $A$ and $B$ to their triangular echelon forms $U$. Which variables are free?  
   a) $\begin{bmatrix}1 & 2 & 2 & 4 & 6 \\1 & 2 & 3 & 6 & 9 \\0 & 0& 1 & 2 & 3 \end{bmatrix}$ b) $\begin{bmatrix}2 & 4 & 2 \\ 0 & 4 & 4 \\ 0 & 8 & 8\end{bmatrix}$   
   a) $\rArr \begin{bmatrix}1 & 2 & 2 & 4 & 6 \\0 & 0 & 1 & 2 & 3 \\0 & 0& 1 & 2 & 3 \end{bmatrix} \rArr \begin{bmatrix}1 & 2 & 0 & 0 & 0 \\0 & 0 & 1 & 2 & 3 \\0 & 0& 0 & 0 & 0 \end{bmatrix}$, columns 2,4, and 5 are free.  
   b) $\rArr \begin{bmatrix}2 & 0 & -2 \\ 0 & 4 & 4 \\ 0 & 0 & 0\end{bmatrix} \rArr \begin{bmatrix}1 & 0 & -1 \\ 0 & 1 & 1 \\ 0 &0 &0\end{bmatrix}$, column 3 is free.    

Questions 5-14 are about free variables and pivot variables.

5. True or false (with reason if true or example to show it is false):   
(a) A square matrix has no free variables.  
(b) An invertible matrix has no free variables.  
(c) An $m$ by $n$ matrix has no more than $n$ pivot variables.  
(d) An $m$ by $n$ matrix has no more than $m$ pivot variables.  
(a) F. $\begin{bmatrix}1 & 2  \\ 3 & 4 \end{bmatrix}$.  
(b) T.  
(c) T. 
(d) T. 

Questions 15-22 ask for matrices (if possible) with specific properties. 

15. Construct a matrix for which $N(A) =$ all combinations of $(2, 2, 1, 0)$ and $(3, 1, 0, 1)$.   
    $\begin{bmatrix}1 & 0 & -2 & -3 \\ 0 & 1 & -2 & -1 \end{bmatrix}$  

23. The reduced form $R$ of a 3 by 3 matrix with randomly chosen entries is almost sure 
to be $I$. What $R$ is virtually certain if the random $A$ is 4 by 3?  $I$ with an extra column of 0s.    

Problems 43-45 are about $r$ by $r$ invertible matrices inside $A$.

43. If $A$ has rank $r$, then it has an $r$ by $r$ submatrix $S$ that is invertible. Remove $m - r$ rows and $n - r$ columns to find an invertible submatrix $S$ inside $A, B$, and $C$. You could keep the pivot rows and pivot columns:  
    $A = \begin{bmatrix}1 & 2 & 3 \\ 1 & 2 & 4 \end{bmatrix}, B = \begin{bmatrix}1 & 2 & 3 \\ 2 & 4 & 6 \end{bmatrix}, C = \begin{bmatrix}0 & 1 & 0 \\ 0 & 0 & 0 \\ 0& 0 & 1 \end{bmatrix}$  
    $A: \begin{bmatrix}1 & 3 \\ 1 & 4 \end{bmatrix}, B: \begin{bmatrix}1\end{bmatrix}, C: \begin{bmatrix}1 & 0\\ 0 & 1  \end{bmatrix}$  

Problems 46-51 show that $rank(AB)$ is not greater than $rank(A)$ or $rank(B)$.  

46. Find the ranks of $AB$ and $AC$ (rank one matrix times rank one matrix):  
    $A = \begin{bmatrix}1 & 2 \\ 2 & 4 \end{bmatrix}, B = \begin{bmatrix}2 & 1 & 4 \\ 3 & 1.5 & 6 \end{bmatrix}, C = \begin{bmatrix}1 & b \\ c & bc \end{bmatrix}$  
    $AB = \begin{bmatrix}8 & 4 & 16\\ 16 & 8 &32\end{bmatrix}$ rank 1  
    $AC = \begin{bmatrix}1+2c & b + 2bc \\ 2+4c & 2b + 4bc \end{bmatrix}$ rank 1  

52. Suppose $A$ and $B$ have the same reduced row echelon form $R$.   
(a) Show that $A$ and $B$ have the same nullspace and the same row space.     
(b) We know $E_1A =R$ and $E_2B = R$. So $A$ equals an *invertible* matrix times $B$.
#### Challenge problems  
57. Suppose $A$ is an $m$ by $n$ matrix of rank $r$. Its reduced echelon form is $R$. Describe exactly the matrix $Z$ (its shape and all its entries) that comes from transposing the reduced row echelon form of $R^T$ : 
    $$R = rref(A), Z = (rref(A^T))^T$$           
    $Z$ is $n$ by $m$. It contains an $I$ along the main diagonal, and all the rest are 0
### 3.3 The Complete Solution to $A\bold{x} = \bold{b}$
1. (Recommended) Execute the six steps of Worked Example 3.3 A to describe the column space and nullspace of $A$ and the complete solution to $A\bold{x} = \bold{b}$:  
   $A = \begin{bmatrix}2 & 4& 6 &4 \\ 2 & 5 & 7 &6 \\ 2 & 3 & 5 &2 \end{bmatrix}, \bold{b} = \begin{bmatrix}b_1\\ b_2 \\ b_3\end{bmatrix} = \begin{bmatrix}4\\ 3 \\5\end{bmatrix}$   
   1. $\rArr \begin{bmatrix}2 & 4& 6 &4 & 4\\ 0 & 1 & 1 &2 &-1\\ 0 & -2 & -2 &-4 & 2 \end{bmatrix}$  
   $\rArr  \begin{bmatrix}2 & 4& 6 &4 & 4\\ 0 & 1 & 1 &2 &-1\\ 0 & 0 & 0 &0 & 0\end{bmatrix}$
   2. $b_3 + b_2 -2b_1 = 0$   
   3. The plane containing all linear combinations of $(2,2,2)$ and $(4,5,3)$, which is $b_3 + b_2 -2b_1 = 0$ in $\bold{R}^3$
   4. $s_1 = (-1,-1,1,0), s_2=(2,-2,0,1)$. The nullspace is all $c_1s_1 + c_2s_2$ in $\bold{R}^4$   
   5. $\rArr \begin{bmatrix}2 & 0& 2 &-4 & 8\\ 0 & 1 & 1 &2 &-1\\ 0 & 0 & 0 &0 & 0\end{bmatrix} \rArr \begin{bmatrix}1& 0& 1 &-2 & 4\\ 0 & 1 & 1 &2 &-1\\ 0 & 0 & 0 &0 & 0\end{bmatrix}$  
   6. $\bold{x}_p = (4,-1,0,0), \bold{x} = \bold{x}_p + c_1s_1 + c_2s_2$

Questions 3-15 are about the solution of $A\bold{x} = \bold{b}$. Follow the steps in the text to $\bold{x}_p$ and $\bold{x}_n$. Start from the augmented matrix with last column $\bold{b}$.

3. Write the complete solution as $\bold{x}_p$ plus any multiple of $\bold{s}$ in the nullspace:   
   $$x + 3y + 3z = 1 \\2x + 6y + 9z = 5 \\ -x -3y + 3z = 5$$   
   $\begin{bmatrix}1 & 3 & 3 &1\\ 2 & 6 & 9 &1 \\ -1 & -3 & 3 &5 \end{bmatrix} \rArr \begin{bmatrix}1 & 3 & 3 &1\\ 0 & 0 & 3 &3\\ 0 & 0 & 6 &6\end{bmatrix}\rArr \begin{bmatrix}1 & 3 &0 &-2\\ 0 & 0 & 1 &1\\ 0 & 0 & 0 &0\end{bmatrix}$   
   $\bold{x}_p =(-2,0,1), \bold{x}_n =c_1(-3,1,0)$  
   $\bold{x} = \begin{bmatrix}-2\\ 0 \\ 1\end{bmatrix} + x_2\begin{bmatrix}-3\\ 1 \\ 0\end{bmatrix}$  

Questions 16-20 are about matrices of "full rank" $r = m$ or $r = n$. 

16.  The largest possible rank of a 3 by 5 matrix is *3* Then there is a pivot in every *row* of $U$ and $R$. The solution to $A\bold{x} = \bold{b}$ *always exists*. The column space of $A$ is *a subspace of $\bold{R}^3$* . An example is $A = \begin{bmatrix}1 & 2 &3 &4&5 \\ 2 & 3 & 4 &5 &6\\ 3 & 4 & 5 &7 &7 \end{bmatrix}$  

21. Find the complete solution in the form $\bold{x}_p + \bold{x}_n$ to these full rank systems:   
    a) $x + y + z = 4$ b) $\begin{aligned} x + y + z = 4 \\  x-y+z =4  \end{aligned}$  
    a) $\begin{bmatrix}1 & 1 & 1 &4\end{bmatrix}$   
    $\bold{x}_p =(4,0,0), \bold{x}_n =c_1(-1,1,0) + c_2 (-1,0,1)$  
    $\bold{x} = \begin{bmatrix}4\\ 0 \\ 0\end{bmatrix} +y\begin{bmatrix}-1\\ 1 \\ 0\end{bmatrix} + z \begin{bmatrix}-1\\ 0 \\ 1\end{bmatrix}$  
    b) $\begin{bmatrix}1 & 1 & 1 &4 \\ 1 & -1 & 1 & 4\end{bmatrix}\rArr  \begin{bmatrix}1 & 1 & 1 &4 \\ 0 & -2 & 0 & 0\end{bmatrix}$     
    $\rArr \begin{bmatrix}1 & 0 & 1 &4 \\ 0 & 1 & 0 & 0\end{bmatrix}$
    $\bold{x}_p =(4,0,0), \bold{x}_n =c_1(-1,0,1)$  
    $\bold{x} = \begin{bmatrix}4\\ 0 \\ 0\end{bmatrix} + z \begin{bmatrix}-1\\ 0 \\ 1\end{bmatrix}$  

Questions 26-33 are about Gauss-Jordan elimination (upwards as well as downwards) and the reduced echelon matrix $R$.

26. Continue elimination from $U$ to $R$. Divide rows by pivots so the new pivots are all 1. Then produce zeros above those pivots to reach $R$:   
    $U = \begin{bmatrix}2 & 4 &4 \\ 0 & 3 & 6 \\ 0 & 0 & 0 \end{bmatrix}$ and $U = \begin{bmatrix}2 & 4 &4 \\ 0 & 3 & 6 \\ 0 & 0 & 5 \end{bmatrix}$   
    $\rArr\begin{bmatrix}2 & 0 &-4 \\ 0 & 3 & 6 \\ 0 & 0 & 0 \end{bmatrix} \rArr \begin{bmatrix}1 & 0 &-2 \\ 0 & 1 & 2 \\ 0 & 0 & 0 \end{bmatrix}$   
    $\rArr \begin{bmatrix}2 & 0 &0 \\ 0 & 3 & 0\\ 0 & 0 & 5 \end{bmatrix} \rArr\begin{bmatrix}1 & 0 &0 \\ 0 & 1 &0 \\ 0 & 0 & 1\end{bmatrix}$
#### Challenge Problems 
34. (Recommended!) Suppose you know that the 3 by 4 matrix $A$ has the vectors $= (2, 3, 1, 0)$ as the only special solution to $A\bold{x} = \bold{0}$.   
(a) What is the rank of $A$ and the complete solution to $A\bold{x} = \bold{0}$?  
(b) What is the exact row reduced echelon form $R$ of $A$?  
(c) How do you know that $A\bold{x} = \bold{b}$ can be solved for all $\bold{b}$?  
a) rank 3. $\bold{x} = \begin{bmatrix}0\\ 0 \\ 0 \\ 0\end{bmatrix} + x_3 \begin{bmatrix}2\\ 3 \\ 1 \\ 0\end{bmatrix}$  
b) $\begin{bmatrix}1 & 0 & -2&0 \\ 0 & 1 & -3&0 \\ 0 & 0 & 0 &1 \end{bmatrix}$  
c) $r = m < n,$ infinite solutions
### 3.4 Independence, Basis and Dimension
Questions 1-10 are about linear independence and linear dependence. 
1. Show that $\bold{v}_1,\bold{v}_2,\bold{v}_3$ are independent but $\bold{v}_1,\bold{v}_2,\bold{v}_3,\bold{v}_4$ are dependent: 
    $$\bold{v}_1 =\begin{bmatrix}1\\ 0 \\ 0 \end{bmatrix}, \bold{v}_2 =\begin{bmatrix}1\\ 1 \\ 0 \end{bmatrix}, \bold{v}_3 =\begin{bmatrix}1\\ 1 \\1 \end{bmatrix},\bold{v}_4 =\begin{bmatrix}2\\ 3 \\ 4 \end{bmatrix}$$
    Solve $c_1\bold{v}_1+c_2\bold{v}_2+c_3\bold{v}_3+c_4\bold{v}_4=0$ or $A\bold{x} = \bold{0}$. The $\bold{v}$'s go in the columns of $A$.   
    $A = \begin{bmatrix}1 & 1 & 1 \\ 0 & 1& 1\\ 0 & 0 & 1 \end{bmatrix}$ is rank 3.  
    $A = \begin{bmatrix}1 & 1 & 1 &2\\ 0 & 1& 1&3\\ 0 & 0 & 1 &4\end{bmatrix}\rArr \begin{bmatrix}1 & 0 & 0 &-1\\ 0 & 1& 0&-1\\ 0 & 0 & 1 &4\end{bmatrix}$  
    $A\bold{x} = \bold{0}$ has solution $(1,1,-4,1)$

Questions 11-14 are about the space spanned by a set of vectors. Take all linear combinations of the vectors. 

11. Describe the subspace of $\bold{R}^3$ (is it a line or plane or$R^3$?) spanned by   
(a) the two vectors $(1, 1, -1)$ and $( -1, -1, 1)$  
(b) the three vectors $(0, 1, 1)$ and $(1, 1, 0)$ and $(0, 0, 0)$  
(c) all vectors in $\bold{R}^3$ with whole number components  
(d) all vectors with positive components.  
(a) a line. (b) a plane (c) $\bold{R}^3$ (d) $\bold{R}^3$  

Questions 15-25 are about the requirements for a basis. 

15.  If $\bold{v}_1,\bold{v}_2, \dots,\bold{v}_n$ are linearly independent, the space they span has dimension *$n$*. These vectors are a *basis* for that space. If the vectors are the columns of an $m$ by $n$ matrix, then $m$ is *no less than* than $n$. If $m = n$, that matrix is *invertible*.   

Questions 26-30 are about spaces where the "vectors" are matrice. 

26. Find a basis (and the dimension) for each of these subspaces of 3 by 3 matrices:   
(a) All diagonal matrices.  
(b) All symmetric matrices ($A^T = A$).  
(c) All skew-symmetric matrices ($A^T = -A$).  
(a) $\begin{bmatrix}1 & 0 & 0 \\ 0 & 0& 0 \\ 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix}0 & 0 & 0 \\ 0 & 1& 0 \\ 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix}1 & 0 & 0 \\ 0 & 0& 0 \\ 0 & 0 & 1 \end{bmatrix}$, 3d  
(b) $\begin{bmatrix}1 & 0 & 0 \\ 0 & 0& 0 \\ 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix}0 & 1 & 0 \\ 1 &0& 0 \\ 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix}0 & 0 & 1\\ 0 & 0& 0 \\ 1 & 0 & 0\end{bmatrix}$  
$\begin{bmatrix}0 & 0& 0 \\ 0 & 1& 0 \\ 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix}0 & 0 & 0 \\ 0 &0& 1 \\ 0 & 1 & 0 \end{bmatrix}, \begin{bmatrix}0 & 0 & 0\\ 0 & 0& 0 \\ 0 & 0 & 1\end{bmatrix}$, 6d 
(c) $\begin{bmatrix}0 & 1 & 0 \\ -1 & 0& 0 \\ 0 & 0 & 0 \end{bmatrix}, \begin{bmatrix}0 & 0 &1 \\ 0 &0& 0 \\ -1 & 0 & 0 \end{bmatrix}, \begin{bmatrix}0 & 0 & 0\\ 0 & 0& 1 \\ 0 & -1 & 0\end{bmatrix}$, 3d   

Questions 31-35 are about spaces where the "vectors" are functions.   

31. (a) Find all functions that satisfy $\dfrac{dy}{dx} = 0$.   
(b) Choose a particular function that satisfies $\dfrac{dy}{dx} = 3$.  
(c) Find all functions that satisfy $\dfrac{dy}{dx} = 3$.  
(a) $y = c$ (b) $y=3x$ (c) $y=3x + c$  

36. Find a basis for the space $S$ of vectors $(a, b, c, d)$ with $a+ c + d = 0$ and also for the space $T$ with $a+ b = 0$ and $c = 2d$. What is the dimension of the intersection $S \cap T$?  
    $(1,0,1,-2),(1,-1,1,-2),(1,0,-1,0)$  
    $(1,-1,2,1),(0,0,2,1)$  
    $S\cap T: a+3d = 0, a+b = 0, c = 2d$  
    $(-3,3,2,1)$ is the only basis, a 1d line
#### Challenge Problems 
41.  Write the 3 by 3 identity matrix as a combination of the other five permutation matrices! Then show that those five matrices are linearly independent. (Assume a combination gives $c_1P_1+c_2P_2+ \dots,c_5P_5 =$ zero matrix, and check entries to prove that $c_1$ to $c_5$ must all be zero.) The five permutations are a basis for the subspace of 3 by 3 matrices with row and column sums all equal.     
    $I =\begin{bmatrix}0 & 1 & 0 \\ 1 & 0 & 0 \\ 0 & 0 & 1 \end{bmatrix} + \begin{bmatrix}0 & 0 & 1 \\ 0 & 1 & 0 \\ 1 & 0 & 0 \end{bmatrix} +\begin{bmatrix}1 & 0 & 0 \\ 0 & 0 & 1 \\  0 & 1& 0 \end{bmatrix} - \begin{bmatrix}0 & 1& 0 \\ 0 & 0 & 1 \\ 1& 0& 0 \end{bmatrix} - \begin{bmatrix}0 & 0 & 1 \\ 1 & 0 & 0 \\ 0 & 1 & 0 \end{bmatrix}$   
    $\begin{bmatrix}c_3 & c_1 + c_4 &c_2 + c_5 \\ c_1 + c_5 & c_2 & c_3 + c_4 \\ c_2 + c_4 & c_3 + c_4 & c_1 \end{bmatrix} = \bold{0}$  
    $c_1 = c_2 = c_3 = c_4 = c_5 =0$
### 3.5 Dimensions of the Four Subspaces
1. (a) If a 7 by 9 matrix has rank 5, what are the dimensions of the four subspaces? What is the sum of all four dimensions?
(b) If a 3 by 4 matrix has rank 3, what are its column space and left nullspace?   
a) column/row: 5, null space: 4, left null space: 2. sum: 16  
b) column space: rank 3, left null space: a line  
#### Challenge Problems
29. 29 If $A = \bold{u}\bold{v}^T$ is a 2 by 2 matrix of rank 1, redraw Figure 3.5 to show clearly the Four 
Fundamental Subspaces. If $B$ produces those same four subspaces, what is the exact relation of $B$ to $A$  
$B = cA, c\ne 0$