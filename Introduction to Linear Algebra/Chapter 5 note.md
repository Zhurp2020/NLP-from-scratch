# Introduction to Linear Algebra
## Chapter 5 Determinants
### 5.1 The Properties of Determinants
When $A$ is invertible, the determinant of $A^{-1}$ is $\dfrac{1}\det{A}$.  
$A = \begin{bmatrix}a & b  \\ c & d \end{bmatrix},A^{-1} = \dfrac{1}{ad-bc}\begin{bmatrix}d & -b  \\ -c & a \end{bmatrix}$  
The product of the pivots is the determinant: $a(d-\dfrac{c}{a}b) = ad-bc$  

#### The Properties of the Determinant 
1. The determinant of the $n$ by $n$ identity matrix is 1
   $$\begin{vmatrix} 1 & 0 \\ 0 & 1\end{vmatrix} =1$$
2. The determinant changes sign when two rows are exchanged (sign reversal):  
   $$\begin{vmatrix} a & b \\ c & d\end{vmatrix} = -\begin{vmatrix} c & d \\ a & b\end{vmatrix} $$ 
3. The determinant is a linear function of each row separately
$$\begin{vmatrix} ta & tb \\ c & d\end{vmatrix} = t\begin{vmatrix} a & b \\ c & d\end{vmatrix} \\ \begin{vmatrix} a + a' & b+b' \\ c & d\end{vmatrix} = \begin{vmatrix} a & b \\ c & d\end{vmatrix}+ \begin{vmatrix} a' & b' \\ c & d\end{vmatrix}$$  
4. If two rows of $A$ are equal, then $\det{A} = 0$.  
   $$\begin{vmatrix} a & b \\ a & b\end{vmatrix} = 0$$ 
5.  Subtracting a multiple of one row from another row leaves $\det{A}$ unchanged.  
   $$\begin{vmatrix} a & b \\c-la & d-lb\end{vmatrix} = \begin{vmatrix} a & b \\c & d\end{vmatrix}$$ 
6.  A matrix with a row of zeros has $\det{A}=0$    
   $$\begin{vmatrix} a & b \\0 & 0\end{vmatrix} = 0$$ 
7.  If $A$ is triangular then $\det{A} = a_{11}a_{22} \cdots a_{nn} =$ product of diagonal entries.   
$$\begin{vmatrix} a & b \\ 0 &d\end{vmatrix} = \begin{vmatrix} a & 0 \\ b& d\end{vmatrix} =ad$$   
1. If $A$ is singular then $\det{A}=0$. If $A$ is invertible then $\det{A}\ne 0$   
   $\begin{bmatrix}a & b  \\ c & d \end{bmatrix}$ is singular if and only if $ad-bc=0$
2.  The determinant of $AB$ is $\det{A}$ times $\det{B}$: $|AB|$ = $|A||B|$  
      $$\begin{vmatrix} a & b \\ c &d\end{vmatrix} \begin{vmatrix} p & q \\ r &s\end{vmatrix} = \begin{vmatrix} ap+br & aq+bs \\ cp+dr& cq+ds\end{vmatrix} $$  
3.  The transpose $A^T$ has the same determinant as $A$.  
    $$\begin{vmatrix} a & b \\ c &d\end{vmatrix} = \begin{vmatrix} a & c \\ b& d\end{vmatrix} =ad-bc$$  
### 5.2 Permutations and Cofactors 
#### The Pivot Formula  
$\det A = \det L \det U = \plusmn d_1d_2\cdots d_n$   
$k$th pivot is $\dfrac{\det A_k}{\det A_{k-1}}$
#### The Big Formula for Determinants
$\det A = \sum (\det P)a_{1\alpha}a_{2\beta}\cdots a_{n\omega}, P = \{\alpha, \beta, \cdots, \omega\}$is the permutation matrices. 
#### Determinant by Cofactors
The determinant is the dot product of any row $i$ of $A$ with its cofactors using other rows:  
$\det A = a_{i1}C_{i1} + a_{i2}C_{i2} + \cdots a_{in}C_{in}$    
Each cofactor $C_{ij}$ (order $n - 1$, without row $i$ and column $j$) includes its correct sign:  
$C_{ij}=(-1)^{i+j}\det M_{ij}$
### 5.3 Cramer's Rule, Inverses, and Volumes
If $\det{A}$ is not zero, $A\bold{x} = \bold{b}$ is solved by determinants:  
$$x_1 = \dfrac{\det B_1}{\det A}, x_1 = \dfrac{\det B_n}{\det A}$$
The matrix $B_j$ has the $j$th column of $A$ replaced by the vector $\bold{b}$.   
The $i, j$ entry of $A^{-1}$ is the cofactor $C_{ji}$ (not $C_{ij}$) divided by $\det A$  
$$A^{-1}_{ij} = \dfrac{C_{ji}}{\det A}, A^{-1} = \dfrac{C^T}{\det A}$$
#### Area of a Triangle
The tnangle with corners $(x_1, y_1)$ and $(x2, y_2)$ and $(x_3, y_3)$ has area $=\dfrac{1}{2}\begin{vmatrix}x_1 & y_1 & 1 \\ x_2 & y_2 & 1 \\  x_3 & y_3 & 1 \\\end{vmatrix}$. When $(x3, y3) = (0, 0)$, area $=\dfrac{1}{2}\begin{vmatrix}x_1 & y_1 \\ x_2 & y_2   \\\end{vmatrix}$
#### The Cross Product
The cross product of $\bold{u} = ( u_1, u_2, u_3)$ and $\bold{v} = ( v_1, v_2, v_3)$ is a vector $\bold{u} \times \bold{v} = \begin{vmatrix}\bold{i}& \bold{j} & \bold{k} \\ u_1& u_2&u_3 \\  v_1& v_2&v_3 \\\end{vmatrix} = (u_2v_3-u_3v_2)\bold{i}+(u_3v_1-u_1v_3)\bold{j}+(u_1v_2-u_2v_1)\bold{k}$  
This vector $\bold{u} \times \bold{v}$ is perpendicular to $\bold{u}$ and $\bold{v}$. The cross product $\bold{v} \times \bold{u}$ is $-(\bold{u} \times \bold{v})$.  
When $\bold{u}$ and $\bold{v}$ are parallel, the cross product is zero.   
$||\bold{u} \times \bold{v}||=||\bold{u}||||\bold{v}|||\sin \theta|$
#### Triple Product = Determinant = Volume
$(\bold{u} \times \bold{v} )\cdot \bold{w}= \begin{vmatrix}w_1&w_2&w_3 \\ u_1& u_2&u_3 \\  v_1& v_2&v_3 \\\end{vmatrix}$