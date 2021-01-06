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
### 8.4 Trigonometric Substitutions
With $x = a \tan\theta,\theta = \tan^{-1}(\dfrac{x}{a}),\dfrac{\pi}{2} < \theta < \dfrac{\pi}{2}$,
$$
a^2 + x^2 = a^2 + a^2\tan^2\theta = a^2(1 + \tan^2\theta) = a^2\sec^2\theta.
$$
With $x = a \sin\theta,\theta = \sin^{-1}(\dfrac{x}{a}),\dfrac{\pi}{2}\le \theta \le \dfrac{\pi}{2}$,
$$
a^2 - x^2 = a^2 - a^2\sin^2\theta = a^2(1 - \sin^2\theta) = a^2\cos^2\theta.
$$
With $x = a \sec\theta,\theta = \sec^{-1}(\dfrac{x}{a}),\left\{\begin{aligned}0 \le \theta<\dfrac{\pi}{2} &\quad\mathsf{if}\quad\dfrac{x}{a} \ge 1 \\  \dfrac{\pi}{2} < \theta \le \pi &\quad\mathsf{if}\quad\dfrac{x}{a} \le -1\end{aligned}\right.$,
$$
x^2 - a^2 = a^2\sec^2\theta - a^2 = a^2(\sec^2\theta-1) = a^2\tan^2\theta.
$$
### 8.5 Integration of Rational Functions by Partial Fractions
#### General Description of the Method
Success in writing a rational function $\dfrac{f(x)}{g(x)}$ as a sum of partial fractions depends on two things:
+ The degree of $f(x)$ must be less than the degree of $g(x)$. 
+ We must know the factors of $g(x)$.

1. Let $x - r$ be a linear factor of $g(x)$. Suppose that $(x - r)^m$ is the highest power of $x - r$ that divides $g(x).$ Then, to this factor, assign the sum of the $m$ partial fractions: 
   $$\dfrac{A_1}{(x - r)} + \dfrac{A_2}{(x - r)^2}+\cdots + \dfrac{A_m}{(x - r)^m} $$
   Do this for each distinct linear factor of $g(x).$  
2. Let $x^2 + px + q$ be an irreducible quadratic factor of $g(x)$ so that $x^2 + px + q$ has no real roots. Suppose that $(x^2 + px + q)^n$ is the highest power of this factor that divides $g(x)$. Then, to this factor, assign the sum of the n partial fractions:
    $$
    \dfrac{B_1x + C_1}{x^2 + px + q} + \dfrac{B_2x + C_2}{(x^2 + px + q)^2} + \cdots + \dfrac{B_nx + C_n}{(x^2 + px + q)^n}
    $$
    Do this for each distinct quadratic factor of $g(x)$.
3. Set the original fraction $\dfrac{f(x)}{g(x)}$ equal to the sum of all these partial fractions. Clear the resulting equation of fractions and arrange the terms in decreasing powers of $x$.
2. Equate the coefficients of corresponding powers of x and solve the resulting equations for the undetermined coefficients
#### Other Ways to Determine the Coefficients
