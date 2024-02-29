# Introduction to Linear Algebra
## Chapter 8 Linear Transformations
### 8.1 The Idea of a Linear Transformation
1. A linear transformation must leave the zero vector fixed: $T(0) = 0$. Prove this from $T(\bold{v} + \bold{w}) = T(\bold{v}) + T(\bold{w})$ by choosing $\bold{w} = -\bold{v}$(and finish the proof). Prove it 
also from $T(c\bold{v}) = cT(\bold{v})$ by choosing $c = 0$.

Problems 13-19 may be harder. The input space $V$ contains all 2 by 2 matrices $M$.  

13. $M$ is any 2 by 2 matrix and $A = \begin{bmatrix}1& 2  \\ 3 & 4 \end{bmatrix}$. The transformation $T$ is defined by $T (M) = AM$. What rules of matrix multiplication show that $T$ is linear?  
    $A(M+N) = AM + AN$  
    $AcM = cAM$  
### 8.2 The Matrix of a Linear Transformation
Questions 1-4 extend the first derivative example to higher derivatives.  
1. The transformation $S$ takes the second derivative. Keep $1, x, x^2, x^3$ as the input basis $\bold{v}_1$, $\bold{v}_2$ , $\bold{v}_3$, $\bold{v}_4$ and also as output basis $\bold{w}_1$, $\bold{w}_2$ , $\bold{w}_3$, $\bold{w}_4$. Write $S(\bold{v}_1), S(\bold{v}_2), S(\bold{v}_3), S(\bold{v}_4)$ in terms of the $\bold{w}$'s. Find the 4 by 4 matrix $A_2$ for $S$.    
   $S(\bold{v}_1) = 0 =\begin{bmatrix}0 \\0  \\ 0\\0 \end{bmatrix}$    
   $S(\bold{v}_2) = 0= \begin{bmatrix}0 \\0  \\ 0\\0 \end{bmatrix}$  
   $S(\bold{v}_3) = 2= \begin{bmatrix}2 \\0  \\ 0\\0 \end{bmatrix}$  
   $S(\bold{v}_4) = 6x= \begin{bmatrix}0 \\6  \\ 0\\0 \end{bmatrix}$   
   $A = \begin{bmatrix}0 & 0 & 2&0 \\0 & 0&0&6 \\ 0 & 0 & 0&0\\0 & 0 & 0&0 \end{bmatrix}$

Questions 5-9 are about a particular transformation $T$ and its matrix $A$.

5. With bases $\bold{v}_1$, $\bold{v}_2$ , $\bold{v}_3$ and $\bold{w}_1$, $\bold{w}_2$ , $\bold{w}_3$, suppose $T(\bold{v}_1) = \bold{w}_2$ and $T(\bold{v}_2) = T(\bold{v}_3) =\bold{w}_1 + \bold{w}_3$ . $T$ is a linear transformation. Find the matrix $A$ and multiply by the vector $(1, 1, 1)$. What is the output from $T$ when the input is $\bold{v}_1 + \bold{v}_2 +\bold{v}_3$?  
   $A = \begin{bmatrix}0 & 1 & 1 \\ 1 & 0 & 0  \\ 0 & 1 & 1 \end{bmatrix}$  
   $T(\bold{v}) =(2,1,2)$  
   $T(\bold{v}_1 + \bold{v}_2 +\bold{v}_3)= 2(\bold{w}_1 + \bold{w}_2 +\bold{w}_3)$

Questions 10-13 are about invertible linear transformations. 

10. Suppose $T(\bold{v}_1) =\bold{w}_1 + \bold{w}_2 +\bold{w}_3$ and $T(\bold{v}_2) = \bold{w}_2 +\bold{w}_3$ and $T(\bold{v}_3) = \bold{w}_3$. Find the matrix $A$ for $T$ using these basis vectors. What input vector $\bold{v}$ gives $T(\bold{v}) = \bold{w}_1$?   
    $A = \begin{bmatrix}1 & 0 & 0 \\ 1 & 1 & 0  \\ 1 & 1 & 1 \end{bmatrix}$  
    $\bold{v} = \bold{v}_1-\bold{v}_2$

Questions 14-19 are about changing the basis. 
 
14. (a) What matrix $B$ transforms $(1, 0)$ into $(2, 5)$ and transforms $(0, 1)$ to $(1, 3)$?  
(b) What matrix $C$ transforms $(2, 5)$ to $(1, 0)$ and $(1, 3)$ to $(0, 1)$?  
(c) Why does no matrix transform $(2, 6)$ to $(1, 0)$ and $(1, 3)$ to $(0, 1)$?  
(a) $B = \begin{bmatrix}3 & -1  \\ -5 & 2 \end{bmatrix}$   
(b) $B = \begin{bmatrix}2 & 1  \\ 5& 3\end{bmatrix}$ 
(c) The two vectors are not a basis

Questions 20-23 are about the space of quadratic polynomials $y = A + Bx + C x^2$

20. The parabola $w_1 = \frac{1}{2}(x^2 + x)$ equals one at $x = 1$, and zero at $x = 0$ and $x = -1$.   Find the parabolas $w_2, w_3$, and then find $y(x)$ by linearity.   
(a) $w_2$ equals one at $x = 0$ and zero at $x = 1$ and $x = -1$.  
(b) $w_3$ equals one at $x = -1$ and zero at $x = 0$ and $x = 1$.  
(c) $y(x)$ equals 4 at $x = 1$ and 5 at $x = 0$ and 6 at $x = -1$. Use $w_1, w_2 , w_3.$  
$w_2 = -x^2+1,w_3 = \frac{1}{2}(x^2-x)$  
$y=4w_1+5w_2+6w_3=-x+5$
### 8.3 The Search for a Good Basis
2. These matrices $A_1$ and $A_2$ are similar to $J$. Solve $A_1B_1 = B_1J$ and $A_2B_2 = B_2J$ to find the basis matrices $B_1$ and $B_2$ with $J = B_1^{-1} A_1B_1$ and $J = B_2^{-1} A_2B_2$  
   $J = \begin{bmatrix}0& 1  \\ 0 & 0 \end{bmatrix},A_1 = \begin{bmatrix}0& 4  \\ 0 & 0 \end{bmatrix},A_2 = \begin{bmatrix}4& -8 \\ 2 & -4 \end{bmatrix}$  
   eigenvectors for $A_1$: $(1,0)$, generalized eigenvector: $(0,1)$  
   $B_1 = \begin{bmatrix}1& 0  \\ 0 & \frac{1}{4} \end{bmatrix}$  
    eigenvectors for $A_2$: $(2,1)$, generalized eigenvector: $(-\frac{3}{2},-1)$  
    $B_2 = \begin{bmatrix}2& -\frac{3}{2} \\ 1 &-1 \end{bmatrix}$