# Thomas Calculus
## Chapter 8 Techniques of Integration
### 8.1 Using Basic Integration Formulas
### 8.2 Integration by Parts
#### Product Rule in Integral Form
>Integration by Parts Formula  
>$$
>\int u(x)v'(x)dx = u(x)v(x)-\int u'(x)v(x)dx
>$$
#### Evaluating Definite Integrals by Parts
### 8.3 Trigonometric Integrals
#### Products of Powers of Sines and Cosines
$\int\sin^mx\cos^nxdx$  
If $m$ is odd    
$\sin^mx = \sin^{2k+1}x = (1-\cos^2x)^k\sin x$   
$\int\sin^mx\cos^nxdx = \int(1-\cos^2x)^k\sin x\cos^nxdx =  \int(1-\cos^2x)^k\cos^nx(-d\cos x)$
If $n$ is odd  
$\cos^nx = \cos^{2k+1}x = (1-\sin^2x)^k\cos x$  
$\int\sin^mx\cos^nxdx = \int(1-\sin^2x)^k\cos x\sin^mxdx =  \int(1-\sin^2x)^k\sin^mxd\sin x$   
If $m$ and $n$ are even, use:  
$\sin^2x = \dfrac{1-\cos2x}{2},\cos^2x = \dfrac{1+\cos2x}{2}$  
#### Eliminating Square Roots
$\cos^2\theta =  \dfrac{1+\cos2\theta}{2}$ 
#### Integrals of Powers of $\tan x$ and $\sec x$
$\tan^2x = \sec^2x-1, \sec^2x = \tan^2x+1$
#### Products of Sines and Cosines
$$
\sin mx\sin nx = \dfrac{1}{2}[\cos(m-n)x-\cos(m+n)x] \\
\sin mx\cos nx = \dfrac{1}{2}[\sin(m-n)x+\sin(m+n)x] \\
\cos mx\sin nx = \dfrac{1}{2}[\cos(m-n)x+\cos(m+n)x] \\
$$