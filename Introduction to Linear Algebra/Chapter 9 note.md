# Introduction to Linear Algebra
## Chapter 9 Complex Vectors and Matrices
### 9.1 Complex Numbers 
A complex number is a real number plus an imaginary number. Addition keeps the real and imaginary parts separate. Multiplication uses $i^2 = -1$
#### The Complex Plane
$\bar{z_1}\bar{z_2} = \overline{z_1z_2}$  
$\bar{z_1}+\bar{z_2} = \overline{z_1+z_2}$  
If $A\bold{x} = \lambda \bold{x}$ and $A$ is real then $A\bar{\bold{x}} = \lambda \bar{\bold{x}}$
#### The Polar Form $re^{i\theta}$
$z = a+bi \lrArr z = r\cos \theta + r\sin \theta i$  
#### Powers and Products: Polar Form  
$z = r\cos \theta + r\sin \theta i, z^n = r^n(\cos n \theta + \sin n\theta i)$  
Euler's Formula $e^{i\theta} = \cos \theta + \sin \theta i, z = r\cos \theta + r\sin \theta i=re^{i\theta}$  
Set $w = e^{\frac{2\pi i}{n}}$. The $n$th powers of $1,w,\dots,w^{n-1}$ all equal 1.  
### 9.2 Hermitian and Unitary Matrices
When you transpose a complex vector $\bold{z}$ or matrix $A$, take the complex conjugate too: $\bold{z}^H = \bar{\bold{z}}^T$  
The length $||\bar{\bold{z}}||$ is the square root of $\bar{\bold{z}}^T\bold{z} = \bold{z}^H\bold{z} = |z_1|^2+\cdots + |z_n|^2$  
#### Complex Inner Products 
The inner product of real or complex vectors $\bold{u}$ and $\bold{v}$ is $\bold{u} ^H \bold{v} = \overline{u_1}v_1 + \cdots + \overline{u_n}v_n$    
With complex vectors, $\bold{u} ^H \bold{v}$ is different from $\bold{v} ^H \bold{u}$. In fact $\bold{v} ^H \bold{u} = \overline{v_1}u_1 + \cdots + \overline{v_n}u_n = (\bold{u} ^H \bold{v})^H$   
The inner product of $A\bold{u}$ with $\bold{v}$ equals the inner product of $\bold{u}$ with $A^H\bold{v}$: $(A\bold{u})^H\bold{v} = \bold{u}^H(A^H\bold{v})$   
$A^H$ is also called the "adjoint" of $A$   
The conjugate transpose of $AB$ is $(AB)^H = B^HA^H$
#### Hermitian Matrices $S = S^H$ 
Among complex matrices, the special class contains the Hermitian matrices: $S = S^H$. The condition on the entries is $S_{ij} = \overline{S_{ji}}$· In this case we say that "$S$ is Hermitian." Every real symmetric matrix is Hermitian.  

If $S = S^H$ and $\bold{z}$ is any real or complex column vector, the number $\bold{z}^HS\bold{z}$ is real.  
Proof: $\bold{z}^HS\bold{z}$ is 1 by 1. Take its conjugate transpose: $(\bold{z}^HS\bold{z})^H = \bold{z}^HS\bold{z}$, must be real  

Every eigenvalue of a Hermitian matrix is real.  
Proof: Suppose $S\bold{z} = \lambda \bold{z}$. Multiply both sides by $\bold{z}^H$ to get $\bold{z}^HS\bold{z} = \bold{z}^H\lambda\bold{z}$. On the left side, $\bold{z}^HS\bold{z}$ is real. On the right side, $\bold{z}^H\bold{z}$ is the length squared, real and positive. So the ratio $\lambda = \dfrac{\bold{z}^HS\bold{z}}{\bold{z}^H\bold{z}}$ is a real number.

The eigenvectors of a Hermitian matrix are orthogonal (when they correspond to different eigenvalues). If $S\bold{z} = \lambda \bold{z}$ and $S\bold{y} = \beta \bold{y}$ then $\bold{y}^H\bold{z} = 0$  
Proof: Multiply $S\bold{z} = \lambda \bold{z}$ on the left by $\bold{y}^H$. Multiply $\bold{y}^HS^H = \beta \bold{y}^H$ on the right by $\bold{z}$:   
$\bold{y}^HS\bold{z} = \bold{y}^H\lambda \bold{z}$ and $\bold{y}^HS^H\bold{z} = \beta \bold{y}^H\bold{z}$    
$S=S^H,\lambda \ne \beta$ Then $\bold{y}^H\bold{z} = 0$   
#### Unitary Matrices 
A unitary matrix $Q$ is a (complex) square matrix that has orthonormal columns.  
Every matrix $Q$ with orthonormal columns has $Q^HQ = I$.  
If $Q$ is square, it is a unitary matrix. Then $Q^H=Q^{-1}$  
If $Q$ is unitary then $||Q\bold{z}|| = ||\bold{z}||$ Therefore $Q\bold{z} = \lambda\bold{z}$ leads to $|\lambda| = 1$.
### 9.3 The Fast Fourier Transform
#### Roots of Unity and the Fourier Matrix
The $n$ by $n$ Fourier matrix contains powers of $w = e^{\frac{2\pi i}{n}}$  
$F_n\bold{c} = \begin{bmatrix}1 & 1 & 1 &\cdot &1 \\ 1 &w & w^2 &\cdot &w^{n-1}\\ 1 &w^2 & w^4 &\cdot &w^{2(n-1)} \\ \cdot & \cdot & \cdot & \cdot & \cdot \\ 1 & w^{n-1} & w^{2(n-1)}&\cdot &w^{(n-1)^2} \end{bmatrix}\begin{bmatrix}c_0\\ c_1\\ c_2\\ \cdot\\ c_{n-1} \end{bmatrix} = \begin{bmatrix}y_0\\ y_1\\ y_2\\ \cdot\\ y_{n-1} \end{bmatrix} = y$  
$F_n$ is symmetric but not Hermitian. Its columns are orthogonal, and $F_n\overline{F_n} = nI$. Then $F_n^{-1}$ is $\frac{\overline{F_n}}{n}$.  
The entry in row $j$, column $k$ is $w^{jk}$ Row zero and column zero contain $w^0=1$. 
#### One Step of the Fast Fourier Transform
separating $c_0,\cdots, c_{n-1}$ into even $c_{2k}$ and odd $c_{2k+1}$:  
$y = F\bold{c},y_j = \sum\limits_0^{n-1}w^{jk}c_k$  
$=\sum\limits_0^{m-1}w^{2jk}c_2k+ \sum\limits_0^{m-1}w^{j(2k+1)}c_{2k+1},m=\dfrac{1}{2}n$  
#### The Full FFT by Recursion