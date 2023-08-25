# Introduction to Linear Algebra
## Chapter 2 Solving Linear Equations
### 2.1 Vectors and Linear Equations
#### Three Equations in Three Unknowns
#### The Matrix Form of the Equations
Matrix-vector multiplication $A\bold{x}$ can be computed by dot products, a row at a time. But $A\bold{x}$ must be understood as a combination of the columns of $A$.  
Column picture: $A\bold{x} = \bold{b}$ asks for a combination of columns to produce $\bold{b}$  
Row picture: Each equation in $A\bold{x} = \bold{b}$ gives a line $(n = 2)$ or a plane $(n = 3)$ or a "hyperplane" $(n > 3)$. They intersect at the solution or solutions, if any.
#### Matrix Notation
#### Multiplications in MATLAB
#### Programming Languages for Mathematics and Statistics
### 2.2 The Idea of Elimination
To eliminate $x$, Subtract a multiple of equation 1 from equation 2.   
Pivot: first nonzero in the row that does the elimination
Multiplier: (entry to eliminate) divided by (pivot)
#### Breakdown of Elimination
Singular equations have no solution or infinitely many solutions.  
#### Three Equations in Three Unknowns
#### Elimination from $A$ to $U$
Column 1. Use the first equation to create zeros below the first pivot.   
Column 2. Use the new equation 2 to create zeros below the second pivot.   
Columns 3 to $n$. Keep going to find all n pivots and the upper triangular $U$
### 2.3 Elimination Using Matrices
#### Matrices times Vectors and $A\bold{x} = \bold{b}$  
#### The Matrix Form of One Elimination Step
The identity matrix has 1 's on the diagonal and otherwise O's. Then $I\bold{b} = \bold{b}$ for all $\bold{b}$. The elementary matrix or elimination matrix $E_{ij}$ has the extra nonzero entry $-l$ in the $i, j$ position. Then $E_{ij}$ subtracts a multiple $l$ of row $j$ from row $i$.
#### Matrix Multiplication
$AB = A[\bold{b_1},\bold{b_2},\bold{b_3}] = [A\bold{b_1},A\bold{b_2},A\bold{b_3}]$
> Associative law is True $A(BC) = (AB)C$  
> Commutative law is false $AB \ne BA$
#### The Matrix $P_{ij}$ for a Row Exchange
>$P_{ij}$ is the identity matrix with rows $i$ and $j$ reversed. When this "permutation matrix" $P_{i,j}$ multiplies a matrix, it exchanges rows $i$ and $j$
#### The Augmented Matrix
Elimination does the same row operations to $A$ and to $\bold{b}$. We can include $\bold{b}$ as an extra column and follow it through elimination. The matrix $A$ is enlarged or "augmented" by the extra column $\bold{b}$
### 2.4 Rules for Matrix Operations
To multiply $AB$: If $A$ has $n$ columns, $B$ must have $n$ rows.   
Suppose $A$ is $m$ by $n$ and $B$ is $n$ by $p$. We can multiply. The product $AB$ is $m$ by $p$  
The entry in row $i$ and column $j$ of $AB$ is (row $i$ of $A$) · ( column $j$ of $B$)
#### The Second and Third Ways: Rows and Columns
Each column of $AB$ is a combination of the columns of $A$  
$A[\bold{b}_1 \dots \bold{b}_p] = [A\bold{b}_1 \dots A\bold{b}_p]$    
Every row of $AB$ is a combination of the rows of $B$   

$[$row $i$ of $A]$ $\begin{bmatrix}1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{bmatrix} = [$ row $i$ of $AB]$
#### The Fourth Way: Columns Multiply Rows
Multiply columns 1 to $n$ of $A$ times rows 1 to $n$ of $B$. Add those matrices.  
$\begin{bmatrix} col 1 & col2 & col3 \\ \vdots & \vdots & \vdots  \end{bmatrix}\begin{bmatrix}row 1 & \cdots \\ row 2 &\cdots \\ row 3 & \cdots \end{bmatrix} = (col 1)(row 1) + (col 2)(row 2) + (col 3)(row 3)$
#### The Laws for Matrix Operations
$A + B = B + A$  (commutative law)  
$c(A + B) = cA + cB$  (distributive law)  
$A + (B + C) = (A + B) + C$  ( associative law)  
$A(B + C) = AB + AC$   
$A(BC) = (AB)C$  
$AB \ne BA$  
$A^p = AAA\cdots A$  
$A^pA^q = A^{p+q}$  
$(A^p)^q = A^{pq}$  
#### Block Matrices and Block Multiplication
If blocks of $A$ can multiply blocks of $B$, then block multiplication of $AB$ is allowed. Cuts between columns of $A$ match cuts between rows of $B$.  
$\begin{bmatrix}A_{11} & A_{12} \\ A_{21} & A_{22}\end{bmatrix}\begin{bmatrix}B_{11}  \\B_{21} \end{bmatrix} = \begin{bmatrix}A_{11}B_{11}+A_{12}B_{11} \\ A_{21}B_{21}+A_{22}B_{21} \end{bmatrix}$   
Block Elimination: $\begin{bmatrix}I & 0 \\ -CA^{-1} & I\end{bmatrix}\begin{bmatrix}A & B \\C & D \end{bmatrix} = \begin{bmatrix} A & B\\ 0 & D-BCA^{-1} \end{bmatrix}$   
Schur complement: $D-BCA^{-1}$
### 2.5 Inverse Matrices
The matrix $A$ is invertible if there exists a matrix A^{-1}$ that "inverts" $A$ 
$$AA^{-1}=I$$ 
The inverse exists if and only if elimination produces $n$ pivot   
The matrix $A$ cannot have two different inverses.   
If $BA = I, AC = I$, then $B=C$  
If $A$ is invertible, the one and only solution to $A\bold{x} = \bold{b}$ is $x = A^{-1} b$   
Suppose there is a nonzero vector $x$ such that $A\bold{x} = \bold{0}$. Then $A$ cannot have an inverse  
A 2 by 2 matrix is invertible if and only if $ad - bc$ is not zero  
$\begin{bmatrix}a & b  \\ c & d \end{bmatrix}^{-1} = \dfrac{1}{ad-bc}\begin{bmatrix}d & -b  \\ -c & a \end{bmatrix}$  
A diagonal matrix has an inverse provided no diagonal entries are zero   
If $A = \begin{bmatrix}d_1 &  &  \\  & \ddots &  \\  &  & d_n \end{bmatrix}$, then $A^{-1} = \begin{bmatrix}\frac{1}{d_1} &  &  \\  & \ddots &  \\  &  & \frac{1}{d_n} \end{bmatrix}$
#### The Inverse of a Product $AB$  
If $A$ and $B$ are invertible then so is $AB$. The inverse of a product $AB$ is  
$(AB)^{-1} = B^{-1}A^{-1}$  
$AB(B^{-1}A^{-1}) = AIA^{-1} = I$
#### Calculating $A^{-1}$ by Gauss-Jordan Elimination  
Multiply $[A\quad I]$ by $A^{-1}$ to get $[I\quad A^{-1}]$  
#### Singular versus Invertible 
#### Recognizing an Invertible Matrix 
Diagonally dominant matrices are invertible $|a_{ii}| > \sum\limits_{i\ne j}|a_{ij}|$
### 2.6 Elimination = Factorization: $A = LU$
#### Explanation and Examples
$(E_{32}E_{31}E_{21})U = A, A = (E^{-1}_{32}E^{-1}_{31}E^{-1}_{21})U= LU$   
This is elimination without row exchanges. The upper triangular $U$ has the pivots on its diagonal. The lower triangular $L$ has all $l$'s on its diagonal. The multipliers $l_{ij}$ are below the diagonal of $L$.
#### One Square System = Two Triangular Systems
#### The Cost of Elimination 
### 2.7 Transposes and Permutations
$A^T_{ij} = A_{ji}$  
$(A + B)^T = A^T + B^T$    
$(AB)^T = B^TA^T$  
$(A^{-1})^T = (A^T)^{-1}$
#### The Meaning of Inner Products
The dot product or inner product is $\bold{x}^T\bold{y}$  
The rank one product or outer product is $\bold{xy}^T$  
$(A\bold{x})^T\bold{y} = \bold{x}^T(A^T\bold{y})$  
#### Symmetric Matrices
A symmetric matrix has $S^T = S$ . This means that $S_{ji} = S_{ij}$  
#### Symmetric Products $A^TA$ and $AA^T$ and $LDL^T$  
If $S = S^T$ is factored into $LDU$ with no row exchanges, then $U$ is exactly $L^T$.  
$S = LDL^T$
#### Permutation Matrices 
A permutation matrix $P$ has the rows of the identity $I$ in any order.  
$P^{-1} = P^T,PP^T = I$  
#### The $PA = LU$ Factorization with Row Exchanges