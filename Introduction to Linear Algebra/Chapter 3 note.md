# Introduction to Linear Algebra
## Chapter 3 Vector Spaces and Subspaces
### 3.1 Spaces of Vectors
The space $\bold{R}^n$ consists of all column vectors $\bold{v}$ with $n$ components.  
We can add any vectors in $\bold{R}^n$, and we can multiply any vector $\bold{v}$ by any scalar $c$
#### Subspaces
A subspace of a vector space is a set of vectors (including 0) that satisfies two requirements: If $\bold{v}$ and $\bold{w}$ are vectors in the subspace and $c$ is any scalar, then   
(i) $\bold{v} + \bold{w}$ is in the subspace  
(ii) $c\bold{v}$ is in the subspace  
or: A subspace containing $\bold{v}$ and $\bold{w}$ must contain all linear combinations $c\bold{v} + d\bold{w}$.   
**Every subspace contains the zero vector.**  
#### The Column Space of $A$
The column space consists of all linear combinations of the columns. The combinations are all possible vectors $A\bold{x}$. They fill the column space $C(A)$.    
The system $A\bold{x} = \bold{b}$ is solvable if and only if $\bold{b}$ is in the column space of $A$.    
Instead of columns in $\bold{R}^m$, we could start with any set $S$ of vectors in a vector space $V$. To get a subspace $SS$ of $V$, we take all combinations of the vectors in that set, $SS$ is the subspace of $V$ "spanned" by $S$
### 3.2 The Nullspace of $A$: Solving $A\bold{x} = \bold{0}$ and $R\bold{x} = \bold{0}$
The nullspace $N(A)$ consists of all solutions to $A\bold{x} = \bold{0}$. These vectors $\bold{x}$ are in $\bold{R}^n$. The nullspace of $A$ consists of all combinations of the special solutions to $A\bold{x} = \bold{0}$. 
#### Pivot Columns and Free Columns
#### The Reduced Row Echelon Form $R$
Suppose $A\bold{x} = \bold{0}$ has more unknowns than equations ($n > m$, more columns than rows). 
There must be at least one free column. Then $A\bold{x} = \bold{0}$ has nonzero solutions.   
#### The Rank of a Matrix
The rank of $A$ is the number of pivots. This number is $r$. 
#### Rank One
$A$ and $U$ and $R$ have $r$ independent rows and columns. The rank $r$ is the "dimension" of the column space. It is also the dimension of the row space. The great thing is that $n - r$ is the dimension of the nullspace.
### 3.3 The Complete Solution to $A\bold{x} = \bold{b}$
#### One Particular Solution $A\bold{x}_p = \bold{b}$
For a solution to exist, zero rows in $R$ must also be zero in $d$. Since $I$ is in the pivot rows and pivot columns of $R$, the pivot variables in $x_p$  come from $d$  
Complete solution: $\bold{x} = \bold{x}_p + \bold{x}_n$  
#### The Complete Solution
$r=m$ and $r=n$  has 1 solution   
$r=m$ and $r<n$ $\infty$ solutions   
$r <m$ and $r=n$ 0 or 1 solution   
$r <m$ and $r<n$ 0 or $\infty$ solutions 
### 3.4 Independence, Basis and Dimension 
Every vector in the space is a unique combination of the basis vectors
#### Linear Independence  
The columns of $A$ are linearly independent when the only solution to $A\bold{x} = \bold{0}$ is $\bold{x} = \bold{0}$. No other combination $A\bold{x}$ of the columns gives the zero vector.  
The sequence of vectors $\bold{v}_1+ \bold{v}_2, \dots, \bold{v}_n$ is linearly independent if the only
combination that gives the zero vector is $0\bold{v}_1+0\bold{v}_2+ \dots + 0\bold{v}_n$   
The columns of $A$ are independent exactly when the rank is $r = n$.There are $n$ pivots and no free variables. Only $\bold{x} = \bold{0}$ is in the nullspace. Any set of $n$ vectors in $\bold{R}^m$ must be linearly dependent if $n > m$. 
#### Vectors that Span a Subspace
A set of vectors spans a space if their linear combinations fill the space.  
The row space of a matrix is the subspace of $\bold{R}^n$ spanned by the rows. The row space of $A$ is $C(A^T)$. It is the column space of $A^T$
#### A Basis for a Vector Space
A basis for a vector space is a sequence of vectors with two properties: The basis vectors are linearly independent and they span the space. There is one and only one way to write $\bold{v}$ as a combination of the basis vectors.  
The vectors $\bold{v}_1, \bold{v}_2, \dots, \bold{v}_n$ are a basis for $\bold{R}^n$ exactly when they are the columns of an $n$ by $n$ invertible matrix. Thus $\bold{R}^n$ has infinitely many different bases. The pivot columns of $A$ are a basis for its column space. The pivot rows of $A$ are a basis for its row space. So are the pivot rows of its echelon form $R$.  
#### Dimension of a Vector Space
If $\bold{v}_1,\bold{v}_2, \dots, \bold{v}_m$ and $\bold{w}_1,\bold{w}_2, \dots, \bold{w}_n$ are both bases for the same vector space, then $m = n$.  
Proof: Suppose $n > m$, then $\bold{w}_n$ is a combination of the $\bold{v}$s.   
$W = \begin{bmatrix}\bold{v}_1 \dots \bold{v}_m \end{bmatrix}\begin{bmatrix}a_{11} & \dots & a_{1n} \\ \vdots & \ddots & \vdots \\ a_{m1} & \dots & a_{mn} \end{bmatrix} = VA$  
$A$ has $n>m,A\bold{x} = \bold{0}$ has a nonzero solution.  
Then $VA\bold{x} = 0, W\bold{x} = 0$ for nonzero $\bold{x}$ then $\bold{w}$s can not be bases.  
The dimension of a space is the number of vectors in every basis. 
#### Bases for Matrix Spaces and Function Spaces 
The dimension of the whole $n$ by $n$ matrix space is $n^2$.
### 3.5 Dimensions of the Four Subspaces
#### The Four Subspaces for $R$
The dimension of the row space is the rank $r$. The nonzero rows of $R$ form a basis.  
The dimension of the column space is the rank $r$. The pivot columns form a basis.  
The nullspace has dimension $n - r$. The special solutions form a basis.   
If $A$ is $m$ by $n$ of rank $r$, its left nullspace has dimension $m - r$.   
In $\bold{R}^n$ the row space and nullspace have dimensions $r$ and $n - r$ (adding to $n$).   
In $\bold{R}^m$ the column space and left nullspace have dimensions $r$ and $m - r$ ( total $m$).  
#### The Four Subspaces for A
The subspace dimensions for $A$ are the same as for $R$.  
Rank Theorem: The number of independent columns = the number of independent rows.   
(dimension of column space) + ( dimension of nullspace) = dimension of $\bold{R}^n$.  
> Fundamental Theorem of Linear Algebra, Part 1   
The column space and row space both have dimension $r$.    
The nullspaces have dimensions $n - r$ and $m - r$.  
#### Rank One Matrices (Review)
Every rank one matrix is one column times one row $A =\bold{u} \bold{v}^T$
#### Rank Two Matrices = Rank One plus Rank One 

