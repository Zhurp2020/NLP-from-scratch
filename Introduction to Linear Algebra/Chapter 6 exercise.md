# Introduction to Linear Algebra
## Chapter 6 Eigenvalues and Eigenvectors
### 6.1 Introduction to Eigenvalues
1. The example at the start of the chapter has powers of this matrix $A$:  
   $$A =\begin{bmatrix}0.8 & 0.3  \\ 0.2 & 0.7\end{bmatrix}, A^2 = \begin{bmatrix}0.7 & 0.45  \\ 0.3 & 0.55\end{bmatrix}, A^{\infty} =\begin{bmatrix}0.6 & 0.4  \\ 0.6 & 0.4\end{bmatrix}$$
    Find the eigenvalues of these matrices. All powers have the same eigenvectors.   
    (a) Show from $A$ how a row exchange can produce different eigenvalues.  
    (b) Why is a zero eigenvalue not changed by the steps of eliminations  
    $\det (A - \lambda I) = (0.8-\lambda)(0.7 - \lambda) - 0.06 = 0$  
    $\lambda^2 - 1.5\lambda +0.5 = 0$  
    $(\lambda - 1)(\lambda - 0.5) = 0$  
    $\lambda_1 = 1, \lambda_2 = 0.5$  
    $\begin{bmatrix}-0.2& 0.3  \\ 0.2 & -0.3 \end{bmatrix}\bold{x}_1 = \begin{bmatrix}0 \\ 0 \end{bmatrix}, \bold{x}_1 =\begin{bmatrix}1.5 \\ 1 \end{bmatrix}$  
    $\begin{bmatrix}0.3& 0.3  \\ 0.2 & 0.2 \end{bmatrix}\bold{x}_1 = \begin{bmatrix}0 \\ 0 \end{bmatrix}, \bold{x}_2 =\begin{bmatrix}1\\ -1 \end{bmatrix}$
    $\det (B-\lambda I) =  (0.2-\lambda)(0.3 - \lambda) - 0.56 = 0$  
    $\lambda^2-0.5\lambda -0.5 = 0$  
    $\lambda_1 = -0.5, \lambda_2 = 1$  
    (b) the determinant stays zero, means the product of all eigenvalues must be zero
#### Challenge Problems 
33. Show that $\bold{u}$ is an eigenvector of the rank one 2 x 2 matrix $A = \bold{u}\bold{v}^T$. Find both eigenvalues of $A$. Check that $\lambda_1 + \lambda_2$ agrees with the trace $u_1 v_1 + u_2v_2$.  
    $A = \begin{bmatrix}u_1 v_1 & u_1 v_2  \\ u_2 v_1 & u_2v_2 \end{bmatrix}$   
    $\det (A-\lambda I)=(u_1 v_1-\lambda)(u_2 v_2-\lambda) - u_1 v_2u_2 v_1=0$  
    $\lambda^2 -(u_2 v_2+u_1 v_1)\lambda = 0$  
    $\lambda_1 = 0,\lambda_2=u_2 v_2+u_1 v_1$   
    $A\bold{u} = \bold{u}\bold{v}^T\bold{u} = (\bold{v}^T\bold{u})\bold{u} = (u_2 v_2+u_1 v_1)\bold{u} = \lambda_2\bold{u}$
### 6.2 Diagonalizing a Matrix
Questions 1-7 are about the eigenvalue and eigenvector matrices $\Lambda$ and $X$
1. (a) Factor these two matrices into $A = X\Lambda X^{-1}$  
   $A = \begin{bmatrix}1 & 2  \\ 0 &3 \end{bmatrix}$ and $A = \begin{bmatrix}1 & 1  \\ 3 &3 \end{bmatrix}$  
   (b) If $A = X\Lambda X^{-1}$ then $A^3=, A^{-1} =$  
   (a) $\det (A-\lambda I) = (1-\lambda)(3-\lambda) = \lambda^2-4\lambda+3=0$  
   $\lambda_1 = 3,\lambda_2=1$  
   $\begin{bmatrix}-2 & 2  \\ 0 &0 \end{bmatrix}\bold{x}_1=0,\bold{x}_1 = (1,-1)$  
   $\begin{bmatrix}0 & 2  \\ 0 &2 \end{bmatrix}\bold{x}_2=0,\bold{x}_2 = (1,0)$  
   $A = \begin{bmatrix}1 & -1  \\ 1 &0 \end{bmatrix}\begin{bmatrix}3 & 0  \\ 0 &1 \end{bmatrix}\begin{bmatrix}0 & 1  \\ -1 &1\end{bmatrix}$  
   $\det (A-\lambda I) = (1-\lambda)(3-\lambda) -3= \lambda^2-4\lambda=0$  
   $\lambda_1 = 4,\lambda_2=0$  
   $\begin{bmatrix}-3 & 1  \\ 3 &-1 \end{bmatrix}\bold{x}_1=0,\bold{x}_1 = (1,3)$  
   $\begin{bmatrix}1 & 1  \\ 3 &3 \end{bmatrix}\bold{x}_2=0,\bold{x}_2 = (1,1)$  
   $A = \begin{bmatrix}1 & 1  \\ 3 &1 \end{bmatrix}\begin{bmatrix}4 & 0  \\ 0 &0 \end{bmatrix}\begin{bmatrix}-\frac{1}{2} & \frac{1}{2}  \\ \frac{3}{2} &-\frac{1}{2}\end{bmatrix}$  
   (b)$X\Lambda^3 X^{-1}$  
   $A^{-1}=(X\Lambda X^{-1})^{-1} =(X^{-1})^{-1}(X\Lambda)^{-1} =X\Lambda^{-1}X^{-1}$

Questions 8-10 are about Fibonacci and Gibonacci numbers. 

8. Diagonalize the Fibonacci matrix by completing $X^{-1}:$
   $$
   \begin{bmatrix}1 & 1  \\ 1 &0 \end{bmatrix} = \begin{bmatrix}\lambda_1 & \lambda_2  \\ 1 &1 \end{bmatrix}\begin{bmatrix}\lambda_1 & 0\\ 0 &\lambda_2 \end{bmatrix}\begin{bmatrix} & \\  & \end{bmatrix}
   $$
   Do the multiplication $X\Lambda^kX^{-1}\begin{bmatrix}1\\0\end{bmatrix}$ to find its second component. This is the $k$ th Fibonacci number $F_k = \dfrac{\lambda_1^k-\lambda_2^k}{\lambda_1-\lambda_2}$  
   $X^{-1}=\dfrac{1}{\lambda_1-\lambda_2}\begin{bmatrix}1 & -\lambda_2\\ -1 &\lambda_1 \end{bmatrix}$  
   $X\Lambda^kX^{-1}\begin{bmatrix}1\\0\end{bmatrix} = \begin{bmatrix}\lambda_1^{k+1} & \lambda_2^{k+1}\\ \lambda_1^k&\lambda_2^k \end{bmatrix}\begin{bmatrix}\frac{1}{\lambda_1-\lambda_2} \\ -\frac{1}{\lambda_1-\lambda_2}  \end{bmatrix} = \begin{bmatrix}\frac{\lambda_1^{k+1}-\lambda_2^{k+1}}{\lambda_1-\lambda_2} \\ \frac{\lambda_1^{k}-\lambda_2^{k}}{\lambda_1-\lambda_2}  \end{bmatrix}$

Questions 11-14 are about diagonalizability. 

11. True or false: If the eigenvalues of $A$ are 2, 2, 5 then the matrix is certainly   
(a) invertible (b) diagonalizable (c) not diagonalizable.  
  (a),(c)

Questions 15-19 are about powers of matrices. 
15. $A^k = X \Lambda^k X^{-1}$ approaches the zero matrix as $k \to \infty$ if and only if every $\lambda$ has absolute value less than *1* Which of these matrices has $A^k\to\bold{0}$?   
   $$A_1=\begin{bmatrix}0.6 & 0.9  \\ 0.4 & 0.1 \end{bmatrix}, A_2=\begin{bmatrix}0.6 & 0.9  \\ 0.1 & 0.6 \end{bmatrix}$$
   $\det (A_1-\lambda I) = (0.6-\lambda)(0.1-\lambda)-0.36=0$  
   $\lambda^2-0.7\lambda+0.24 =0$  
   $\lambda_1=0.6,\lambda_2=0.1$  
   $\det (A_2-\lambda I) = (0.6-\lambda)(0.6-\lambda)-0.9=0$  
   $\lambda^2-1.2\lambda-0.54 =0$  
   $\lambda=\dfrac{1.2\plusmn\sqrt{3.6}}{2}$  
   $A_1^k \to 0$
#### Challenge Problems
34. The $n$th power of rotation through $\theta$ is rotation through $n\theta$:  
    $$
    A^n = \begin{bmatrix}\cos\theta & -\sin\theta \\ \sin\theta& \cos\theta \end{bmatrix}^n=\begin{bmatrix}\cos n\theta & -\sin n\theta \\ \sin n\theta& \cos n\theta\end{bmatrix}
    $$
    Prove that neat formula by diagonalizing $A = X \Lambda X ^{-1}$. The eigenvectors (columns of $X$) are $(1,i)$ and $(i, 1)$. You need to know Euler's formula $e^{i\theta} = \cos\theta + i\sin\theta.$    
    $\det (A-\lambda I) = \lambda^2-2\cos\theta\lambda+1=0$  
    $\lambda=\dfrac{2\cos\theta\plusmn\sqrt{4\cos^2\theta-4}}{2} =\cos\theta\plusmn\sqrt{\cos^2\theta-1}=\cos\theta \plusmn i\sin\theta$  
    $A = \begin{bmatrix}1 & i \\ i& 1 \end{bmatrix} \begin{bmatrix}e^{-i\theta} & 0\\ 0& e^{i\theta} \end{bmatrix}\dfrac{1}{2}\begin{bmatrix}1 & -i \\ -i& 1 \end{bmatrix}$  
    $A^n = \dfrac{1}{2}\begin{bmatrix}e^{-i\theta n} & ie^{i\theta n} \\ ie^{-i\theta n}& e^{i\theta n} \end{bmatrix}\begin{bmatrix}1 & -i \\ -i& 1 \end{bmatrix}$  
    $= \dfrac{1}{2}\begin{bmatrix}e^{-i\theta n} + e^{i\theta n}& -ie^{-i\theta n} + ie^{i\theta n}\\ ie^{-i\theta n}-ie^{i\theta n}& e^{-i\theta n} + e^{i\theta n}\end{bmatrix}$  
    $e^{-i\theta n} + e^{i\theta n}= \cos n\theta -i\sin n\theta + \cos n\theta + i\sin\theta=2\cos\theta$  
    $-ie^{-i\theta n} + ie^{i\theta n}=-i(\cos n\theta -i\sin n\theta - \cos n\theta -i\sin n\theta) = -2\sin\theta$  
   $A^n = \begin{bmatrix}\cos n\theta & -\sin n\theta \\ \sin n\theta& \cos n\theta\end{bmatrix}$
### 6.3 Systems of Differential Equations
1. Find two $\lambda$'s and $\bold{x}$'s so that $\bold{u}= e^{\lambda t}$ solves  
   $$\dfrac{d\bold{u}}{dt} = \begin{bmatrix}4 & 3  \\ 0 & 1 \end{bmatrix}\bold{u}$$  
   What combination $\bold{u} =c_1e^{\lambda_1 t}\bold{x}_1 +  c_2e^{\lambda_2 t}\bold{x}_2$ starts from $\bold{u}(0) = (5, -2)$?   
   $\det (A-\lambda I) =(4-\lambda)(1-\lambda) =\lambda^2-5\lambda+4=0$  
   $\lambda_1=4,\bold{x}_1=(1,0)$  
   $\lambda_2=1,\bold{x}_2=(1,-1)$  
   $\bold{u}=c_1e^{4t}\begin{bmatrix}1 \\0 \end{bmatrix}+c_2e^{t}\begin{bmatrix}1 \\-1 \end{bmatrix}$  
   $c_1 =3,c_2=2$

Questions 10-13 reduce second-order equations to first-order systems for $(y, y')$

10. Find $A$ to change the scalar equation $y'' = 5y' + 4y$ into a vector equation for $\bold{u}= (y, y')$:  
   What are the eigenvalues of $A$? Find them also by substituting $y = e^{\lambda t}$ into $y'' = 5y' + 4y$.   
   $\dfrac{d\bold{u}}{dt} = \begin{bmatrix}y' \\y'' \end{bmatrix} = \begin{bmatrix}0 & 1\\4 & 5 \end{bmatrix}\begin{bmatrix}y \\y' \end{bmatrix} = A\bold{u}$  
   $\det (A-\lambda I) = \lambda^2-5\lambda -4=0$  
   $\lambda = \dfrac{5\plusmn \sqrt{41}}{2}$  
   $\lambda^2y = 5\lambda y + 4y, \lambda ^2-5\lambda -4=0$  

Questions 18-27 are about the matrix exponential eAt .

18. Write five terms of the infinite series for $e^{At}$. Take the $t$ derivative of each term. Show that you have four terms of $Ae^{At}$. Conclusion: $e^{At}\bold{u}_0$ solves $\bold{u}' = A\bold{u}$.  
    $e^{At} = I + At + \dfrac{1}{2}At^2+\dfrac{1}{6}At^3+\dfrac{1}{24}At^4$  
    $\dfrac{d}{dt}e^{At} = A + At^+\dfrac{1}{2}At^2+\dfrac{1}{6}At^3$
#### Challenge Problems
28. Centering $y'' = -y$ in Example 3 will produce $Y_{n+1} - 2Y_n + Y_{n-1} = -(\Delta t)^2Y_n$ This can be written as a one-step difference equation for $U = (Y, Z)$:  
    $$\begin{cases}
      Y_{n+1} = Y_n + \Delta t Z_n  \\
      Z_{n+1} = Z_n - \Delta t Y_{n+1} 
    \end{cases}$$
    $$\begin{bmatrix}1 & 0\\\Delta t & 1 \end{bmatrix}\begin{bmatrix}Y_{n+1}\\Z_{n+1}\end{bmatrix} = \begin{bmatrix}1 & \Delta t\\0 & 1 \end{bmatrix}\begin{bmatrix}Y_n\\Z_n\end{bmatrix}$$
    Invert the matrix on the left side to write this as $U_{n+1} = AU_n$. Show that $\det A = 1$. Choose the large time step $\Delta t = 1$ and find the eigenvalues $\lambda_1$ and $\lambda_2=\bar{\lambda_1}$ of $A$:  
    $A= \begin{bmatrix}1 & 1\\-1& 0 \end{bmatrix}$ has $|\lambda_1| = |\lambda_2| = 1$. Show that $A^6$ is exactly $I$  
    After 6 steps to $t= 6, U_6$ equals $U _0$. The exact $y =\cos t$ returns to 1 at $t = 2\pi r$  
    $\begin{bmatrix}Y_{n+1}\\Z_{n+1}\end{bmatrix} = \begin{bmatrix}1 & 0\\-\Delta t & 1 \end{bmatrix}\begin{bmatrix}1 & \Delta t\\0 & 1 \end{bmatrix}\begin{bmatrix}Y_n\\Z_n\end{bmatrix}=\begin{bmatrix}1 & \Delta t\\-\Delta t & -\Delta  t^2 +1 \end{bmatrix}\begin{bmatrix}Y_n\\Z_n\end{bmatrix}$    
    $\det A = 1$  
    $\Delta t = 1, \det (A-\lambda I) = \lambda^2 -\lambda+1=0$  
    $\lambda = \dfrac{1\plusmn \sqrt{3}i}{2}$  
    $(\frac{1}{2}+\frac{\sqrt{3}}{2}i)x + y = 0,(\frac{1}{2}-\frac{\sqrt{3}}{2}i)x + y = 0 \\ x +(\frac{1}{2}-\frac{\sqrt{3}}{2}i)y=0,x +(\frac{1}{2}+\frac{\sqrt{3}}{2}i)y=0$    
    $X = \begin{bmatrix}-\frac{1}{2}+\frac{\sqrt{3}}{2}i & -\frac{1}{2}-\frac{\sqrt{3}}{2}i\\1&1\end{bmatrix}$
    $A^6 = X\begin{bmatrix}1 & 0\\0&1\end{bmatrix}X^{-1} = I$
### 6.4 Symmetric Matrices 
1. Which of these matrices $ASB$ will be symmetric with eigenvalues 1 and -1?  
   $\begin{bmatrix}1 & 0  \\ 1 & 1 \end{bmatrix}\begin{bmatrix}1 & 0 \\ 0 & -1 \end{bmatrix}\begin{bmatrix}1 & 1  \\ 0 & 1 \end{bmatrix}$  
    $\begin{bmatrix}1 & 0  \\ 1 & 1 \end{bmatrix}\begin{bmatrix}1 & 0 \\ 0 & -1 \end{bmatrix}\begin{bmatrix}1 & 0  \\ -1 & 1 \end{bmatrix}$
    $\begin{bmatrix}0 & -1  \\ 1 & 0 \end{bmatrix}\begin{bmatrix}1 & 0 \\ 0 & -1 \end{bmatrix}\begin{bmatrix}0 & 1  \\ -1 & 0 \end{bmatrix}$  
    $B = A^T$ doesn't do it. $B = A^{-1}$ doesn't do it. $B=A^T=A^{-1}$ will succeed. So $B$ must be a symmetric matrix.
#### Challenge Problems 
30. For complex matrices, the symmetry $S^T = S$ that produces real eigenvalues must change in Section 9.2 to $\bar{S}^T = S$. From $\det(S - \lambda I) = 0$, find the eigenvalues of the 2 by 2 Hermitian matrix $S =\begin{bmatrix}4 & 2+i \\ 2-i & 0\end{bmatrix} = \bar{S}^T$  
    $(4-\lambda)(-\lambda)-5=0$  
    $\lambda^2-4\lambda -5=0,\lambda_1=5,\lambda_2=-1$
### 6.5 Positive Definite Matrices
Problems 1-13 are about tests for positive definiteness.
1. Suppose the 2 by 2 tests $a > 0$ and $ac - b^2 > 0$ are passed. Then $c > \dfrac{b^2}{a} > 0$.   
(i) $\lambda_1$ and $\lambda_2$ have the same sign because their product $\lambda_1\lambda_2$ equals $ac-b^2$ .    
(i) That sign is positive because $\lambda_1+\lambda_2$ equals $a+c$  
Conclusion: The tests $a > 0, ac - b^2 > 0$ guarantee positive eigenvalues $\lambda_1,\lambda_2$.

Problems 14-20 are about applications of the tests.

14. If $S$ is positive definite then $S^{-1}$ is positive definite. Best proof: The eigenvalues of $S^{-1}$ are positive because *the eigenvalues of the inverse of a matrix are the reciprocals of the eigenvalues of the matrix*. Second proof (only for 2 by 2):   
The entries of $S^{-1}=\dfrac{1}{ac-b^2}\begin{bmatrix}c & -b  \\ -b & a \end{bmatrix}$ 
pass the determinant tests  $c>0, ac-b^2>0$

Problems 21-24 use the eigenvalues; 

21. For which $s$ and $t$ do $S$ and $T$ have all $\lambda>0$ (therefore positive definite)?  
    $S = \begin{bmatrix}s & -4 & -4 \\ -4 & s & -4 \\ -4 & -4 & s \end{bmatrix},T= \begin{bmatrix}t& 3 & 0 \\ 3 & t & 4 \\ 0& 4 & t \end{bmatrix}$  
    $s>0, \dfrac{s^2-16}{s}>0, s(s^2-16)+4(-4s-16)-4(16+4s)>0$  
    $s(s^2-16)-16(4+s)-16(4+s)>0$  
    $s^2-4s-32>0$   
    $s>8$  
    $t>0, t^2-9>0, t(t^2-16)-9t>0$  
    $t>5$

Problems 25-27 are based on pivots.

25. With positive pivots in $D$, the factorization $S = LDL^T$ becomes $L\sqrt{D}\sqrt{D}L^T$. (Square roots of the pivots give $D = \sqrt{D}\sqrt{D}$.) Then $C = \sqrt{D}L^T$ yields the Cholesky factorization $A = C^T C$ which is "symmetrized $L U$":  
    From $C=\begin{bmatrix}3 &1  \\ 0& 2 \end{bmatrix}$ find $S$.  
    From  $S=\begin{bmatrix}4 &8  \\ 8& 25 \end{bmatrix}$ find $C=chol(S)$  
    $S = \begin{bmatrix}3 &0 \\ 1& 2 \end{bmatrix}\begin{bmatrix}3 &1  \\ 0& 2 \end{bmatrix}=\begin{bmatrix}9 &3  \\ 3& 5 \end{bmatrix}$  
   $S\rArr \begin{bmatrix}4 &8  \\ 0& 9 \end{bmatrix}$  
   $S = \begin{bmatrix}1 &0 \\ 2& 1 \end{bmatrix}\begin{bmatrix}4 &8  \\ 0& 9 \end{bmatrix}=\begin{bmatrix}1 &0 \\ 2& 1 \end{bmatrix}\begin{bmatrix}4 &0  \\ 0& 9 \end{bmatrix}\begin{bmatrix}1 &2  \\ 0& 1 \end{bmatrix}$  
   $C=\begin{bmatrix}2 &0  \\ 0& 3 \end{bmatrix}\begin{bmatrix}1 &2  \\ 0& 1 \end{bmatrix}=\begin{bmatrix}2 &4\\ 0& 3 \end{bmatrix}$  
#### Challenge Problems 
32. A group of nonsingular matrices includes $AB$ and $A^{-1}$ if it includes $A$ and $B$. "Products and inverses stay in the group." Which of these are groups (as in 2.7.37)?  Invent a "subgroup " of two of these groups (not $I$ by itself= the smallest group).   
(a) Positive definite symmetric matrices $S$.    
(b) Orthogonal matrices $Q$.  
(c) All exponentials $e^{t A}$ of a fixed matrix $A$.  
(d) Matrices $P$ with positive eigenvalues.   
(e) Matrices $D$ with determinant 1  
(b) and (c)  