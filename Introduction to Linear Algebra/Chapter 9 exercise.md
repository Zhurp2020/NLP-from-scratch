# Introduction to Linear Algebra
## Chapter 9 Complex Vectors and Matrices
### 9.1 Complex Numbers 
Questions 1-8 are about operations on complex numbers. 
1. Add and multiply each pair of complex numbers:   
(a) $2 + i, 2 - i$ (b)$-1+i,-1+i$ (c) $\cos\theta + \sin \theta i, \cos \theta - \sin \theta i$   
(a) $4,5$ (b)$-2+2i,2$ (c)$1$ 
 
Questions 9-16 are about the conjugate $\bar{z} = a - ib = re^{-i\theta} = z^*$. 

9. Write down the complex conjugate of each number by changing $i$ to $-i$ : 
(a) $2 -i$ (b)$(2-i)(1-i)$ (c)$e^{\frac{\pi i}{2}}$ (which is $i$) (d) $e^{\pi i} = -1$ (e) $\frac{1+i}{1-i}$ (which is also $i$) (f) $i^{103}$  

(a) $2 +i$ (b)$1+3i$ (c)$e^{-\frac{\pi i}{2}}$ (which is $i$) (d) $e^{-\pi i}$ (e) $-i$ (f) $i$  

Questions 15-22 are about the form $re^{i\theta}$ of the complex number $r\cos\theta + r\sin \theta i$

15. Write these numbers in Euler's form $re^{i\theta}$. Then square each number:  
(a) $1 + \sqrt{3}i$ (b)$\cos2\theta + \sin 2\theta i$  (c) $-7i$ (d) $5 - 5i.$  
(a) $r = 2,\theta =\frac{\pi}{3},2e^{\frac{\pi}{3}i}, 4e^{\frac{2\pi}{3}i}$  
(b) $e^{2\theta i},e^{4\theta i}$  
(c) $r = 7, \theta = -\frac{\pi}{2},7e^{-\frac{\pi}{2}i},-49$  
(d) $r = 5\sqrt{2},\theta = -\frac{\pi}{4},5\sqrt{2}e^{-\frac{\pi}{4}i},50e^{-\frac{\pi}{2}i}$
### 9.2 Hermitian and Unitary Matrices
1. Find the lengths of $\bold{u} = (1 + i, 1 - i, 1 + 2i)$ and $\bold{v} = (i, i, i)$. Find $\bold{u}^H\bold{v}$ and $\bold{v}^H\bold{u}$  
   $||\bold{u}|| = \sqrt{2+2+5}=3$  
   $||\bold{v}|| = \sqrt{3}$  
   $\bold{u}^H\bold{v} = (1-i)i+(1+i)i+(1-2i)i =3i-2i^2=2+3i$  
   $\bold{v}^H\bold{u} = (-i)(1+i)+(-i)(1-i)+(-i)(1+2i) =2-3i$
### 9.3 The Fast Fourier Transform
1. Multiply the three matrices in equation (3) and compare with $F$. In which six entries do you need to know that $i^2 = -1$?   
   $F = \begin{bmatrix}1 &  &1 & \\ & 1 &  &i\\ 1 &  & -1 & \\ & 1 &  &-i \end{bmatrix}\begin{bmatrix}1 &  1& & \\ 1& i^2 &  &\\  &  & 1 & 1\\ &  & 1 &i^2 \end{bmatrix}\begin{bmatrix}1 &  & & \\ &  & 1 &\\  & 1 &  & \\ &  &  &1 \end{bmatrix}$  
   $=\begin{bmatrix}1 & 1 &1 &1 \\1& i^2 & i &i^3\\ 1 & 1 & -1 &-1 \\ 1& i^2 & -i &-i^3 \end{bmatrix}\begin{bmatrix}1 &  & & \\ &  & 1 &\\  & 1 &  & \\ &  &  &1 \end{bmatrix}$  
   $=\begin{bmatrix}1 & 1 &1 &1 \\1& i & i^2 &i^3\\ 1 & -1 & 1 &-1 \\ 1& -i & i^2 &-i^3 \end{bmatrix} = \begin{bmatrix}1 & 1 &1 &1 \\1& -1 & i &-i\\ 1 & 1 & -1 &-1 \\ 1& -i & -1 &i \end{bmatrix}$