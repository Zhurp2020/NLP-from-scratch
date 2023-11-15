# Introduction to Linear Algebra
## Chapter 4 Orthogonality
### 4.1 Orthogonality of the Four Subspaces 
Orthogonal vectors $\bold{v}^T\bold{w}=0, ||\bold{v}||^2 + ||\bold{w}||^2 = ||\bold{v} + \bold{w}||^2$  
Orthogonal subspaces $\bold{v}^T\bold{w}=0$ for all $\bold{v}$ in $V$ and or all $\bold{w}$ in $W$  
Every vector $\bold{x}$ in the nullspace is perpendicular to every row of $A$, because $A\bold{x} = \bold{0}$.  
The nullspace $N(A)$ and the row space $C(A^T)$ are orthogonal subspaces of $\bold{R}^n$   
Every vector $\bold{y}$ in the nullspace of $A^T$ is perpendicular to every column of $A$.   
The left nullspace $N(A^T)$ and the column space $C(A)$ are orthogonal in $\bold{R}^m$ .   
![](im/../../images/linear%20algebra/4.1.png)  
#### Orthogonal Complements
The orthogonal complement of a subspace $V$ contains every vector that is perpendicular to $V$. This orthogonal subspace is denoted by $V^{\perp}$  
>Fundamental Theorem of Linear Algebra, Part 2   
$N(A)$ is the orthogonal complement of the row space $C(A^T)$ (in $\bold{R}^n$).   
$N(A^T )$ is the orthogonal complement of the column space $C(A)$ (in $\bold{R}^m$). 
#### Drawing the Big Picture
#### Combining Bases from Subspaces
If the $n$ columns of $A$ are independent, they span $\bold{R}^n$. So $A\bold{x} = \bold{b}$ is solvable.
### 4.2 Projections
When $\bold{b}$ is projected onto a line, its projection $p$ is the part of $\bold{b}$ along that line. If $\bold{b}$ is projected onto a plane, $p$ is the part in that plane. The projection $p$ is $P\bold{b}$. The projection matrix $P$ multiplies $\bold{b}$ to give $p$.
#### Projection Onto a Line
$a\cdot e =a\cdot(b-\hat{x}a) = 0$  
$\hat{x} = \dfrac{a\cdot b}{a\cdot a}$   
The projection of $\bold{b}$ onto the line through $a$ is the vector $p = \dfrac{a^Tb}{a^Ta}a$    
Special case 1: If $b = a$ then $\hat{x} = 1$. The projection of $a$ onto $a$ is itself. $Pa= a$.   
Special case 2: If $\bold{b}$ is perpendicular to $a$ then $a^T b = 0$. The projection is $p = 0.$   
![](../images/linear%20algebra/4.2.png)  
$||\bold{p}||= ||\bold{b}||\cos\theta$  
Projection matrix $P$: $p = \dfrac{a^Tb}{a^Ta}a = P\bold{b},P = \dfrac{aa^T}{a^Ta}$  
Projecting a second time doesn't change anything, so $P^2 = P$.When $P$ projects onto one subspace, $I - P$ projects onto the perpendicular subspace
#### Projection Onto a Subspace
$A^T(b-A\hat{x}) = 0$ or: $A^TA\hat{x} = A^Tb$   
$p = A\hat{x} = A(A^TA)^{-1}A^Tb$  
$P  = A(A^TA)^{-1}A^T$  
$A^TA$ is invertible if and only if $A$ has linearly independent columns. 
### 4.3 Least Squares Approximations
When $A\bold{x} = \bold{b}$ has no solution, multiply by $A^T$ and solve $A^TA\hat{x}=A^T\bold{b}$
#### Minimizing the Error
The least squares solution $\hat{x}$ makes $E = || Ax - \bold{b} ||^2$ as small as possible.   
The partial derivatives of $|| Ax - \bold{b} ||^2$ are zero when $A^TA\hat{x}=A^T\bold{b}$
#### The Big Picture for Least Squares
![](/images/linear%20algebra/4.3.png)  
#### Fitting a Straight Line
The closest line $C + Dt$ has heights $p_1, \cdots , P_m$ with errors $e_1,\cdots , e_m$.  
Solve $A^TA\hat{x}=A^T\bold{b}$ for $x = (C, D)$. The errors are $e_i = b_i - C - Dt_i$.  
The line $C + Dt$ minimizes $e_1^2 + \cdots + e_n^2 = ||Ax - \bold{b}||^2$ when $A^TA\hat{x}=A^T\bold{b}$  
$$\begin{bmatrix}m & \sum t_i  \\ \sum t_i & \sum t_i^2 \end{bmatrix}\begin{bmatrix}C\\ D\end{bmatrix} = \begin{bmatrix}\sum b_i  \\  \sum t_ib_i \end{bmatrix}$$    
#### Dependent Columns in $A$: What is $\hat{x}$?  
#### Fitting by a Parabola
### 4.3 Orthonormal Bases and Gram-Schmidt
The vectors $\bold{q}_1,\bold{q}_2, \dots,\bold{q}_n$ are orthonormal if  
$$\bold{q}_i^T\bold{q}_j = \begin{cases}
    0\quad i \ne j\\ 1\quad i = j(||
    \bold{q}_i||^2=1)
\end{cases}$$   
A matrix with orthonormal columns is assigned the special letter $Q$.  
$Q^TQ = I$. When $Q$ is square, $Q^T Q = I$ means that $Q^T= Q{^-1}$ transpose= inverse.  
If $Q$ has orthonormal columns ( $Q^T Q = I$), it leaves lengths unchanged
$||Q\bold{x}||^2 = (Q\bold{x})^T(Q\bold{x}) = \bold{x}^TQ^TQ\bold{x}= \bold{x}^T\bold{x} = ||\bold{x}||^2$      
$(Q\bold{x})^T(Q\bold{y}) = \bold{x}^T\bold{y}$
#### Projections Using Orthonormal Bases: $Q$ Replaces $A$  
The least squares solution of $Q\bold{x} = \bold{b}$ is $\hat{x} = Q^T \bold{b}$. The projection matrix is $QQ^T$. $\bold{p} =\bold{q}_1(\bold{q}_1^T\bold{b})+\bold{q}_2(\bold{q}_2^T\bold{b})+ \dots+\bold{q}_n(\bold{q}_n^T\bold{b})$  
#### The Gram-Schmidt Process
1. $$A = \bold{a}$$
2. $$B = \bold{b} - \dfrac{A^T\bold{b}}{A^TA}A$$
3. $$C = \bold{c}-\dfrac{A^T\bold{c}}{A^TA}A-\dfrac{B^T\bold{c}}{B^TB}B$$
4. $$A = \dfrac{A}{||A||}$$
#### The Factorization $A = QR$
From independent vectors $\bold{a}_1,\bold{a}_2, \dots,\bold{a}_n$, Gram-Schmidt constructs orthonormal vectors $\bold{q}_1,\bold{q}_2, \dots,\bold{q}_n$. The matrices with these columns satisfy $A = QR$. Then $R = Q^T A$ is upper triangular because later $\bold{q}$'s are orthogonal to earlier $\bold{a}$'s. 
$$\begin{bmatrix} &  &  \\ a & b & c \\  &  &  \end{bmatrix} = \begin{bmatrix} &  &  \\ q_1 & q_2 & q_3 \\  &  &  \end{bmatrix}\begin{bmatrix} q_1^Ta&q_1^Tb& q_1^Tc \\ & q_2^Tb & q_2^Tc \\  &  &q_3^Tc  \end{bmatrix}$$  
$R^R\hat{x}=R^TQ^T\bold{b},R\hat{x}=Q^T\bold{b},\hat{x}= R^{-1}Q^T\bold{b}$  