# Introduction to Linear Algebra
## Chapter 5 Determinants
### 5.1 The Properties of Determinants
Questions 1-12 are about the rules for determinants. 
1. If a 4 by 4 matrix has $\det{A} = \dfrac{1}{2}$, find $\det{2A}$ and $\det{-A}$ and $\det{A^2}$ and $\det{A^{-1}}$.   
   $\det{2A} = 2^4\cdot\dfrac{1}{2} = 8$  
   $\det{-A} = \dfrac{1}{2}$  
   $\det{A^2}=\dfrac{1}{4}$  
   $\det{A^{-1}} = 2$   

Questions 13-27 use the rules to compute specific determinants. 

13. Reduce $A$ to $U$ and find $\det{A}$ = product of the pivots:  
    $A = \begin{bmatrix}1 & 1& 1 \\ 1 & 2 & 2 \\ 1 & 2 & 3 \end{bmatrix}$ and  $A = \begin{bmatrix}1 & 2& 3 \\ 2 & 2 & 3 \\ 3 & 3& 3 \end{bmatrix}$   
    $A\rArr \begin{bmatrix}1 & 1& 1 \\ 0 & 1 & 1 \\ 0& 0 & 1 \end{bmatrix}, \det A =1$   
    $A\rArr \begin{bmatrix}1 & 2& 3 \\ 0 &-2 & -3 \\ 0& 0 & -\frac{3}{2} \end{bmatrix}, \det A =3$  

28. True or false (give a reason if true or a 2 by 2 example if false):  
(a) If $A$ is not invertible then $AB$ is not invertible.   
(b) The determinant of $A$ is always the product of its pivots.  
( c) The determinant of $A - B$ equals $\det A - \det B$.      
(d) $AB$ and $BA$ have the same determinant.  
(a) True. $\det AB =0$  
(b) True.  
(c) True. $(a-p)(d-s)-(b-q)(c-r) = ad-ps-bc+qr = ad-bc-(ps-qr)$  
(d) True. $|A||B|=|B||A|$
### 5.2 Permutations and Cofactors 
Problems 1-10 use the big formula with $n!$ terms: $|A|= \sum \plusmn a_{1\alpha}a_{2\beta},\cdots a_{n\omega}$. Every term uses each row and each column once.   
1. Compute the determinants of $A, B, C$ from six terms. Are their rows independent?  
   $A = \begin{bmatrix}1 & 2 & 3 \\ 3 & 1 & 2 \\ 3 & 2 & 1 \end{bmatrix},B = \begin{bmatrix}1 & 2 & 3 \\ 4 & 4 & 4 \\ 5& 6 &7 \end{bmatrix}, C = \begin{bmatrix}1 & 1 & 1 \\ 1 & 1 & 0 \\ 1& 0& 0 \end{bmatrix}$  
   $|A| =1+12+18-4-6-9=12$  
   $|B| = 28+40+72-2-56-60=22$  
   $|C| = 0+0+0-0-0-1=-1$

Problems 11-22 use cofactors $C_{ij} = (-1)^{i+j} \det M_{ij}$. Remove row $i$ and column $j$. 

11. Find all cofactors and put them into cofactor matrices $C, D$. Find $AC$ and $\det B$   
    $A = \begin{bmatrix}a & b  \\ c & d \end{bmatrix},B = \begin{bmatrix}1 & 2 & 3 \\ 4 & 5 & 6 \\ 7& 0 &0 \end{bmatrix}$  
    $C = \begin{bmatrix}d & -c  \\ -b & a \end{bmatrix}, AC = \begin{bmatrix}ad-b^2 &-ac-ab \\  cd-bd &-c^2+ad \end{bmatrix}$  
    $D = \begin{bmatrix}0 & 42 &-35  \\ 0 &-21&14 \\ -3 & 6 &-3\end{bmatrix}$  
    $\det B = -21$

Problems 23-26 are about block matrices and block determinants. 

23. With 2 by 2 blocks in 4 by 4 matrices, you cannot always use block determinants:  
    $\begin{vmatrix}A &B  \\ 0 & D \end{vmatrix} = |A||D|$, but $\begin{vmatrix}A &B  \\ C & D \end{vmatrix} \ne |A||D|-|B||C|$  
(a) Why is the first statement true? Somehow $B$ doesn't enter.  
(b) Show by example that equality fails (as shown) when $C$ enters.  
(c) Show by example that the answer $\det(AD -CB)$ is also wrong.  
(a) With row exchanges, entries in $B$ will always multiply to 0  
(b) $A = \begin{bmatrix}1 & 0  \\ 0 &0 \end{bmatrix},B = \begin{bmatrix}0 & 0  \\ 1 &0 \end{bmatrix},C = \begin{bmatrix}0 & 0 \\ 1 &0 \end{bmatrix}D= \begin{bmatrix}0 & 0  \\ 0 &1 \end{bmatrix}$
#### Challenge Problems 
32. Cofactors of the 1, 3, 1 matrices in Problem 21 give a recursion $S_n = 3S_{n-l} -S_{n-2}$. Amazingly that recursion produces every second Fibonacci number. Here is the challenge.   
Show that $S_n$ is the Fibonacci number $F_{2n+2}$ by proving $F_{2n+2} = 3F_{2n} - F_{2n-2}$   
Keep using Fibonacci's rule $F_k = F_{k-1} + F_{k-2}$ starting with $k = 2n + 2.$   
$F_{2n+3} =F_{2n+2}+F_{2n+1}$  
$F_{2n+1} =F_{2n}+F_{2n-1}$  
$F_{2n+2} = F_{2n+2}+F_{2n+1}-F_{2n}-F_{2n-1}=F_{2n+1}+F_{2n}+F_{2n}+F_{2n-1}-F_{2n-1}-F_{2n-2}-F_{2n-1}=3F_{2n}-F_{2n-2}$
### 5.3 Cramer's Rule, Inverses, and Volumes
Problems 1-5 are about Cramer's Rule for $\bold{x}=A^{-1}\bold{b}$  
1. Solve these linear equations by Cramer's Rule $x_j = \dfrac{\det B_j}{\det A}$   
   (a) $\begin{aligned}2x_1+5x_2=1 \\ x_1 + 4x_2 = 2 \end{aligned}$  (b)$\begin{aligned}2x_1+x_2=1 \\ x_1 + 2x_2 +x_3= 0\\x_2 + 2x_3 = 0 \end{aligned}$    
   (a) $\det A = 3, \det B_1 =-6, \det B_2 = 3$  
   $x_1 = -2, x_2 = 1$  
   (b) $A = \begin{vmatrix}
    2 & 1 & 0 \\ 1 &2& 1\\ 0& 1 & 2
   \end{vmatrix}$  
   $\det A =6-1=2, \det B_1 =3, \det B_2=-1, \det B_3 =1$  
   $x_1 = \dfrac{3}{4}, x_2 = -\dfrac{1}{2}, x_3 = \dfrac{1}{4}$  
Problems 6-15 are about $A^{-1} = \dfrac{C^T}{\det A}$. Remember to transpose $C$.   

6. Find $A^{-1}$ from the cofactor formula  $\dfrac{C^T}{\det A}$. Use symmetry in part (b)  
   (a) $A = \begin{bmatrix}1 & 2 & 0 \\ 0 & 3 & 0 \\ 0& 7& 1 \end{bmatrix}$  (b)$A = \begin{bmatrix}2 & -1 & 0 \\ -1 & 2 & -1 \\ 0& -1& 2 \end{bmatrix}$  
   (a)$C = \begin{bmatrix}3 & 0 & 0 \\ -2 & 1 & -7 \\ 0& 0& 3 \end{bmatrix},\det A =3$  
   $A^{-1} = \begin{bmatrix}1 & -\frac{2}{3} & 0 \\ 0 & \frac{1}{3} &0 \\ 0& -\frac{7}{3}& 1 \end{bmatrix}$  
   (b)$C = \begin{bmatrix}3& 2 & 1 \\ 2 & 4 & 2 \\1& 2& 3 \end{bmatrix},\det A =4$   
   $A^{-1} = \begin{bmatrix}\frac{3}{4} & \frac{1}{2} & \frac{1}{4} \\ \frac{1}{4} & 1 &\frac{1}{4} \\ \frac{1}{4}& \frac{1}{2}& \frac{3}{4} \end{bmatrix}$  

Problems 16-26 are about area and volume by determinants. 

16. (a) Find the area of the parallelogram with edges $\bold{v} = (3, 2)$ and $\bold{w} = (1, 4)$.    
(b) Find the area of the triangle with sides $\bold{v}$,$\bold{w}$ and $\bold{v} + \bold{w}$ Draw it.  
(c) Find the area of the triangle with sides $\bold{v}$, $\bold{w}$, and $\bold{w} - \bold{v}$. Draw it.   
(a) $S = 12-2=10$  
(b) $\bold{v} + \bold{w}=(4,6),S = \dfrac{1}{2}(18-8)=5$  
(c) $S = \dfrac{1}{2}\cdot10=5$  

Problems 27-30 are about areas $dA$ and volumes $dV$ in calculus.

27. Polar coordinates satisfy $x = r \cos \theta$ and $y = r \sin \theta$. Polar area is $J dr d\theta$:   
    $J = \begin{vmatrix}\frac{\partial x}{\partial r} & \frac{\partial x}{\partial \theta}   \\ \frac{\partial y}{\partial r} & \frac{\partial y}{\partial \theta} \end{vmatrix}=\begin{vmatrix}\cos \theta & -r\sin \theta   \\ \sin \theta & r\cos \theta\end{vmatrix}$  
    The two columns are orthogonal. Their lengths are 1 and $r^2$ . Thus $J = r$

Problems 31-38 are about the triple product $(\bold{u} \times \bold{v} )\cdot \bold{w}$ in three dimensions. 

31. A box has base area $||\bold{u}\times\bold{v}||$. Its perpendicular height is $||\bold{w}||\cos\theta$. Base area times height= volume=$||\bold{u}\times\bold{v}||||\bold{w}||\cos\theta$ which is $(\bold{u} \times \bold{v} )\cdot \bold{w}$. Compute base area, height, and volume for $\bold{u} = (2, 4, 0), \bold{v} = (-1, 3, 0), \bold{w} = (1, 2, 2).$     
    $||\bold{u}\times\bold{v}||=||0\bold{i}+0\bold{j}+10\bold{k}||=10$  
    $\cos\theta=\dfrac{20}{30}=\dfrac{2}{3},h=2$  
    $V =20$
#### Challenge Problems 
39. If you know all 16 cofactors of a 4 by 4 invertible matrix $A$, how would you find $A$?  
    $\det A \det C = (\det A)^n$ construct $A^{-1}$ then inverse. 
