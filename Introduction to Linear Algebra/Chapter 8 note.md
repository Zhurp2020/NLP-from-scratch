# Introduction to Linear Algebra
## Chapter 8 Linear Transformations
### 8.1 The Idea of a Linear Transformation
A transformation $T$ assigns an output $T(v)$ to each input vector $\bold{v}$ in $V$. The transformation is linear if it meets these requirements for all $\bold{v}$ and $\bold{w}$:   
(a) $T(\bold{v} + \bold{w}) = T(\bold{v}) + T(\bold{w})$ (b) $T(c\bold{v}) = cT(\bold{v})$
#### Lines to Lines, Triangles to Triangles, Basis Tells All 
The rule of linearity extends to combinations of three vectors or $n$ vectors   
Suppose you know $T(\bold{v})$ for all vectors $\bold{v}_1,\bold{v}_2, \dots,\bold{v}_n$ in a basis. Then you know $T(\bold{u})$ for every vector $\bold{u}$ in the space
#### Examples of Transformations (mostly linear)
#### Linear Transformations of the Plane
### 8.2 The Matrix of a Linear Transformation
Suppose we know $T(\bold{v})$ for the input basis vectors $\bold{v}_1$ to $\bold{v}_n$.   
Columns 1 to $n$ of the matrix will contain those outputs $T(\bold{v}_1)$ to $T(\bold{v}_n)$­.  
$A$ times $c =$ matrix times vector = combination of those $n$ columns.   
$Ac$ is thecorrect combination $c_1T(\bold{v}_1)  + \cdots + c_nT(\bold{v}_n) = T(\bold{v})$.  
#### Change of Basis
When the input basis is in the columns of a matrix $V$, and the output basis is in the columns of $W$, the change of basis matrix for $T = I$ is $B = W^{-1} V$.
#### Construction of the Matrix
$T(\bold{v}_1)$ is a combination $a_{11}\bold{w}_1,\dots,a_{m1}\bold{w}_m$ of the output basis for $W$.   
The $j$th column of $A$ is found by applying $T$ to the $j$th basis vector $\bold{v}_1$, $T(\bold{v}_1) = $ combination of output basis vectors $= a_{11}\bold{w}_1,\dots,a_{mj}\bold{w}_m$. 
#### Matrix Products $AB$ Match Transformations $TS$
The linear transformation $TS$ starts with any vector $\bold{u}$ in $U$, goes to $S(\bold{u})$ in $V$ and then to $T(S(u))$ in $W$. The matrix $AB$ starts with any $\bold{x}$ in $R^p$, goes to $B\bold{x}$ in $R^n$ and then to $AB\bold{x}$ in $R^m$. The matrix $AB$ correctly represents $TS$
#### Choosing the Best Bases
$A_{new} = B^{-1} AB$ in the new basis of $\bold{b}$'s is similar to $A$ in the standard basis  
**Eigenvectors**: If $T$ transforms $R^n$ to $R^n$, its matrix $A$ is square. But using the standard basis, that matrix $A$ is probably not diagonal. If there are $n$ independent eigenvectors, choose those as the input and output basis. In this good basis, the matrix for $T$ is the diagonal eigenvalue matrix $A$.   
**Singular vectors**: The SVD says that $U^{-1}AV = \Sigma$ The right singular vectors $\bold{v}_1,\bold{v}_2, \dots,\bold{v}_n$ will be the input basis. The left singular vectors $\bold{u}_1,\bold{u}_2, \dots,\bold{u}_n$ will be the output basis. By the rule for matrix multiplication, the matrix for the same transformation in these new bases is $B_{out}^{-1}AB_{in} = U^{-1}AV=\Sigma$
### 8.3 The Search for a Good Basis
If $A$ is the matrix for a transformation $T$ in the standard basis, then $B_{out}^{-1}AB$ is the matrix in the new bases.  
Here are four important choices for vectors:
1. $B_{out} = B_{in} =$ eigenvectors matrix $X$, $X^{-1}AX = \Lambda$ of eigenvalues. 
2. $B_{out} = V, B_{in} =U$ singular vectors of $A$, $U^{-1}AV = \Sigma$ of eigenvalues. 
3. $B_{out} = B_{in} =$ generalized eigenvectors matrix, $B^{-1}AB = J$ Jordan forms. 
4. $B_{out} = B_{in} =$ Fourier matrix $F$ Then $F\bold{x}$ is a discrete Fourier Transform of $x$
#### The Jordan Form
If $A$ has $s$ independent eigenvectors, it is similar to a matrix $J$ that has $s$ Jordan blocks $J_1,\dots , J_s$ on its diagonal. Some matrix $B$ puts $A$ into Jordan form:   
$$
B^{-1}AB = J = \begin{bmatrix}
    J_1 & & \\ & \ddots & \\ && J_s
\end{bmatrix}
$$
Each block $J_i$ has one eigenvalue $\lambda_i$, one eigenvector, and 1 's just above the diagonal  
$$
J_i = \begin{bmatrix}
    J_1 &1 & & \\ & \cdot& \cdot &  \\ & & \cdot &  1\\ & & &J_s
\end{bmatrix}
$$
Matrices are similar if they share the same Jordan form $J$-not otherwise.
#### Bases for Function Space
Inner product $(f, g) =\int f(x)g(x) dx$   
Complex inner product $(f, g) =\int \bar{f ( x)}  g( x) dx$   
Weighted inner product $(f, g ) =\int w(x)f(x) g(x)dx$
#### Orthogonal Bases for Function Space
1. The Fourier basis: $1,\sin x, \cos x, \sin 2x, \cos 2x, \dots$
2. The Legendre basis: $1, x, x^2-\frac{1}{3}, x^3-\frac{3}{5}x,\dots$  
3. The Chebyshev basis: $1, x, 2x^2-1, 4x^3-3x,\ddots$
#### Legendre Polynomials and Chebyshev Polynomials