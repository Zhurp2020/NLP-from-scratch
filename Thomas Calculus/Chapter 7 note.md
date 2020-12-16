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
>\ln x = \int_1^e \dfrac{1}{t}dt, x > 0
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