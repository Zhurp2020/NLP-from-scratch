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
2. Equate the coefficients of corresponding powers of $x$ and solve the resulting equations for the undetermined coefficients
#### Other Ways to Determine the Coefficients
### 8.6 Integral Tables and Computer Algebra Systems
#### Integral Tables
#### Reduction Formulas
$$
\int\tan^nx dx =\dfrac{1}{n - 1}\tan^{n-1}x - \int\tan^{n-2}xdx \\
\int(\ln x)^n dx = x(\ln x)^n - n\int(\ln x)^{n-1} dx \\
\int\sin^nx cos^m x dx = -\dfrac{\sin^{n-1}x \cos^{m+1} x}{m + n} + \dfrac{n-1}{m+n}\int\sin^{n-2}x \cos^m x dx (n ≠ -m)
$$
#### Integration with a CAS
#### Nonelementary Integrals
### 8.7 Numerical Integration
#### Trapezoidal Approximations
>The Trapezoidal Rule  
To approximate $\int^b_af(x) dx$, use
>$$
>T =\dfrac{\Delta x}{2}(y_0 + 2y_1 + 2y_2 + \cdots + 2y_{n-1} + y_n).
>$$
>The y’s are the values of $f$ at the partition points
>$$
>x_0 = a, x_1 = a + \Delta x, x2 = a + 2\Delta x,\cdots, x_{n-1} = a + (n - 1)\Delta x, x_n = b,
>$$
>where $\Delta x = \dfrac{b-a}{n}$
#### Simpson’s Rule: Approximations Using Parabolas
>Simpson’s Rule  
To approximate $\int^b_af(x) dx$, use
>$$
>S =\dfrac{\Delta x}{3}(y_0 + 4y_1 + 2y_2 + 4y_3 + \cdots + 2y_{n-2} + 4y_{n-1} + y_n).
>$$
>The $y$’s are the values of $f$ at the partition points
>$$
>x_0 = a, x_1 = a + \Delta x, x2 = a + 2\Delta x,\cdots, x_{n-1} = a + (n - 1)\Delta x, x_n = b,
>$$
>The number $n$ is even, and $\Delta x = \dfrac{b-a}{n}$
#### Error Analysis
>THEOREM 1—Error Estimates in the Trapezoidal and Simpson’s Rules   
If $f''$ is continuous and $M$ is any upper bound for the values of $|f''|$ on $[a, b]$ , then the error $E_T$ in the trapezoidal approximation of the integral of $f$ from $a$ to $b$ for $n$ steps satisfies the inequality
>$$
>| E_T| \le \dfrac{M(b - a)^3}{12n^2}
>$$
>If $f^4$ is continuous and $M$ is any upper bound for the values of $|f^4|$ on $[a, b]$, then the error $E_S$ in the Simpson’s Rule approximation of the integral of $f$ from $a$ to $b$ for $n$ steps satisfies the inequality
>$$
>|E_S| \le \dfrac{M(b - a)^5}{108n^4}
>$$
### 8.8 Improper Integrals
#### Infinite Limits of Integration
>DEFINITION Integrals with infinite limits of integration are improper integrals of type i.  
>1. If $f(x)$ is continuous on $[a, \infty)$, then
>$$
>\int^\infty_af(x) dx = \lim_{b\to\infty}\int^b_af(x) dx
>$$
>2. If $f(x)$ is continuous on $(-\infty, b]$ , then
>$$
>\int^b_{-\infty}f(x) dx = \lim_{a\to-\infty}\int^b_af(x) dx
>$$
>3. If $f(x)$ is continuous on $(-\infty, \infty)$, then
>$$
>\int^\infty_{-\infty}f(x) dx = \int^c_{-\infty}f(x) dx + \int^\infty_cf(x) dx
>$$
>where $c$ is any real number.  
>In each case, if the limit exists and is finite, we say that the improper integral converges and that the limit is the value of the improper integral. If the limit fails to exist, the improper integral diverges.
#### The Integral $\int^\infty_1\dfrac{dx}{x^p}$
the improper integral converges if $p > 1$ and diverges if $p < 1.$
#### Integrands with Vertical Asymptotes
>DEFINITION Integrals of functions that become infinite at a point within the interval of integration are improper integrals of type ii.
>1. If $f(x)$ is continuous on $(a, b]$ and discontinuous at $a$, then
>$$
>\int^b_af(x) dx = \lim_{c\to a^+}\int^b_cf(x) dx 
>$$
>2. If $f(x)$ is continuous on $[a, b)$ and discontinuous at $b$, then
>$$
>\int^b_af(x) dx = \lim_{c\to b^-}\int^c_af(x) dx 
>$$
>3. If $f(x)$ is discontinuous at $c$, where $a < c < b$, and continuous on $[a, c) \cup (c, b]$ , then
>$$
>\int^b_af(x) dx = \int^c_af(x) dx+  \int^b_cf(x) dx 
>$$
>In each case, if the limit exists and is finite, we say the improper integral converges and that the limit is the value of the improper integral. If the limit does not exist, the integral diverges
#### Improper Integrals with a CAS
#### Tests for Convergence and Divergence
>THEOREM 2—Direct Comparison Test
Let $f$ and $g$ be continuous on $[a, \infty)$ with $0 \le f(x) \le g(x)$ for all $x \ge a$. Then
>1. If $\int^\infty_ag(x) dx$ converges, then $\int^\infty_af(x) dx$ also converges.
>2. If $\int^\infty_af(x) dx$ diverges, then $\int^\infty_ag(x) dx$ also diverges.

>THEOREM 3—Limit Comparison Test  
If the positive functions $f$ and $g$ are continuous on $[a, \infty)$, and if
>$$
>\lim_{x\to\infty}\dfrac{f(x)}{g(x)} = L, 0<L<\infty
>$$
>then
>$$
>\int^\infty_af(x) dx\quad\mathsf{and}\quad\int^\infty_ag(x) dx
>$$
>either both converge or both diverge.
### 8.9 Probability
#### Random Variables
>**DEFINITION** A random variable is a function $X$ that assigns a numerical value to each outcome in a sample space.
#### Probability Distributions
>**DEFINITIONS** A probability density function for a continuous random variable is a function $f$ defined over $(-\infty, \infty)$ and having the following properties:
>1. $f$ is continuous, except possibly at a finite number of points.
>2. $f$ is nonnegative, so $f \ge 0$.
>3. $\int^\infty_{-\infty}f(x)dx = 1$
If $X$ is a continuous random variable with probability density function $ƒ$, the probability that $X$ assumes a value in the interval between $X = c$ and $X = d$ is given by the integral
>$$
>P(c \le X \le d ) = \int^d_cf(x) dx.
>$$
#### Exponentially Decreasing Distributions
$$
f(x) = \left\{\begin{aligned}
    0      \quad&x <   0\\
    ce^{-x}\quad&x \ge 0
\end{aligned}\right.
$$
#### Expected Values, Means, and Medians
>**DEFINITION** The expected value or mean of a continuous random variable $X$ with probability density function $f$ is the number
>$$
>\mu = E(X) =\int^\infty_{-\infty}xf(x) dx
>$$

>Exponential Density Function for a Random Variable $X$ with Mean $\mu$
>$$
>f(x) = \left\{\begin{aligned}
>    0      \quad&x <   0\\
>    \mu^{-1}e^{-\frac{x}{u}}\quad&x \ge 0
>\end{aligned}\right.
>$$

>**DEFINITION** The median of a continuous random variable $X$ with probability density function $f$ is the number $m￥ for which
>$$
>\int^m_{-\infty}f(x) dx = \dfrac{1}{2}\quad\mathsf{and}\quad\int^\infty_mf(x) dx = \dfrac{1}{2}
>$$
#### Variance and Standard Deviation
>**DEFINITIONS** The variance of a random variable $X$ with probability density function $f$ is the expected value of $(X - \mu)^2$:
>$$
>Var(x)= \quad\int^\infty_{-\infty}(x - \mu)^2f(x ) dx
>$$
>The standard deviation of $X$ is
>$$
>\sigma_X = \sqrt{Var(x)} = \sqrt{\int^\infty_{-\infty}(x - m)^2f(x ) dx}
>$$
#### Uniform Distributions
$$
f(x) = \dfrac{1}{a - b}, a\le x \le b
$$
If each outcome in the sample space is equally likely to occur, then the random variable $X$ has a uniform distribution. 
#### Normal Distributions
$$
f(x) = \dfrac{1}{\sigma\sqrt{2\pi}}e^{-\frac{(x-\mu)^2}{2\sigma^2}}
$$