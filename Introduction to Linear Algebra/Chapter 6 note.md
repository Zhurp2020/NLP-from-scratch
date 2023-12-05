# Introduction to Linear Algebra
## Chapter 6 Eigenvalues and Eigenvectors
### 6.1 Introduction to Eigenvalues
Almost all vectors change direction, when they are multiplied by $A$. Certain exceptional vectors $\bold{x}$ are in the same direction as $A\bold{x}$. Those are the "eigenvectors". Multiply an eigenvector by $A$, and the vector $A\bold{x}$ is a number $\lambda$ times the original $\bold{x}$.   
The basic equation is $A\bold{x} = \lambda \bold{x}$. The number $\lambda$ is an eigenvalue of $A$.  
When $A$ is squared, the eigenvectors stay the same. The eigenvalues are squared.   
The only eigenvalues of a projection matrix are 0 and 1. The eigenvectors for $\lambda = 0$ (which means $P\bold{x} = 0\bold{x}$) fill up the nullspace. The eigenvectors for $\lambda$ (which means $P\bold{x} =  \bold{x}$) fill up the column space. The nullspace is projected to zero. The column space projects onto itself. The projection keeps the column space and destroys the nullspace.   
The reflection matrix $\begin{bmatrix}0 & 1  \\ 1 & 0 \end{bmatrix}$ has eigenvalues 1 and -1  
#### The Equation for the Eigenvalues 
The number $\lambda$ is an eigenvalue of $A$ if and only if $A - \lambda I$ is singular  
$$
\det (A-\lambda I) = 0
$$
For each eigenvalue $\lambda$ solve $(A-\lambda I)\bold{x} = 0$ or $A\bold{x} = \lambda \bold{x}$ to find an eigenvector $\bold{x}$
#### Determinant and Trace
The product of the $n$ eigenvalues equals the determinant.   
The sum of the $n$ eigenvalues equals the sum of the $n$ diagonal entries. The sum of the entries along the main diagonal is called the trace of $A$  
#### Imaginary Eigenvalues
The 90° rotation $Q = \begin{bmatrix}0 & -1 \\ 1 & 0 \end{bmatrix}$ has no real eigenvectors. Its eigenvalues
are $\lambda_1 = i$ and $\lambda_2 = -i$. Then $\lambda_1 + \lambda_2 =$ trace $= 0$ and $\lambda_1\lambda_2 =$ determinant $= 1$
#### Eigenvalues of $AB$ and $A+ B$
$A$ and $B$ share the same n independent eigenvectors if and only if $AB = BA$
### 6.2 Diagonalizing a Matrix
Suppose the $n$ by $n$ matrix $A$ has $n$ linearly independent eigenvectors $\bold{x}_1,\bold{x}_2, \dots,\bold{x}_n$ . Put them into the columns of an eigenvector matrix $X$. Then $X^{-1}AX$ is the eigenvalue matrix $\Lambda$  
$$
X^{-1}AX = \Lambda = \begin{bmatrix}
    \lambda_1 & & \\ & \ddots & \\ && \lambda _n
\end{bmatrix}
$$
$AX = A \begin{bmatrix} & &  \\ \bold{x}_1 & \cdots & \bold{x}_n\\ && \end{bmatrix} = \begin{bmatrix} & &  \\ \lambda_1\bold{x}_1 & \cdots & \lambda_n\bold{x}_n\\ && \end{bmatrix}$  
$= \begin{bmatrix} & &  \\ \bold{x}_1 & \cdots & \bold{x}_n\\ && \end{bmatrix}\begin{bmatrix}\lambda_1 & & \\ & \ddots & \\ && \lambda _n\end{bmatrix} = X\Lambda$  
$AX=X\Lambda \rArr X^{-1}AX = \Lambda$ or $A = X\Lambda X^{-1}$    
$A^k = (X\Lambda X^{-1})\cdots(X\Lambda X^{-1}) = X\Lambda^k X^{-1}$  
Suppose the eigenvalues $\lambda_1,\lambda_2,\cdots,\lambda_n$ are all different. Then it is automatic that the eigenvectors $\bold{x}_1,\bold{x}_2, \dots,\bold{x}_n$ are independent. The eigenvector matrix $X$ will be invertible. Any matrix that has no repeated eigenvalues can be diagonalized.  
We can multiply eigenvectors by any nonzero constants. $A(cx) = \lambda(cx)$ is still true.   
The eigenvectors in $X$ come in the same order as the eigenvalues in $\Lambda$.  
Some matrices have too few eigenvectors. Those matrices cannot be diagonalized.  
Eigenvectors $\bold{x}_1,\bold{x}_2, \dots,\bold{x}_n$ that correspond to distinct (all different) eigenvalues are linearly independent. An $n$ by $n$ matrix that has $n$ different eigenvalues (no repeated $A$'s) must be diagonalizable.   
#### Similar Matrices: Same Eigenvalues
All the matrices $A = BCB^{-1}$ are "similar." They all share the eigenvalues of $C$
#### Fibonacci Numbers 
Let $\bold{u}_k = \begin{bmatrix}F_{k+1} \\ F_k\end{bmatrix},\bold{u}_{k+1}=\begin{bmatrix}1&1  \\ 1 & 0 \end{bmatrix}\bold{u}_k$   
$\det (A-\lambda I) = 0, \lambda = \dfrac{1 \plusmn \sqrt{5}}{2}$  
Eigenvectors $\bold{x}_1 = (\lambda_1,1),\bold{x}_2= (\lambda_2,1)$  
$\bold{u}_0 = \dfrac{\bold{x}_1-\bold{x}_2}{\lambda_1-\lambda_2},\bold{u}_n = \dfrac{(\lambda_1)^n\bold{x}_1-(\lambda_2)^n\bold{x}_2}{\lambda_1-\lambda_2}$
#### Matrix Powers $A^k$
$$\bold{u}_{k+1}=A\bold{u}_k, \bold{u}_k = A^k\bold{u}_0 = \sum c_i(\lambda_i)^k\bold{x}_i$$  
$\bold{u}_0 = \begin{bmatrix} & &  \\ \bold{x}_1 & \cdots & \bold{x}_n\\ && \end{bmatrix}\begin{bmatrix} c_1  \\ \vdots \\ c_n \end{bmatrix} = X\bold{c},\bold{c} = X^{-1}\bold{u}_0$  
$A^k\bold{u}_0 = X\Lambda^kX^{-1}\bold{u}_0 = X\Lambda^k\bold{c} = \begin{bmatrix} & &  \\ \bold{x}_1 & \cdots & \bold{x}_n\\ && \end{bmatrix}\begin{bmatrix}(\lambda_1)^k & &  \\  & \ddots & \\ && (\lambda_n)^k\end{bmatrix}\begin{bmatrix} c_1  \\ \vdots \\ c_n \end{bmatrix}$
#### Nondiagonalizable Matrices
### 6.3 Systems of Differential Equations 
#### Solution of $\dfrac{d\bold{u}}{dt} = A\bold{u}$
Systems of $n$ equations $\dfrac{d\bold{u}}{dt} = A\bold{u}$ starting from the vector $\bold{u}(0) = \begin{bmatrix} \bold{u}_1(0)\\  \cdots \\ \bold{u}_n(0)\end{bmatrix}$ at $t=0$  
Choose $\bold{u} = e^{\lambda t}\bold{x}, A\bold{x} = \lambda \bold{x}$:  
$\dfrac{d\bold{u}}{dt} = \lambda e^{\lambda t}\bold{x}=A\bold{u}=\lambda e^{\lambda t}\bold{x}$  
1. Write $\bold{u}(0)$ as a combination $c_1\bold{x}_1 + \cdots + c_n\bold{x}_n$ of the eigenvectors of $A$.
2. Multiply each eigenvector $\bold{x}_i$; by its growth factor $e^{\lambda_i t}$
3. The solution is the same combination of those pure solutions $e^{\lambda t}\bold{x}$  
   $$\bold{u}(t) = c_1e^{\lambda_1 t}\bold{x}_1 + \cdots + c_ne^{\lambda_n t}\bold{x}_n$$
#### Second Order Equations
For $my''+by'+ky = 0$, substitute $y=e^{\lambda t}x$  
$m\dfrac{dy^2}{d^2t} + b\dfrac{dy}{dt} + y= 0 \rArr (m\lambda^2 + b\lambda + k)e^{\lambda t} = 0$  
Let $m=1,\bold{u} = (y,y')$  
$\begin{cases}\frac{dy}{dx} = y' \\ \frac{dy'}{dt} = -ky -by'\end{cases}$ converts to $\dfrac{d}{dt}\begin{bmatrix} y \\ y'\end{bmatrix}=\begin{bmatrix}0 & 1  \\ -k & -b \end{bmatrix}\begin{bmatrix} y \\ y'\end{bmatrix}=A\bold{u}$  
The determinant of $A-\lambda I$ is $\lambda^2 + b\lambda +k=0$  
$\bold{u}(t) = c_1e^{\lambda_1 t}\begin{bmatrix} 1 \\ \lambda_1\end{bmatrix}+ c_2e^{\lambda_2 t}\begin{bmatrix} 1 \\ \lambda_2\end{bmatrix}$
#### Difference Equations (optional)
#### Stability of 2 by 2 Matrices
$A$ is stable and $\bold{u}(t) \to 0$ when all eigenvalues $\lambda$. have negative real parts. The 2 by 2 matrix $A = \begin{bmatrix}a & b  \\ c & d \end{bmatrix}$ must pass two tests:  
$\lambda_1 + \lambda_2 < 0,$ The trace $T = a + d$ must be negative  
$\lambda_1\lambda_2 > 0,$ The determinant $D = ad-bc$ must be positive
#### The Exponential of a Matrix
$e^x = 1 + x + \dfrac{1}{2}x^2 + \dfrac{1}{6}x^3 + \cdots + \dfrac{1}{n!}x^n + \cdots$  
$e^{At} = I + At + \dfrac{1}{2}At^2+\dfrac{1}{6}At^3 + \cdots$  
Its derivative: $Ae^{At} =A + A^2t + \dfrac{1}{2}A^3t + \cdots$  
Its eigenvalues $e^{\lambda t}$: $(I + At + \dfrac{1}{2}At^2+ \cdots)\bold{x} =(1+\lambda t + \dfrac{1}{2}\lambda t^2 + \cdots)\bold{x}$  
The solution $\bold{u}(t) = e^{At}\bold{u}(0)$  
$e^{At}= I + X\Lambda X^{-1}t+\dfrac{1}{2}(X\Lambda X^{-1}t)(X\Lambda X^{-1}t)  + \cdots$  
$= X(I + \Lambda t + \dfrac{1}{2}\Lambda t + \cdots)X^{-1} = Xe^{\Lambda t}X^{-1}$  
$\bold{u}(t) = e^{At}\bold{u}(0)=Xe^{\Lambda t}X^{-1}\bold{u}(0)=\begin{bmatrix} && \\ \bold{x}_1& \cdots & \bold{x}_n \\ &&\end{bmatrix}\begin{bmatrix} e^{\lambda_1 t}&& \\ & \ddots &  \\ &&e^{\lambda_n t}\end{bmatrix}\begin{bmatrix} c_1 \\  \vdots\\ c_n\end{bmatrix}$  
1. $e^{At}$ always has the inverse $e^{-At}$. 
2. The eigenvalues of $e^{At}$ are always $e^{\lambda t}$. 
3. When $A$ is antisymmetric, $e^{At}$ is orthogonal. Inverse= transpose= $e^{-At}$.
### 6.4 Symmetric Matrices 
1. A symmetric matrix has only real eigenvalues.
2. The eigenvectors can be chosen orthonormal.
   
Every symmetric matrix has the factorization $S = Q\Lambda Q^T$ with real eigenvalues in $A$ and orthonormal eigenvectors in the columns of $Q$:  
$$
S = Q\Lambda Q^{-1}  = Q\Lambda Q^T, Q^T = Q^{-1}
$$
Suppose $S$ has complex eigenvectors $\lambda = a-ib$ and its conjugate $\bar{\lambda}$  
$S\bold{x} = \lambda \bold{x}, S\bold{\bar{x}}=\bar{\lambda}\bold{\bar{x}}$  
$\bold{\bar{x}}^TS=\bold{\bar{x}}^T\bar{\lambda}$  
$\bold{\bar{x}}^T(S\bold{x}) = \bold{\bar{x}}^T(\lambda \bold{x}),(\bold{\bar{x}}^TS)\bold{x}=(\bold{\bar{x}}^T\bar{\lambda})\bold{x}$  
$\bold{\bar{x}}^T(\lambda \bold{x})=(\bold{\bar{x}}^T\bar{\lambda})\bold{x}$  
$\bold{\bar{x}}^T\bold{x} > 0, \lambda = \bar{\lambda}$  
Suppose $S\bold{x}=\lambda_1\bold{x},S\bold{y}=\lambda_2\bold{y}$  
$(\lambda_1\bold{x})^T\bold{y} = (S\bold{x})^T\bold{y}=\bold{x}^TS^T\bold{y}=\bold{x}^T(S\bold{y})=\bold{x}^T(\lambda_2\bold{y})$  
$\lambda_1\bold{x}^T\bold{y}=\lambda_2\bold{x}^T\bold{y},\bold{x}^T\bold{y}=0$  
For 2x2 symmetric matrices. 
$$S = \begin{bmatrix}a & b  \\ b & c \end{bmatrix},\bold{x}_1=\begin{bmatrix}b  \\ \lambda_1-a \end{bmatrix},\bold{x}_2=\begin{bmatrix}\lambda_2-c\\ b \end{bmatrix}$$
$S = \lambda_1q_1q_1^T+\cdots+ \lambda_n q_nq_n^T, Sq_i = \lambda_i q_i$
#### Complex Eigenvalues of Real Matrices
For real matrices, complex $\lambda$s and $\bold{x}$'s come in "conjugate pairs."  
$$
A\bold{x}=\lambda x, A\bold{\bar{x}}=\bar{\lambda}\bar{\bold{x}}
$$
#### Eigenvalues versus Pivots
he number of positive eigenvalues of $S = S^T$ equals the number of positive pivots.   
Special case: $S$ has all $A_i > 0$ if and only if all pivots are positive.
#### All Symmetric Matrices are Diagonalizable 
### 6.5 Positive Definite Matrices 
For $S = \begin{bmatrix}a & b  \\ b & c \end{bmatrix}$, The eigenvalues of $S$ are positive if and only if $a> 0$ and $ac-b^2>0$  
The eigenvalues of $S$ are positive if and only if the pivots are positive $a> 0$ and $\dfrac{ac -b^2}{a}>0$
#### Energy-based Definition 
$S$ is positive definite if $\bold{x}^T S\bold{x} > 0$ for every nonzero vector $\bold{x}$  
$$
\bold{x}^T S\bold{x} = \begin{bmatrix}x & y \end{bmatrix}\begin{bmatrix}a & b  \\ b & c \end{bmatrix}\begin{bmatrix}x  \\ y \end{bmatrix} = ax^2+2bxy+cy^2 > 0
$$
If $S$ and $T$ are symmetric positive definite, so is $S + T$  
If the columns of $A$ are independent, then $S = A^T A$ is positive definite  
When a symmetric matrix $S$ has one of these five properties, it has them all :  
1. All $n$ pivots of $S$ are positive.  
2. All $n$ upper left determinants are positive.
3. All $n$ eigenvalues of $S$ are positive.
4. $\bold{x}^T S\bold{x}$ is positive except at $x = 0$. This is the energy-based definition.
5. $S$ equals $A^T A$ for a matrix $A$ with independent columns.
#### Positive Semidefinite Matrices
$\bold{x}^T S\bold{x}=0$
#### The Ellipse $ax^2 + 2bxy + cy^ 2 = 1$
$S = Q\Lambda Q^T$ is positive definite when all $\lambda_i > 0$. The graph of $\bold{x}^T S\bold{x} = 1$ is an ellipse:
$$
\begin{bmatrix}x & y \end{bmatrix}Q\Lambda Q^T\begin{bmatrix}x  \\ y \end{bmatrix} = \begin{bmatrix}X &Y \end{bmatrix}\Lambda \begin{bmatrix}X \\ Y \end{bmatrix}=\lambda_1X^2+\lambda_2Y^2=1
$$
The axes point along eigenvectors of $S$. The half-lengths are $\dfrac{1}{\sqrt{\lambda_1}}$ and $\dfrac{1}{\sqrt{\lambda_2}}$.
#### Important Application: Test for a Minimum
$F ( x, y)$ has a minimum if a $\dfrac{\partial F}{\partial x}=\dfrac{\partial F}{\partial y}=0$ and $S=\begin{bmatrix}\frac{\partial^2 F}{\partial x^2} & \frac{\partial^2 F}{\partial y}   \\\frac{\partial^2 F}{\partial x\partial y}  & \frac{\partial^2 F}{\partial y^2}  \end{bmatrix}$ is positive definite