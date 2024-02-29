# Introduction to Linear Algebra
## Chapter 7 Singular Value Decomposition
### 7.1 Image Processing by Linear Algebra
#### Low Rank Images (Examples)
$$
AA^T\bold{u}_i= \sigma_i^2\bold{u}_i\\
A^TA\bold{v}_i= \sigma_i^2\bold{v}_i\\
A\bold{v}_i = \sigma_i\bold{v}
_i$$
$A = \begin{bmatrix} &\\\bold{u}_1&\bold{u}_2 \\ &\end{bmatrix}\begin{bmatrix} \sigma_1&\\& \\ &\sigma_2\end{bmatrix}\begin{bmatrix} \bold{v}_1^T\\\\ \bold{v}_2^T\end{bmatrix}$  
or 
$A\begin{bmatrix} &\\\bold{v}_1&\bold{v}_2 \\ &\end{bmatrix} = \begin{bmatrix} &\\\sigma_1\bold{u}_1&\sigma_2\bold{u}_2 \\ &\end{bmatrix}$
### 7.2 Bases and Matrices in the SVD 
$\bold{u}_1,\bold{u}_2, \dots,\bold{u}_r$ is an orthonormal basis for the column space  
$\bold{u}_{r+1},\bold{u}_2, \dots,\bold{u}_m$ is an orthonormal basis for the left nullspace $N (A^T)$   
$\bold{v}_1,\bold{v}_2, \dots,\bold{v}_r$ is an orthonormal basis for the row space  
$\bold{v}_{r+1},\bold{v}_2, \dots,\bold{v}_n$ is an orthonormal basis for the nullspace $N(A)$.   
To diagonalize $A: A\bold{v}_1=\sigma_1\bold{u}_1,\dots,A\bold{v}_r=\sigma_1\bold{u}_r$  
Those singular values $\sigma_1$ to $\sigma_r$ will be positive numbers: $\sigma_i$ is the length of $A\bold{v}_i$. They go into a diagonal matrix that is otherwise zero, $\Sigma$  
$AV_r = U_r\Sigma_r$  
By including the $\bold{u}$s and $\bold{v}$s from the null space and left null space,   
$AV = U\Sigma$   
**Singular Value Decomposition**  
$$
A = U\Sigma V^T=\bold{u}_1\sigma_1\bold{v}_1^T + \cdots + \bold{u}_r\sigma_r\bold{v}_r^T
$$
Each $\sigma_i^2$ is an eigenvalue of $A^TA$ and also $AA^T$. When we put the singular values in descending order, $\sigma_1 \ge \sigma_2 \ge \sigma_r \ge 0$, the splitting gives the $r$ rank-one pieces of $A$ in order of importance
#### Proof of the SVD
The $\bold{v}$'s will be orthonormal eigenvectors of $A^T A$.  
$A^T A = (U\Sigma V^T)^T(U\Sigma V^T)= V\Sigma^TU^TU\Sigma V^T =V\Sigma^T\Sigma V^T$  
$\bold{u}_i^T\bold{u}_j = (\frac{A\bold{v}_i}{\sigma_1})^T(\frac{A\bold{v}_j}{\sigma_j}) = \dfrac{\bold{v}_i^TA^TA\bold{v}_j}{\sigma_i\sigma_j} = \dfrac{\sigma_j^2}{\sigma_i\sigma_j}\bold{v}_i^T\bold{v}_j = 0$, For $i\ne j$   
The $\bold{v}$'s are eigenvectors of $A^T A$ (symmetric). They are orthogonal and now the $\bold{u}$'s are also orthogonal. Actually those $\bold{u}$'s will be eigenvectors of $AA^T$ .
#### An Example of the SVD
#### An Extreme Matrix 
#### Singular Value Stability versus Eigenvalue Instability
#### Singular Vectors of $A$ and Eigenvectors of $S = A^T A$
Start with the largest eigenvalue $\lambda_1$ of $S$. It solves this problem:   
$\lambda_1 = \max \dfrac{\bold{x}^TS\bold{x}}{\bold{x}^T\bold{x}}, \bold{x} = \bold{q}_1,S\bold{q}_1=\lambda_1\bold{q}_1$   
$\lambda_2 = \max \dfrac{\bold{x}^TS\bold{x}}{\bold{x}^T\bold{x}}, \bold{q}_1^T\bold{x} = 0, \bold{x} = \bold{q}_2$  
the largest singular value $\sigma_1$ of A solves this problem:  
$\sigma_1 = \max\dfrac{||A\bold{x}||}{||\bold{x}||}, \bold{x} = \bold{v_1},A\bold{v}_1=\sigma_1\bold{v}_1$  
$\sigma_2 = \max\dfrac{||A\bold{x}||}{||\bold{x}||},  \bold{v}_1^T\bold{x} = 0,\bold{x} = \bold{v}_2$  
When $S = A^T A$ we find $\lambda_1 = \sigma_1^2$ and $\lambda_2 = \sigma_2^2$  
Let $r(x) = \dfrac{\bold{x}^TS\bold{x}}{\bold{x}^T\bold{x}}, \dfrac{\partial r}{\partial \bold{x}_i} = 0$ when $S\bold{x} = r(\bold{x})\bold{x}$  
When $S = A^T A$, $(\dfrac{||A\bold{x}||}{||\bold{x}||})^2 = \dfrac{\bold{x}^TA^TA\bold{x}}{\bold{x}^T\bold{x}} = \dfrac{\bold{x}^TS\bold{x}}{\bold{x}^T\bold{x}}$
For $\bold{q}_2$, start with any orthogonal matrix $Q_1$. The other $n - l$ orthonormal columns just have to be orthogonal to $\bold{q}_1$. Then use $S\bold{q}_1=\lambda_1\bold{q}_1$  
$SQ_1 = S\begin{bmatrix}\bold{q}_1 & \bold{q}_2 & \dots & \bold{q}_n \end{bmatrix} = \begin{bmatrix}\bold{q}_1 & \bold{q}_2 & \dots & \bold{q}_n \end{bmatrix}\begin{bmatrix}\lambda_1 & \bold{w}^T  \\ \bold{0} & S_{n-1} \end{bmatrix} =Q_1\begin{bmatrix}\lambda_1 & \bold{w}^T  \\ \bold{0} & S_{n-1} \end{bmatrix}$  
Multiply by $Q_1^T, Q_1^TQ_1 = I, Q_1^TSQ_1$ is symmetric    
$Q_1^TSQ_1 = Q_1^TQ_1\begin{bmatrix}\lambda_1 & \bold{w}^T  \\ \bold{0} & S_{n-1} \end{bmatrix} = \begin{bmatrix}\lambda_1 & \bold{w}^T  \\ \bold{0} & S_{n-1} \end{bmatrix}$  
$\bold{w} = 0,S_{n-1}^T = S_{n-1}$
#### Computing the Eigenvalues of $S$ and Singular Values of $A$
### 7.3 Principal Component Analysis (PCA by the SVD)
#### The Essentials of Principal Component Analysis (PCA) 
$S = \dfrac{AA^T}{n-1}$  
The total variance in the data is the sum of all eigenvalues and of sample variances $s^2$: Total variance $T = \sigma_1^2 + \cdots + \sigma_m^2 = s_1^2 + \cdots + s_m^2 =$ trace (diagonal sum).   
The first eigenvector $\bold{u}_1$ of $S$ points in the most significant direction of the data. That direction accounts for (or explains) a fraction $\frac{\sigma_1^2}{T}$ of the total variance. 
The next eigenvector $\bold{u}_2$ (orthogonal to $\bold{u}_1$) accounts for a smaller fraction $\frac{\sigma_2^2}{T}$.
Stop when those fractions are small. You have the $R$ directions that explain most ofthe data. The $n$ data points are very near an $R$-dimensional subspace with basis $\bold{u}_1$ to $\bold{u}_R$ These $\bold{u}$'s are the principal components in $m$-dimensional space.   
$R$ is the "effective rank" of $A$. The true rank $r$ is probably $m$ or $n$ : full rank matrix.
#### Perpendicular Least Squares
![](/images/linear%20algebra/7-1.png)  
The sum of squared distances from the points to the line is a minimum  
$$
\sum_{j=1}^n||a_j||^2 = \sum_{j=1}^n|a_j^T\bold{u}_1|^2 + \sum_{j=1}^n|a_j^T\bold{u}_2|^2
$$
$\sum\limits_{j=1}^n|a_j^T\bold{u}_1|^2 = \bold{u}_1^TAA^T\bold{u}_1$. When we maximize that sum in PCA by choosing the eigenvector $\bold{u}_1$, we minimize the second sum.
#### The Sample Correlation Matrix
#### Genetic Variation in Europe
#### Eigenfaces
#### Applications of Eigenfaces
#### Model Order Reduction
#### Searching the Web
#### PCA in Finance: The Dynamics of Interest Rates 
### 7.4 The Geometry of the SVD
![](/images/linear%20algebra/7-2.png)
#### The Norm of a Matrix 
The norm $||A||$ is the largest ratio $||A|| = \max\limits_{\bold{x}\ne 0}\dfrac{||A\bold{x}||}{||\bold{x}||} = \sigma_1$  
$||A+B||\le ||A|| + ||B||, ||AB|| \le ||A||||B||$
#### Polar Decomposition $A = Q S$
Every real square matrix can be factored into $A = Q S$, where $Q$ is orthogonal and $S$ is symmetric positive semidefinite. If $A$ is invertible, $S$ is positive definite  
$$A = U\Sigma V^T = (UV^T)(V\Sigma V^T) = QS$$
The nearest singular matrix $A_0$ to $A$ comes by changing the smallest $\sigma_{\min}$ to zero
#### The Pseudoinverse $A^+$
$$A^+= V\Sigma^+U^T \begin{bmatrix} && \\ \bold{v}_1 & \bold{v}_r & \bold{v}_n \\ && \end{bmatrix}\begin{bmatrix} \sigma_1^{-1} & & &\\ & \ddots && \\ & & \sigma_r^{-1} &\\ &&&\end{bmatrix} \begin{bmatrix} && \\ \bold{u}_1 & \bold{u}_r & \bold{u}_m \\ && \end{bmatrix}$$  
![](/images/linear%20algebra/7-3.png)
#### Least Squares with Dependent Columns 
$\bold{x}^+ = A^+\bold{b}=(1,1)$ is the shortest solution to $A^TA\hat{\bold{x}} = A^T\bold{b}$ and $A\hat{\bold{x}}=\bold{p}$