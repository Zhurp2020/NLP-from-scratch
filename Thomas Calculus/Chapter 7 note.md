# Thomas Calculus
## Chapter 7 Transcendental Functions
### 7.1 Inverse Functions and Their Derivatives
#### One-to-One Functions
>**DEFINITION**  
A function $f(x)$ is one-to-one on a domain $D$ if $f(x_1) \ne f(x_2)$ whenever $x_1 \ne x_2$ in $D$.  
#### Inverse Functions
>**DEFINITION**   
Suppose that $f$ is a one-to-one function on a domain $D$ with range $R$. The inverse function $f^{-1}$ is defined by
>$$
>f^{-1} (b) = a\quad\mathsf{if}\quad f(a) = b.
>$$
The domain of $f^{-1}$ is $R$ and the range of $f^{-1}$ is $D$.
#### Finding Inverses
#### Derivatives of Inverses of Differentiable Functions
>THEOREM 1—The Derivative Rule for Inverses   
If $f$ has an interval $I$ as domain and $f'(x)$ exists and is never zero on $I$, then $f^{-1}$ is differentiable at every point in its domain (the range of $f$ ). The value of $(f^{-1})'$ at a point $b$ in the domain of $f^{-1}$ is the reciprocal of the value of $f'$ at the point $a = f^{-1}(b)$:
>$$
>(f^{-1})'(b) = \dfrac{1}{f'(f^{-1}(b))}
>$$
>or
>$$
>\dfrac{df^{-1}}{dx}|_{x = b} = \dfrac{df}{dx}|_{x = f^{-1}(b)}
>$$
### 7.2 Natural Logarithms
#### Definition of the Natural Logarithm Function
>**DEFINITION** 
The natural logarithm is the function given by
>$$
>\ln x = \int_1^x \dfrac{1}{t}dt, x > 0
>$$

>**DEFINITION** 
The number $e$ is the number in the domain of the natural logarithm that satisfies
>$$
>\ln e = \int_1^e \dfrac{1}{t}dt, x > 0
>$$
#### The Derivative of $y = \ln x$
$$
\dfrac{d}{dx}\ln u = \dfrac{1}{u}\dfrac{du}{dx}, u > 0
$$
#### Properties of Logarithms
>THEOREM 2—Algebraic Properties of the Natural Logarithm   
For any numbers $b > 0$ and $z > 0$, the natural logarithm satisfies the following rules:
>1. Product Rule: 
>$$
>\ln bx = \ln b + \ln x 
>$$
>2. Quotient Rule:
>$$
>\ln \dfrac{b}{x} = \ln b - \ln x 
>$$
>3. Reciprocal Rule: 
>$$
>\ln \dfrac{1}{x}= -\ln x 
>$$
>4. Power Rule: 
>$$
>\ln x^r = r\ln x 
>$$
Proof:
$$
\dfrac{d}{dx}\ln(bx) = \dfrac{b}{bx} = \dfrac{1}{x} = \dfrac{d}{dx}\ln x \\
\ln (bx) = \ln x + C \\
C = \ln b - \ln 1 = \ln b
$$
#### The Graph and Range of $\ln x$
$$
\ln 2 > 1\cdot\dfrac{1}{2} = \dfrac{1}{2}   \\
\ln 2^n = n\ln2 > \dfrac{1}{2} \\
\ln 2^n \to \infty\quad\mathsf{as}\quad n\to\infty  \\
\lim_{x\to\infty}\ln x = \infty \\
\lim_{x\to0^+}\ln x = \lim_{t\to\infty}\ln t^{-1} = -\lim_{t\to\infty}\ln t = -\infty
$$
#### The Integral $\int\dfrac{1}{u} du$
If $u$ is a differentiable function that is never zero, then
$$
\int\dfrac{1}{u} du = \ln |u| + C
$$
#### The Integrals of $\tan x, \cot x, \sec x$, and $\csc x$
$$
\int\tan xdx = \int \dfrac{\sin x}{\cos x} dx\\
\cos x = u, \dfrac{du}{dx} = -\sin x, \sin x dx = -du \\
\int\tan x =\int-\dfrac{1}{u}du = -\ln |u| + C = -\ln |\cos x| +C \\
= \ln |\sec x| + C
$$
>Integrals of the tangent, cotangent, secant, and cosecant functions
>$$
>\int\tan u du = \ln |\sec u| + C \\
>\int\cot u du = \ln |\sin u| + C \\
>\int\sec u du = \ln |\sec u + \tan u| + C \\
>\int\csc u du = \ln |\csc u + \cot u| + C \\
>$$
#### Logarithmic Differentiation
### 7.3 Exponential Functions
#### The Inverse of $\ln x$ and the Number $e$  
$$
\ln e^r = r\ln e = r \\
\ln ^{-1} \ln e^r = \ln ^{-1} r \\
\exp r = e^r
$$
>**DEFINITION**    
For every real number $x$, we define the natural exponential function to be $e^x = \exp x$
>Inverse Equations for $e^x$ and $\ln x$
>$$
>e^{\ln x} = x (\forall x > 0)  \\
>\ln (e^x) = x (\forall x)
>$$
#### The Derivative and Integral of $e^x$
$$
\ln (e^x) = x \\
\dfrac{d}{dx}\ln e^x = 1 \\
\dfrac{1}{e^x}\dfrac{d}{dx}e^x = 1 \\
\dfrac{d}{dx}e^x = e^x 
$$
If $u$ is any differentiable function of $x$, then  
$$
\dfrac{d}{dx}e^u = e^u\dfrac{du}{dx}
$$
>The general antiderivative of the exponential function  
>$$
>\int e^xdx = e^x + C
>$$
#### Laws of Exponents
#### The General Exponential Function $a^x$
>**DEFINITION**   
For any numbers $a > 0$ and $x$, the exponential function with base $a$ is
>$$
>a^x = e^{x \ln a}
>$$
#### Proof of the Power Rule (General Version)
>DEFINITION    
For any $x > 0$ and for any real number $n$,
>$$
>x^n = e^{n \ln x}
>$$
When $x > 0$
$$
\dfrac{d}{dx}x^n = \dfrac{d}{dx}e^{n \ln x} \\
= e^{n \ln x}\dfrac{d}{dx}n \ln x \\
= x^n\dfrac{n}{x} \\
= nx^{n - 1}
$$
When $x < 0$:
$$
\ln |y| = \ln |x^n| = n\ln |x| = n\ln (-x) \\
\dfrac{y'}{y} = \dfrac{n}{x} \\
y' =\dfrac{nx^n}{n} = nx^{n - 1}
$$
#### The Number $e$ Expressed as a Limit
> THEOREM 4—The Number e as a Limit  
The number $e$ can be calculated as the limit
>$$
>e = \lim_{x\to0}(1 + x)^\frac{1}{x}
>$$
Proof
$$
f(x) = \ln x, f'(x) = \dfrac{1}{x}, f'(1) = 1 \\
f'(1) = \lim_{h\to0}\dfrac{f(1 + h) -f(1)}{h} \\
= \lim_{h\to0}\dfrac{\ln (1 + h) - \ln 1}{h}  \\
= \lim_{h\to0}\dfrac{1}{h}\ln(\dfrac{1 + h}{1}) \\
= \lim_{h\to0}\ln(1 + h)^\frac{1}{h} \\
= \ln(\lim_{h\to0}(1 +h)^\frac{1}{h}) = 1 \\
e = \lim_{x\to0}(1 + x)^\frac{1}{x}
$$
#### The Derivative of $a^u$
$$
\dfrac{d}{dx}a^x = \dfrac{d}{dx}e^{x\ln a} = e^{x\ln a}\dfrac{d}{dx}(x\ln a) \\
= a^x\ln a
$$
If $a > 0$ and $u$ is a differentiable function of $x$, then $a^u$ is a differentiable function of $x$ and  
$$
\dfrac{d}{dx}a^u = a^u\ln a \cdot\dfrac{du}{dx} \\
\int a^udu =\dfrac{a^u}{\ln a} + C 
$$
#### Logarithms with Base $a$
$$
\log_ax = \dfrac{\ln x}{\ln a}
$$
#### Derivatives and Integrals Involving $\log_a x$
$$
\dfrac{d}{dx} \log_a u = \dfrac{1}{\ln a}\cdot\dfrac{1}{u}\dfrac{du}{dx}    
$$
### 7.4 Exponential Change and Separable Differential Equations
#### Exponential Change
The solution of the initial value problem
$$
\dfrac{dy}{dt} = ky, y(0) = y_0 \\
\dfrac{1}{y}\dfrac{dy}{dt} = k \\
\int\dfrac{1}{y}\dfrac{dy}{dt}dt = \int kdt \\
\ln |y| + C_1 = kt + C_2 \\
|y| = e^{kt + C_2 - C_1} \\
y = \plusmn e^{C_2 - C_1}\cdot e^{kt} \\
y(0) = \plusmn e^{C_2 - C_1} = y_0 \\
y = y_0e^{kt}
$$
#### Separable Differential Equations
#### Unlimited Population Growth
#### Radioactivity
#### Heat Transfer: Newton’s Law of Cooling
### 7.5 Indeterminate Forms and L’Hôpital’s Rule
#### Indeterminate Form $\dfrac{0}{0}$  
>THEOREM 5—L’Hôpital’s Rule  
Suppose that $f(a) = g(a) = 0$, that $f$ and $g$ are differentiable on an open interval $I$ containing $a$, and that $g'(x) \ne 0$ on $I$ if $x \ne a$. Then
>$$
>\lim_{x\to a}\dfrac{f(x)}{g(x)} = \lim_{x\to a}\dfrac{f'(x)}{g'(x)}
>$$
>assuming that the limit on the right side of this equation exists.
#### Indeterminate Forms $\dfrac{\infty}{\infty},\infty\cdot0,\infty-\infty$  
For $\dfrac{\infty}{\infty}$, L’Hôpital’s Rule still applies
#### Indeterminate Powers
If $\lim\limits_{x\to a}\ln f(x) = L$, then   
$$
\lim\limits_{x\to a}f(x) = \lim\limits_{x\to a}e^{\ln f(x)} = e^L
$$
Here $a$ may be either finite or infinite
#### Proof of L’Hôpital’s Rule
>THEOREM 6—Cauchy’s Mean Value Theorem   
Suppose functions $f$ and $g$ are continuous on $[a, b]$ and differentiable throughout $(a, b)$ and also suppose $g'(x) \ne 0$ throughout $(a, b)$. Then there exists a number $c$ in $(a, b)$ at which  
>$$
>\dfrac{f'(c)}{g'(c)} = \dfrac{f(b)-f(a)}{g(b)-g(a)}
>$$
Proof:   
If $g(a) = g(b)$, then there is a point $c\in(a,b)$ such that 
$$
g'(c) = \dfrac{g(b) - g(a)}{b - a} = 0
$$
But $g'(x) \ne 0$ throughout $(a, b)$, therefore, $g(a) \ne g(b)$   
Let $F(x)$ be
$$
F(x) = f(x) - f(a) - \dfrac{f(b) - f(a)}{g(b) - g(a)}[g(x) - g(a)]
$$
then there is a point $c\in(a,b)$ such that 
$$
F'(c) = f'(c) - \dfrac{f(b) - f(a)}{g(b) - g(a)}g'(x) = 0\\
\dfrac{f'(c)}{g'(c)} = \dfrac{f(b)-f(a)}{g(b)-g(a)}
$$
Proof of L’Hôpital’s Rule:   
Suppose $x > a$, then there is a point $c\in(x,a)$ such that  
$$
\dfrac{f'(c)}{g'(c)} = \dfrac{f(x)-f(a)}{g(x)-g(a)} = \dfrac{f(x)}{g(x)}
$$
As $x\to a^+, c\to a^+$  
$$
\lim_{x\to a^+}\dfrac{f(x)}{g(x)} = \lim_{c\to a^+}\dfrac{f'(c)}{g'(c)} = \lim_{x\to a^+}\dfrac{f'(x)}{g'(x)}
$$   
Similarly, 
$$
\lim_{x\to a^-}\dfrac{f(x)}{g(x)} = \lim_{x\to a^-}\dfrac{f'(x)}{g'(x)}
$$
therefore, 
$$
\lim_{x\to a}\dfrac{f(x)}{g(x)} = \lim_{x\to a}\dfrac{f'(x)}{g'(x)}
$$
### 7.6 Inverse Trigonometric Functions
#### Defining the Inverse Trigonometric Functions
![](../images/Thomas%20Calculus/7-1.jpg)
#### The Arcsine and Arccosine Functions
#### Identities Involving Arcsine and Arccosine
#### Inverses of $\tan x, \cot x, \sec x$, and $\csc x$
#### The Derivative of $y = \arcsin u$
$$
(f^{-1})'(x) = \dfrac{1}{f'(f^{-1}(x))} \\
= \dfrac{1}{\cos(\arcsin x)} \\
= \dfrac{1}{\sqrt{1-\sin^2(\arcsin x)}} \\
= \dfrac{1}{1-x^2}
$$
#### The Derivative of $y = \arctan u$
$$
(f^{-1})'(x) = \dfrac{1}{f'(f^{-1}(x))} \\
= \dfrac{1}{\sec^2(\arctan x)} \\  
= \dfrac{1}{1 + \tan^2(\arctan x)} \\
= \dfrac{1}{1+x^2}
$$
#### The Derivative of $y = arc\sec u$
$$
y = arc\sec x  \\
\sec y = x \\
\dfrac{d}{dx}\sec y = 1 \\
\sec y \tan y\dfrac{dy}{dx}  = 1\\
\dfrac{dy}{dx} = \dfrac{1}{\sec y\tan y}  \\
\sec y = x, \tan y = \plusmn \sqrt{\sec^2 y -1} = \plusmn \sqrt{x^2 - 1} \\
\dfrac{dy}{dx} = \plusmn \dfrac{1}{x\sqrt{x^2 - 1}} \\
= \left\{\begin{aligned}
    \dfrac{1}{x\sqrt{x^2 - 1}} \quad&x > 1\\
    -\dfrac{1}{x\sqrt{x^2 - 1}}\quad&x < -1
\end{aligned}\right. \\
= \dfrac{1}{|x|\sqrt{x^2 - 1}}
$$
#### Derivatives of the Other Three Inverse Trigonometric Functions
>Inverse Function–Inverse Cofunction Identities   
>$$
>\arccos x = \dfrac{\pi}{2} - \arcsin x \\
>\arcctg x = \dfrac{\pi}{2} - \arctan x \\
>arc\csc x = \dfrac{\pi}{2} - arc\sec x
>$$ 
#### Integration Formulas
The following formulas hold for any constant $a > 0$.
1. $\int\dfrac{du}{\sqrt{a^2-u^2}} = \sin^{-1}\dfrac{u}{a} + C$ 
2. $\int\dfrac{du}{\sqrt{a^2+u^2}} = \dfrac{1}{a}\tan^{-1}\dfrac{u}{a} + C$
3. $\int\dfrac{du}{u\sqrt{u^2-a^2}} = \dfrac{1}{a}\sec^{-1}|\dfrac{u}{a}| + C$
### 7.7 Hyperbolic Functions
#### Definitions and Identities
$$
\sinh x = \dfrac{e^x - e^{-x}}{2},\cosh x = \dfrac{e^x + e^{-x}}{2}
$$
![](../images/Thomas%20Calculus/7-2.jpg)
#### Derivatives and Integrals of Hyperbolic Functions
#### Inverse Hyperbolic Functions
![](../images/Thomas%20Calculus/7-3.jpg)  
![](../images/Thomas%20Calculus/7-4.jpg)
#### Useful Identities
#### Derivatives of Inverse Hyperbolic Functions
$$
\dfrac{d\sinh^{-1}u}{dx} = \dfrac{1}{\sqrt{1 + u^2}}\dfrac{du}{dx}  \\
\dfrac{d\cosh^{-1}u}{dx} = \dfrac{1}{\sqrt{u^2 - 1}}\dfrac{du}{dx}, u>1  \\
\dfrac{d\tanh^{-1}u}{dx} = \dfrac{1}{\sqrt{1 - u^2}}\dfrac{du}{dx}, |u|<1  \\
\dfrac{d\coth^{-1}u}{dx} = \dfrac{1}{\sqrt{1 - u^2}}\dfrac{du}{dx}, |u|>1  \\
\dfrac{d\sec h^{-1}u}{dx} = -\dfrac{1}{u\sqrt{1 - u^2}}\dfrac{du}{dx}, 0<u<1  \\
\dfrac{d\csc h^{-1}u}{dx} = -\dfrac{1}{|u|\sqrt{1 + u^2}}\dfrac{du}{dx}, u \ne 0  \\
\int\dfrac{du}{\sqrt{a^2 + u^2}} =\sinh^{-1}(\dfrac{u}{a}) + C, a>0\\
\int\dfrac{du}{\sqrt{ u^2-a^2 }} =\cosh^{-1}(\dfrac{u}{a}) + C , u>a>0\\
\int\dfrac{du}{a^2- u^2} = 
\left\{\begin{aligned}
    \dfrac{1}{a}\tanh^{-1}(\dfrac{u}{a}) + C , u^2<a^2\\ 
    \dfrac{1}{a}\coth^{-1}(\dfrac{u}{a}) + C , u^2>a^2\\
\end{aligned}\right.\\
\int\dfrac{du}{u\sqrt{a^2 -u^2 }} =-\dfrac{1}{a}\sec h^{-1}(\dfrac{u}{a}) + C , u<a<0\\
\int\dfrac{du}{u\sqrt{a^2 +u^2 }} =-\dfrac{1}{a}\sec h^{-1}|\dfrac{u}{a}| + C , u\ne0, a>0
$$
### 7.8 Relative Rates of Growth
#### Growth Rates of Functions
>**DEFINITION**   
Let $f(x)$ and $g(x)$ be positive for $x$ sufficiently large
>1. $f$ grows faster than $g$ as $x \to\infty$ if
>$$
>\lim_{x\to\infty}\dfrac{f(x)}{g(x)} = \infty
>$$
>or, equivalently, 
>$$
>\lim_{x\to\infty}\dfrac{g(x)}{f(x)} = 0
>$$
>We also say that $g$ grows slower than $f$ as $x \to\infty$
>2.  $f$ and $g$ grow at the same rate as $x \to\infty$ if
>$$
>\lim_{x\to\infty}\dfrac{f(x)}{g(x)} = L
>$$
>where $L$ is finite and positive.
#### Order and Oh-Notation
>**DEFINITION**   
A function $f$ is of smaller order than $g$ as $x \to\infty$ if $\lim\limits_{x\to\infty}\dfrac{f(x)}{g(x)} = 0$. We indicate this by writing $f = o(g)$

>**DEFINITION**   
Let $f(x)$ and $g(x)$ be positive for $x$ sufficiently large. Then $f$ is of at most the order of $g$ as $x \to\infty$ if there is a positive integer $M$ for which 
>$$\dfrac{f(x)}{g(x)} \le M$$
>for $x$ sufficiently large. We indicate this by writing $f = O(g)$ 
#### Sequential vs. Binary Search
