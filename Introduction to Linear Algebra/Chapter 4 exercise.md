# Introduction to Linear Algebra
## Chapter 4 Orthogonality
### 4.1 Orthogonality of the Four Subspaces 
Questions 1-12 grow out of Figures 4.2 and 4.3 with four subspaces.
1. Construct any 2 by 3 matrix of rank one. Copy Figure 4.2 and put one vector in each subspace (and put two in the nullspace). Which vectors are orthogonal?  
   $\begin{bmatrix}1 & 2 &6 \\ 2 & 4 &12 \end{bmatrix}$    
   column space: $\begin{bmatrix}1  \\ 2 \end{bmatrix}$  
   row space: $\begin{bmatrix}1 \\ 2 \\ 6 \end{bmatrix}$  
   null space: $\begin{bmatrix}-6 \\0 \\1 \end{bmatrix},\begin{bmatrix}-2 \\1\\0 \end{bmatrix}$  
   left null space: $\begin{bmatrix}-2 \\1 \end{bmatrix}$   

Questions 13-23 are about orthogonal subspaces. 

13. Put bases for the subspaces $V$ and $W$ into the columns of matrices $V$ and $W$. Explain why the test for orthogonal subspaces can be written $V^TW =$ zero matrix. This matches $\bold{v}^T \cdot \bold{w}=0$ for orthogonal vectors.   
    $(a_1V_1+ a_2V_2)(b_1W_1+b_2W_2)$  
    $= a_1b_1V_1W_1+a_2b_2V_2W_2 + a_1b_2V_1W_2 + a_2b_1V_2W_1=0$

Questions 24-30 are about perpendicular columns and rows. 

24. Suppose an $n$ by $n$ matrix is invertible: $AA^{-1} = I.$ Then the first column of $A^{-1}$ is orthogonal to the space spanned by which rows of $A$?   
    any combinations of the rest rows + none * first row 
####  Challenge Problems
30. Suppose $A$ is 3 by 4 and $B$ is 4 by 5 and $AB = 0$. So $N(A)$ contains $C(B)$. Prove from the dimensions of $N(A)$ and $C(B)$ that $rank(A) + rank(B) \le 4$.  
    $rank(A) + rank(B)$  
    $=4-r_{N(A)} + r_{C(B)}$  
    $= 4-(r_{N(A)} - r_{C(B)}) \le 4$
### 4.2 Projections 
Questions 1-9 ask for projections $\bold{p}$ onto lines. Also errors $e = b - p$ and matrices $P$.  
1. Project the vector $\bold{b}$ onto the line through a. Check that $\bold{e}$ is perpendicular to $a$:  
   (a) $\bold{b} = \begin{bmatrix}1 \\ 2 \\ 2  \end{bmatrix}, a = \begin{bmatrix}1 \\ 1 \\ 1  \end{bmatrix}$   
   (b)  $\bold{b} = \begin{bmatrix}1 \\ 3 \\ 1  \end{bmatrix}, a = \begin{bmatrix}-1 \\ -3 \\ -1  \end{bmatrix}$  
   (a) $\bold{p} =\dfrac{1+2+2}{1+1+1}\bold{a} = \begin{bmatrix}\frac{5}{3} \\ \frac{5}{3}  \\ \frac{5}{3}   \end{bmatrix}$  
   $\bold{e} = \begin{bmatrix}-\frac{2}{3} \\ \frac{1}{3} \\ \frac{1}{3} \end{bmatrix}, \bold{e}\cdot\bold{a} = 0$  
   (b) $\bold{p} =\dfrac{-1-9-1}{1+9+1}\bold{a} = \begin{bmatrix}1 \\ 3 \\1   \end{bmatrix}$   
   $\bold{e} = 0, \bold{e}\cdot\bold{a} = 0$  

Questions 11-20 ask for projections, and projection matrices, onto subspaces. 

11.  Project $\bold{b}$ onto the column space of $A$ by solving $A^TA\hat{x}=A^T\bold{b}$ and $\bold{p} = A\hat{x}$:    
(a) $A = \begin{bmatrix}1 & 1 \\0 & 1\\ 0 & 0 \end{bmatrix}$ and $\bold{b} = \begin{bmatrix}2 \\3\\4 \end{bmatrix}$   
(b) $A = \begin{bmatrix}1 & 1 \\1 & 1\\ 0 & 1 \end{bmatrix}$ and $\bold{b} = \begin{bmatrix}4\\4\\6 \end{bmatrix}$      
Find $\bold{e} = \bold{b}-\bold{p}$. It should be perpendicular to the columns of $A$   
(a)$A^T = \begin{bmatrix}1 & 0&0 \\1& 1& 0 \end{bmatrix}$  
$\begin{bmatrix}1 & 1 \\1&2 \end{bmatrix}\hat{x}=\begin{bmatrix}2 \\5 \end{bmatrix}$  
$\hat{x} = \begin{bmatrix}-1 \\3 \end{bmatrix}$  
$\bold{p} = A\hat{x} = \begin{bmatrix}2\\3 \\0 \end{bmatrix}, \bold{e} = \begin{bmatrix}0\\0 \\4\end{bmatrix}$  
(b)$A^T = \begin{bmatrix}1 & 1&0 \\1& 1& 1\end{bmatrix}$   
$\begin{bmatrix}2 & 2\\2&3 \end{bmatrix}\hat{x}=\begin{bmatrix}8 \\14 \end{bmatrix}$   
$\hat{x} = \begin{bmatrix}-2\\6 \end{bmatrix}$  
$\bold{p} = A\hat{x} = \begin{bmatrix}4\\4\\6 \end{bmatrix}, \bold{e} = \begin{bmatrix}0\\0\\0\end{bmatrix}$ 

Questions21-26show that projection matrices satisfy $P^2 = P$ and $P^T = P.$

21. Multiply the matrix $P= A(A^T A)^{-1} A^T$ by itself. Cancel to prove that $P2 = P$. Explain why $P(P\bold{b})$ always equals $P\bold{b}$: The vector $P\bold{b}$ is in the column space of $A$ so its projection onto that column space is *itself*.  
    $P^2 = A(A^T A)^{-1} A^T A(A^T A)^{-1} A^T$  
    $=A I (A^T A)^{-1} A^T=P$

27. The important fact that ends the section is this: If $A^T A\bold{x}  = 0$ then $A\bold{x} = 0.$  New Proof: The vector $A\bold{x}$ is in the nullspace of $A^T$. $A\bold{x}$ is always in the column space of $A$. To be in both of those perpendicular spaces, $A\bold{x}$  must be zero.
#### Challenge Problems
30. (a) Find the projection matrix $P_C$ onto the column space of $A$ (after looking closely at the matrix!)  
    $$A = \begin{bmatrix}3 & 6 & 6 \\ 4 & 8 & 8 \end{bmatrix}$$  
    (b) Find the 3 by 3 projection matrix $P_R$ onto the row space of $A$. Multiply $B = P_CAP_R$. Your answer $B$ should be a little surprising-can you explain it?  
    (a)$P_C = \begin{bmatrix}\frac{9}{25}& \frac{12}{25}  \\ \frac{12}{25} & \frac{16}{25} \end{bmatrix}$   
    (b) $A^T = \begin{bmatrix}3 & 4 \\ 6 & 8 \\ 6 & 8 \end{bmatrix}$  
    $P_R = \begin{bmatrix}\frac{1}{9}& \frac{2}{9} & \frac{2}{9} \\ \frac{2}{9} & \frac{4}{9} & 
    \frac{4}{9} \\ \frac{2}{9} & \frac{4}{9} & 
    \frac{4}{9} \end{bmatrix}$  
    $P_CA =A,AP_R =A, B=A$
### 4.3 Least Squares Approximations
Problems 1-11 use four data points $b = (0, 8, 8, 20)$ to bring out the key ideas.  
1. With $b = 0, 8, 8, 20$ at $t = 0, 1, 3, 4$, set up and solve the normal equations $A^TA\hat{x}=A^T\bold{b}$. For the best straight line in Figure 4.9a, find its four heights $P_i$ and four errors $e_i$. What is the minimum value $E = e_1^2 + e_2^2 + e_3^2 + e_4^2$?   
   $A^TA = \begin{bmatrix}4 & 8 \\ 8 & 26 \end{bmatrix}, A^T\bold{b} = \begin{bmatrix}36  \\ 112 \end{bmatrix}$  
   $\hat{x} = \begin{bmatrix}1 \\ 4 \end{bmatrix}, l:1+4t$  
   $p_i = 1,5,13,17, E = 1+9+25+9=44$

Questions 12-16 introduce basic ideas of statistics-the foundation for least squares. 

12. (Recommended) This problem projects $b = ( b_1, ... , b_m)$ onto the line through $a = 
(1, ... , 1)$. We solve $m$ equations $A\bold{x} = \bold{b}$ in 1 unknown (by least squares).     
(a) Solve $a^Ta\hat{x}=a^T\bold{b}$ to show that $\hat{x}$ is the mean (the average) of the $b$'s.    
(b) Find $e = b - a\hat{x}$ and the variance $||\bold{e}||^2$ and the standard deviation $||\bold{e}||$   
(c) The horizontal line $\hat{b} = 3$ is closest to $b = (1, 2, 6)$. Check that $p = (3, 3, 3)$ is perpendicular to $e$ and find the 3 by 3 projection matrix $P$.   
(a) $a^Ta=m, a^Tb = \sum b_i$  
$\hat{x} = \dfrac{\sum  b_i}{m}$  
(b) $e_i = b_i-\dfrac{\sum  b_i}{m},||e_i||^2 = (b_i-\dfrac{\sum  b_i})^2, ||e|| = |b_i-\dfrac{\sum  b_i}|$     
(c) $\hat{x} = 3,e = (-2,-1,3). e\cdot p = 0$  
$P = \begin{bmatrix}\frac{1}{3} & \frac{1}{3} & \frac{1}{3}  \\ \frac{1}{3}  & \frac{1}{3} & \frac{1}{3}  \\ \frac{1}{3}  & \frac{1}{3}  & \frac{1}{3}  \end{bmatrix}$

Questions 17-24 give more practice with $\hat{x}$ and $p$ and $e$.

17. Write down three equations for the line $b = C + Dt$ to go through $b = 7$ at $t = -1$, $b = 7$ at $t = 1$, and $b = 21$ at $t = 2$. Find the least squares solution $\hat{x} = (C, D)$ and draw the closest line.   
    $A^TA = \begin{bmatrix}3 & 2 \\ 2 & 6 \end{bmatrix}, A^T\bold{b}= \begin{bmatrix}35 \\ 42 \end{bmatrix}$  
    $\hat{x} = \begin{bmatrix}9 \\ 4 \end{bmatrix}, b=9+4t$
#### Challenge Problems
25. What condition on $( t_1, b_1), ( t_2 , b_2), ( t_3, b_3)$ puts those three points onto a straight line? A column space answer is: $(b1 , b2 , b3 )$ must be a combination of $(1, 1, 1)$ and $( t1, t2, t3)$. Try to reach a specific equation connecting the $t$'s and $b$'s. I should have  thought of this question sooner!   
    $\dfrac{b_3-b_2}{t_3-t_2} = \dfrac{b_2-b1}{t_2-t_1}$
### 4.4 Orthonormal Bases and Gram-Schmidt
Problems 1-12 are about orthogonal vectors and orthogonal matrices. 
1. Are these pairs of vectors orthonormal or only orthogonal or only independent?  
(a) $\begin{bmatrix}1  \\ 0 \end{bmatrix}$ and $\begin{bmatrix}-1  \\ 1 \end{bmatrix}$ (b) $\begin{bmatrix}.6  \\ .8 \end{bmatrix}$ and $\begin{bmatrix}.4  \\ -.3 \end{bmatrix}$ (c) $\begin{bmatrix}\cos\theta  \\ \sin\theta \end{bmatrix}$ and $\begin{bmatrix}-\sin\theta  \\ \cos\theta\end{bmatrix}$   
Change the second vector when necessary to produce orthonormal vectors.  
(a) independent. $\begin{bmatrix}0  \\ 1 \end{bmatrix}$  
(b) orthogonal $\begin{bmatrix}-0.8  \\ 0.6 \end{bmatrix}$  
(c) orthonormal 

Problems 13-25 are about the Gram-Schmidt process and $A= QR$.

13. What multiple of $\bold{a}= \begin{bmatrix}1 \\ 1 \end{bmatrix}$ should be subtracted from $\bold{b} = \begin{bmatrix}4  \\ 0\end{bmatrix}$ to make the result $B$ orthogonal to $\bold{a}$? Sketch a figure to show $a, b,$ and $B$.   
    $\dfrac{A^T\bold{b}}{A^TA}A=\dfrac{4}{2}\begin{bmatrix}1 \\ 1 \end{bmatrix}=\begin{bmatrix}2 \\ 2\end{bmatrix}$

Problems 30-35 involve orthogonal matrices that are special. 

30. The first four wavelets are in the columns of this wavelet matrix $W$:   
    $$W = \dfrac{1}{2}\begin{bmatrix}1 & 1 & \sqrt{2} &0 \\ 1 & 1 & -\sqrt{2} &0 \\ 1 & -1 & 0 &\sqrt{2} \\ 1 & -1 & 0 &-\sqrt{2} \end{bmatrix}$$    
    What is special about the columns? Find the inverse wavelet transform $W^{-1}$  
   They are orthonormal.  
   $W^{-1} = \begin{bmatrix} \frac{1}{2} & \frac{1}{2} & \frac{1}{2} &\frac{1}{2} \\ \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} &-\frac{1}{2} \\ \frac{\sqrt{2}}{2} & -\frac{\sqrt{2}}{2} & 0 &0\\ 0 &0&\frac{\sqrt{2}}{2} & -\frac{\sqrt{2}}{2}\end{bmatrix}$

