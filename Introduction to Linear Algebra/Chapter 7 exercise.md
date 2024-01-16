# Introduction to Linear Algebra
## Chapter 7 Singular Value Decomposition
### 7.1 Image Processing by Linear Algebra
1. What are the ranks $r$ for these matrices with entries $i$ times $j$ and $i$ plus $j$ ? Write $A$ and $B$ as the sum of $r$ pieces $\bold{u}\bold{v}^T$ of rank one. Not requiring $\bold{u}_1^T\bold{u}_2 = \bold{v}_1^T\bold{v}_2 = 0.$  
   $A = \begin{bmatrix}1 &2  & 3 &4 \\ 2 & 4 & 6 &8 \\ 3 & 6 & 9 &12    \\ 4 & 8 & 12 &16 \end{bmatrix}, B = \begin{bmatrix}2 &3 & 4&5 \\ 3 & 4 & 5 &6 \\ 4 & 5 & 6 &7    \\ 5& 6 & 7 &8 \end{bmatrix}$  
   $A: r=1, A = \begin{bmatrix}1  \\ 2  \\ 3  \\ 4 \end{bmatrix}\begin{bmatrix}1  & 2 & 3 & 4 \end{bmatrix}$  
   $B: r=4,B=\begin{bmatrix}2 \\3 \\ 4 \\ 5 \end{bmatrix}\begin{bmatrix}1  & 0 & 0 & 0 \end{bmatrix} + \begin{bmatrix}3\\4 \\ 5\\ 6 \end{bmatrix}\begin{bmatrix}0 & 1 & 0 & 0 \end{bmatrix}+\begin{bmatrix}4\\5 \\6\\ 7 \end{bmatrix}\begin{bmatrix}0 & 0 & 1 & 0 \end{bmatrix}+\begin{bmatrix}5\\6 \\ 7\\ 8 \end{bmatrix}\begin{bmatrix}0 & 0 & 0 & 1\end{bmatrix}$
### 7.2 Bases and Matrices in the SVD
1. Find the eigenvalues of these matrices. Then find singular values from $A^TA$:  
   $$A = \begin{bmatrix}0 & 4  \\ 0 & 0 \end{bmatrix}, A = \begin{bmatrix}0 & 4  \\ 1 & 0 \end{bmatrix}$$  
   For each $A$, construct $V$ from the eigenvectors of $A^T A$ and $U$ from the eigenvectors of $AA^T$ . Check that $A = U\Sigma V^T$.   
   $|\det A-\lambda I| = \lambda^2=0,\lambda = 0$  
   $A^TA = \begin{bmatrix}0 & 0  \\ 4 & 0 \end{bmatrix}\begin{bmatrix}0 & 4  \\ 0 & 0 \end{bmatrix}  =\begin{bmatrix}0 & 0 \\ 0 & 16 \end{bmatrix}, \lambda^2 - 16\lambda = 0, \lambda_1=16,\lambda_2=0, \sigma_1=4,\sigma_2 =0$  
   $\bold{v}_1 =\begin{bmatrix}0 \\ 1 \end{bmatrix}  ,\bold{v_2}= \begin{bmatrix}1 \\ 0 \end{bmatrix}$  
   $AA^T = \begin{bmatrix}0 & 4  \\ 0 & 0 \end{bmatrix}\begin{bmatrix}0 & 0  \\ 4 & 0 \end{bmatrix}  =\begin{bmatrix}16 & 0 \\ 0 & 0 \end{bmatrix}, \lambda^2 - 16\lambda = 0, \lambda_1=16,\lambda_2=0, \sigma_1=4,\sigma_2 =0$  
   $\bold{u}_1 = \begin{bmatrix}1 \\ 0 \end{bmatrix},\bold{u_2} = \begin{bmatrix}0 \\ 1 \end{bmatrix}$  
   $A = \begin{bmatrix}1&0 \\ 0&1 \end{bmatrix}\begin{bmatrix}4&0 \\ 0&0\end{bmatrix}\begin{bmatrix}0&1 \\ 1&0 \end{bmatrix}$  
   
   $|\det A-\lambda I| = \lambda^2-4=0,\lambda = 2$  
   $A^TA = \begin{bmatrix}0 & 1  \\ 4 & 0 \end{bmatrix}\begin{bmatrix}0 & 4  \\ 1 & 0 \end{bmatrix}  =\begin{bmatrix}1 & 0 \\ 0 & 16 \end{bmatrix}, \lambda^2 - 17\lambda +16= 0, \lambda_1=16,\lambda_2=1, \sigma_1=4,\sigma_2 =1$  
   $\bold{v}_1 =\begin{bmatrix}0 \\ 1 \end{bmatrix}  ,\bold{v_2}= \begin{bmatrix}1 \\ 0 \end{bmatrix}$  
   $AA^T = \begin{bmatrix}0 & 4  \\ 1 & 0 \end{bmatrix}\begin{bmatrix}0 & 1  \\ 4 & 0 \end{bmatrix}  =\begin{bmatrix}16 & 0 \\ 0 & 1 \end{bmatrix}, \lambda^2 - 17\lambda +16= 0, \lambda_1=16,\lambda_2=0, \sigma_1=4,\sigma_2 =0$  
   $\bold{u}_1 = \begin{bmatrix}1 \\ 0 \end{bmatrix},\bold{u_2} = \begin{bmatrix}0 \\ 1 \end{bmatrix}$  
   $A = \begin{bmatrix}1&0 \\ 0&1 \end{bmatrix}\begin{bmatrix}4&0 \\ 0&1\end{bmatrix}\begin{bmatrix}0&1 \\ 1&0 \end{bmatrix}$
### 7.3 Principal Component Analysis (PCA by the SYD) 
1. Suppose $A_0$ holds these 2 measurements of 5 samples:
   $$A_0 = \begin{bmatrix}5 & 4 & 3 & 2 & 1  \\ -1 & 1 & 0 & 1 & -1\end{bmatrix}$$  
   Find the average of each row and subtract it to produce the centered matrix $A$. Compute the sample covariance matrix $S = \dfrac{AA^T}{n-1}$ and find its eigenvalues $\lambda_1$ and $\lambda_2$ . What line through the origin is closest to the 5 samples in columns of $A$?   
   $A = \begin{bmatrix}2 & 1 & 0 & -1 & -2  \\ -1 & 1 & 0 & 1 & -1\end{bmatrix}, A^T = \begin{bmatrix}2 & -1 \\1&1 \\0 &  0 \\ -1& 1\\  -2  & -1 \end{bmatrix}$  
   $S = \dfrac{1}{4}\begin{bmatrix}10 & 0 \\ 0 & 4\end{bmatrix}$  
   $det(S-\lambda I) = (\dfrac{5}{2}-\lambda)(1-\lambda) =\lambda^2-\dfrac{7}{2}\lambda+\dfrac{5}{2}=0$  
   $(\lambda-1)(2\lambda-5)=0, \lambda_1=\dfrac{5}{2},\lambda_2=1$  
   $\bold{u}_1=\begin{bmatrix}1  \\ 1\end{bmatrix}$
### 7.4 The Geometry of the SVD
Problems 1-4 compute and use the SVD of a particular matrix (not invertible).
1. (a) Compute $A^T A$ and its eigenvalues and unit eigenvectors $\bold{v}_1$ and $\bold{v}_2$. Find $\sigma_1$.   
Rank one matrix $A = \begin{bmatrix}1& 2 \\ 3 & 6 \end{bmatrix}$   
(b) Compute $AA^T$ and its eigenvalues and unit eigenvectors $\bold{u}_1$ and $\bold{u}_2$.   
(c) Verify that $A\bold{v}_1 = \sigma_1\bold{u}_1$. Put numbers into $A= U\Sigma V^T$ (this is the SYD).  
   (a) $A^T = \begin{bmatrix}1& 3 \\ 2 & 6 \end{bmatrix}, A^TA = \begin{bmatrix}10& 20 \\ 20 & 40 \end{bmatrix}$  
   $(10-\lambda)(40-\lambda) -400= \lambda^2-50\lambda = 0, \lambda_1 = 50, \lambda_2 = 0$  
   $\bold{v}_1=\dfrac{1}{\sqrt{5}}\begin{bmatrix}1\\ 2 \end{bmatrix},\bold{v}_2 = \dfrac{1}{\sqrt{5}}\begin{bmatrix}-2\\ 1 \end{bmatrix},\sigma_1 = 5\sqrt{2}$  
   (b) $AA^T =\begin{bmatrix}5& 15 \\ 15 & 45 \end{bmatrix}$  
   $(5-\lambda)(45-\lambda)-225=0,\lambda^2-50\lambda=0,\lambda_1=50,\lambda_2=0$  
   $\bold{u}_1=\dfrac{1}{\sqrt{10}}\begin{bmatrix}1\\ 3 \end{bmatrix},\bold{u}_2 = \dfrac{1}{\sqrt{10}}\begin{bmatrix}-3\\ 1 \end{bmatrix}$  
   (c) $A\bold{v}_1 = \dfrac{1}{\sqrt{5}}\begin{bmatrix}5 \\ 15 \end{bmatrix},\sigma_1\bold{u}_1=\dfrac{5}{\sqrt{5}}\begin{bmatrix}1 \\ 3 \end{bmatrix}$   
   $A = \dfrac{1}{5\sqrt{2}}\begin{bmatrix}1& 3 \\ -3 & 1 \end{bmatrix}\begin{bmatrix}5\sqrt{2}& 0 \\ 0 & 0 \end{bmatrix}\begin{bmatrix}1& 2 \\ -2 & 1 \end{bmatrix}$

Problems 5-9 are about the SVD of an invertible matrix. 

5. Compute $A^T A$ and its eigenvalues and unit eigenvectors $\bold{v}_1$ and $\bold{v}_2$. What are the singular values $\sigma_1$ and $\sigma_2$ for this matrix $A$?  
   $A = \begin{bmatrix}3& 3 \\ -1 & 1 \end{bmatrix}$  
   $A^T = \begin{bmatrix}3& -1 \\ 3 & 1 \end{bmatrix},A^TA = \begin{bmatrix}10& 8 \\ 8 & 10\end{bmatrix}$  
   $(10-\lambda)^2-64=\lambda^2-20\lambda+36 = 0,\lambda_1=18,\lambda_2=2,\sigma_1=3\sqrt{2},\lambda_2=\sqrt{2}$  
   $\bold{v}_1 = \dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\  1 \end{bmatrix},\bold{v}_2 = \dfrac{1}{\sqrt{2}}\begin{bmatrix}1 \\ -1 \end{bmatrix}$  

Problems 10-11 compute and use the SVD of a 1 by 3 rectangular matrix

10. Compute $A^T A$ and $AA^T$ and their eigenvalues and unit eigenvectors when the matrix is $A = \begin{bmatrix}3&4&  0 \end{bmatrix}$ . What are the singular values of $A$?   
    $A^T =  \begin{bmatrix}3\\4\\  0 \end{bmatrix}, A^TA = \begin{bmatrix}9&12&  0\\12 & 16 &0 \\0 & 0 &0 \end{bmatrix}$  
    $(0-\lambda)[(9-\lambda)(16-\lambda)-144] = (-\lambda)(\lambda^2-25\lambda)=0,\lambda_1=25,\lambda_2=0,\lambda_3=0\sigma_1=5,\sigma_2=0,\sigma_3=0$  
    $\bold{v}_1 = \dfrac{1}{5}\begin{bmatrix}3\\  4 \\0\end{bmatrix},\bold{v}_2 = \dfrac{1}{5}\begin{bmatrix}-4 \\ 3 \\ 0 \end{bmatrix},\bold{v}_3 = \begin{bmatrix}0 \\ 0\\ 1 \end{bmatrix}$   
    $AA^T = \begin{bmatrix}25\end{bmatrix}$  

Problems 15-18 bring out the main properties of $A^+$ and $x^+ = A^+\bold{b}$.  

15. All matrices in this problem have rank one. The vector $\bold{b}$ is $(b_1, b_2)$  
    $$A = \begin{bmatrix}2&2\\1&1\end{bmatrix},AA^T = \begin{bmatrix}8&4\\4&2\end{bmatrix},A^TA = \begin{bmatrix}5 & 5 \\5&5\end{bmatrix},A^+ = \begin{bmatrix}.2 & .1 \\.2&.1\end{bmatrix}$$  
    (a) The equation $A^TA\hat{\bold{x}} = A^T\bold{b}$ has many solutions because $A^T A$ is *singular* ,  
    (b) Verify that $\bold{x}^+ = A^+ \bold{b} = (.2b_1 + .1b_2, .2b_1 + .1b_2)$ solves $A^TA\bold{x}^+ = A^T\bold{b}$,  
    (c) Add $(1, -1)$ to that $\bold{x}^+$ to get another solution to $A^TA\hat{\bold{x}} = A^T\bold{b}$, Show that $||\hat{\bold{x}}||^2 = ||\bold{x}^+||^2 + 2$, and $\bold{x}^+$ is shorter  
    (b)  $A^TA\bold{x}^+ = \begin{bmatrix}2b_1+1b_2\\2b1+1b_2\end{bmatrix},A^T=\begin{bmatrix}2&1\\2&1\end{bmatrix},A^T\bold{b} = \begin{bmatrix}2b_1+b_2\\2b_1+b_2\end{bmatrix}$  
    (c) $||\hat{\bold{x}}||^2=(.2b_1 + .1b_2+1)^2+(.2b_1 + .1b_2-1)^2=2(.2b_1 + .1b_2)^2+2=||\bold{x}^+||^2 + 2$
 