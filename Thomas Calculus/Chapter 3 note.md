# Thomas Calculus
## Chapter 3 Derivatives
### 3.1 Tangent Lines and the Derivative at a Point
#### Finding a Tangent Line to the Graph of a Function
>**DEFINITIONS** The slope of the curve $y = f(x)$ at the point $P(x_0, f(x_0))$ is 
>$$
>\lim_{h\to0}\dfrac{f(x_0 + h) - ƒ(x_0)}{h}
>$$
>(provided the limit exists).  
>The tangent line to the curve at $P$ is the line through $P$ with this slope.
#### Rates of Change: Derivative at a Point
>**DEFINITION** The derivative of a function $f$ at a point $x_0$, denoted $f'(x_0)$, is
>$$
>f'(x_0) = \lim_{h\to0}\dfrac{f(x_0 + h) - ƒ(x_0)}{h}
>$$
>provided this limit exists
#### Summary
### 3.2 The Derivative as a Function
If $f′$ exists at a particular $x$, we say that $f$ is differentiable at $x$. If $f′$ exists at every point in the domain of $f$, we call $f$ differentiable
>**Alternative Formula for the Derivative**
>$$
>f'(x) = \lim_{z\to x}\dfrac{f(z) - f(x)}{z - x}
>$$
#### Calculating Derivatives from the Definition
$\dfrac{d}{dx}\dfrac{1}{x}$  
$= \lim\limits_{h\to0}\dfrac{\dfrac{1}{x + h} - \dfrac{1}{x}}{h}$   
$= \lim\limits_{h\to0}\dfrac{\dfrac{x - x - h}{(x + h)x}}{h}$   
$= \lim\limits_{h\to0}\dfrac{-1}{(x + h)x}$   
$= -\dfrac{1}{x^2}$   
Derivative of the Reciprocal Function  
$$
\dfrac{d}{dx}\dfrac{1}{x} = -\dfrac{1}{x^2}, x \ne 0
$$
$\dfrac{d}{dx}\sqrt{x}$  
$= \lim\limits_{z\to x}\dfrac{\sqrt{z} - \sqrt{x}}{z - x}$  
$= \lim\limits_{z\to x}\dfrac{1}{\sqrt{z} + \sqrt{x}}$  
$= \lim\limits_{z\to x}\dfrac{1}{2\sqrt{x}}$  
Derivative of the Square Root Function
$$
\dfrac{d}{dx}\sqrt{x} = \dfrac{1}{2\sqrt{x}}, x > 0
$$
#### Notation
#### Graphing the Derivative
#### Differentiable on an Interval; One-Sided Derivatives
A function $y = f(x)$ is differentiable on an open interval (finite or infinite) if it has a derivative at each point of the interval. It is differentiable on a closed interval $[a, b]$ if it is differentiable on the interior $(a, b)$ and if the limits $\lim_{h\to0^+}\dfrac{f(x_0 + h) - ƒ(x_0)}{h}$(Right-hand derivative at $a$) and $\lim_{h\to0^-}\dfrac{f(x_0 + h) - ƒ(x_0)}{h}$ (Left-hand derivative at $b$) exist at the endpoints.
#### When Does a Function Not Have a Derivative at a Point?
![](../images/Thomas%20Calculus/3-1.jpg) 
#### Differentiable Functions Are Continuous
>**THEOREM 1**—Differentiability Implies Continuity  
>If $ƒ$ has a derivative at $ƒ$, then $ƒ$ is continuous at $x = c$.

Proof:
$$
f(c + h) = f(c) + \dfrac{f(c + h) - f(c)}{h}\cdot h \\
\lim_{h\to 0}f(c + h) = \lim_{h\to 0}f(c) + \lim_{h\to 0}\dfrac{f(c + h) - f(c)}{h}\cdot \lim_{h\to 0}h \\
= f(c) \\ 
\lim_{x\to c} = f(c)
$$
Therefore, $f$ is continuous at $x = c$
### 3.3 Differentiation Rules
#### Powers, Multiples, Sums, and Differences
>Derivative of a Constant Function  
>If $f$ has the constant value $f(x) = c$, then
>$$
>\dfrac{df}{dx} = \dfrac{d}{dx}c = 0
>$$

>Derivative of a Positive Integer Power  
>If $n$ is any real number, then
>$$
>\dfrac{d}{dx}x^n= nx^{n-1}
>$$
>for all $x$ where the powers $x^n$ and $x^{n-1}$ are defined.

Proof:
$$
(z - x)(z^{n-1} + z^{n - 2}x + \cdots + zx^{n - 2} + x^{n - 1})  \\
=z^n + z^{n - 1}x + \cdots + z^2x^{n - 2} + zx^{n - 1}- z^{n-1}x - z^{n - 2}x^2 - \cdots - zx^{n - 1} - x^n\\
= z^n - x^n  \\
f'(x) = \lim_{z\to x}\dfrac{f(z) - f(x)}{z - x} \\
= \lim_{z\to x}\dfrac{z^n - x^n}{z - x} \\
= \lim_{z\to x}(z^{n-1} + z^{n - 2}x + \cdots + zx^{n - 2} + x^{n - 1}) \\
= nx^{n - 1}
$$
>Derivative Constant Multiple Rule  
>If $u$ is a differentiable function of $x$, and $c$ is a constant, then
>$$
>\dfrac{d}{dx}cu= c\dfrac{du}{dx}
>$$

>Derivative Sum Rule
If $u$ and $v$ are differentiable functions of $x$, then their sum $u + v$ is differentiable at every point where $u$ and $v$ are both differentiable. At such points,
>$$
>\dfrac{d}{dx}(u + v) = \dfrac{du}{dx} + \dfrac{dv}{dx}
>$$
#### Products and Quotients
>Derivative Product Rule
If $u$ and $v$ are differentiable at x, then so is their product $uv$, and
>$$
>\dfrac{d}{dx}(uv) = v\dfrac{du}{dx} + u\dfrac{dv}{dx}
>$$

Proof:
$$
\dfrac{d}{dx}(uv) = \lim_{h\to0}\dfrac{uv(x + h) -uv(x)}{h} \\ 
= \lim_{h\to0}\dfrac{u(x + h)v(x + h) -u(x)v(x)}{h} \\
= \lim_{h\to0}\dfrac{u(x + h)v(x + h) +u(x + h)v(x) - u(x + h)v(x) - u(x)v(x)}{h} \\
= \lim_{h\to0}u(x + h)\dfrac{v(x + h) - v(x)}{h} + \lim_{h\to0}v(x)\dfrac{u(x + h)- u(x)}{h} \\
= u\dfrac{dv}{dx} + v\dfrac{du}{dx}
$$
>Derivative Quotient Rule  
If $u$ and $v$ are differentiable at $x$ and if $y(x) \ne 0$, then the quotient $\dfrac{u}{v}$ is differentiable at $x$, and
>$$
>\dfrac{d}{dx}(\dfrac{u}{v}) = \dfrac{v\dfrac{du}{dx} - u\dfrac{dv}{dx}}{v^2}
>$$
#### Second- and Higher-Order Derivatives
$n$th derivative of $y$ with respect to $x$ 
$$
y^{(n)} = \dfrac{d}{dx}y^{(n-1)} = \dfrac{d^ny}{dx^n} =D^ny
$$
### 3.4 The Derivative as a Rate of Change
#### Instantaneous Rates of Change
#### Motion Along a Line: Displacement, Velocity, Speed, Acceleration, and Jerk
#### Derivatives in Economics
#### Sensitivity to Change
### 3.5 Derivatives of Trigonometric Functions
#### Derivative of the Sine Function
$\lim\limits_{h\to 0}\dfrac{\sin h}{h} = 1$   
$\lim\limits_{h\to 0}\dfrac{(\cos h - 1)}{h} = \lim\limits_{h\to 0}\dfrac{(1-2\sin^2\dfrac{h}{2} - 1)}{h} = -\lim\limits_{h\to 0}\dfrac{\sin\dfrac{h}{2}}{\dfrac{h}{2}}\sin\dfrac{h}{2} =0$  
$f(x) = \sin x$   
$f'(x) = \lim\limits_{h\to0}\dfrac{\sin(x + h) - \sin x}{h}$  
$= \lim\limits_{h\to0}\dfrac{\sin x\cos h + \cos x \sin h - \sin x}{h}$  
$= \lim\limits_{h\to0}\dfrac{\sin x(\cos h - 1)+\cos x \sin h }{h}$  
$= \sin x\lim\limits_{h\to0}\dfrac{(\cos h - 1)}{h} + \cos x \lim\limits_{h\to0}\dfrac{\sin h }{h}$  
$=\cos x$
>The derivative of the sine function is the cosine function:  
>$$
>\dfrac{d}{dx}(\sin x) = \cos x.
>$$
#### Derivative of the Cosine Function
$f(x) = \cos x$  
$f'(x) = \lim\limits_{h\to0}\dfrac{\cos(x + h) - \cos x}{h}$  
$= \lim\limits_{h\to0}\dfrac{\cos x\cos h - \sin x \sin h - \cos x}{h}$  
$= \lim\limits_{h\to0}\dfrac{\cos x(\cos h - 1)-\sin x \sin h }{h}$  
$= \cos x\lim\limits_{h\to0}\dfrac{(\cos h - 1)}{h} - \sin x \lim\limits_{h\to0}\dfrac{\sin h }{h}$  
$=-\sin x$
>The derivative of the cosine function is the negative of the sine function:
>$$
>\dfrac{d}{dx}(\cos x) = -\sin x.
>$$
#### Simple Harmonic Motion
#### Derivatives of the Other Basic Trigonometric Functions
>The derivatives of the other trigonometric functions:
>$$
>\dfrac{d}{dx}(\tan x) = \sec^2 x,\dfrac{d}{dx}(\cot x) = -\csc^2x\\
>\dfrac{d}{dx}(\sec x) = \sec x\tan x, \dfrac{d}{dx}(\csc x) = -\csc x\cot x
>$$
### 3.6 The Chain Rule
#### Derivative of a Composite Function
>**THEOREM 2**—The Chain Rule   
>If $f(u)$ is differentiable at the point $u = g(x)$ and $g(x)$ is differentiable at $x$, then the composite function $(f \circ g)(x) = f(g(x))$ is differentiable at $x$, and 
>$$
>(f \circ g)'(x) = f'(g(x))\cdot g'(x)
>$$  
>In Leibniz’s notation, if $y = f(u)$ and $u = g(x)$, then
>$$
>\dfrac{dy}{dx} = \dfrac{dy}{du}\cdot\dfrac{du}{dx}
>$$ 
>where $\dfrac{dy}{du}$ is evaluated at $u = g(x)$

A Proof of One Case of the Chain Rule:   
Let $\Delta u \ne 0$ be the change in $u$ when $x$ changes by $\Delta x$, so that
$$
\Delta u = g(x + \Delta x) - g(x)\\
\Delta y = f(u + \Delta u) - f(u)\\
\dfrac{\Delta y}{\Delta x} = \dfrac{\Delta y}{\Delta u} \cdot \dfrac{\Delta u}{\Delta x} 
$$
If the function $g(x)$ oscillates rapidly near $x$, then $\Delta u$ can be zero even when $\Delta x \ne 0$, so the cancellation would be invalid. 
$$
\dfrac{dy}{dx} = \lim_{\Delta x\to 0}\dfrac{\Delta y}{\Delta x} \\
= \lim_{\Delta x\to 0}\dfrac{\Delta y}{\Delta u} \cdot \dfrac{\Delta u}{\Delta x}\\
= \lim_{\Delta u\to 0}\dfrac{\Delta y}{\Delta u} \cdot \lim_{\Delta x\to 0}\dfrac{\Delta u}{\Delta x}\\
= \dfrac{dy}{du}\cdot\dfrac{du}{dx}
$$
#### “Outside-Inside” Rule
#### Repeated Use of the Chain Rule
#### The Chain Rule with Powers of a Function
If $u$ is a differentiable function of $x$, then we can use the Chain Rule to extend this to the Power Chain Rule:
$$
\dfrac{d}{dx}u^n = nu^{n - 1}\dfrac{du}{dx}
$$ 
### 3.7 Implicit Differentiation
#### Implicitly Defined Functions
Implicit Differentiation
1. Differentiate both sides of the equation with respect to $x$, treating $y$ as a differentiable function of $x$.
2. Collect the terms with $\dfrac{dy}{dx}$ on one side of the equation and solve for $\dfrac{dy}{dx}$.
#### Derivatives of Higher Order
#### Lenses, Tangent Lines, and Normal Lines
### 3.8 Related Rates
#### Related Rates Equations
### 3.9 Linearization and Differentials
#### Linearization
>**DEFINITIONS** If $f$ is differentiable at $x = a$, then the approximating function
>$$
>L(x) = f(a) + f'(a)(x - a)
>$$
>is the linearization of $f$ at $a$. The approximation 
>$$
>f(x) \approx L(x)
>$$ 
of $f$ by L is the standard linear approximation of $f$ at $a$. The point $x = a$ is the center of the approximation.
#### Differentials
>**DEFINITION** Let $y = f(x)$ be a differentiable function. The differential $dx$ is an independent variable. The differential $dy$ is 
>$$
>dy = f'(x)dx
>$$
#### Estimating with Differentials
#### Error in Differential Approximation
>Change in $y = f(x)$ near $x = a$   
If $y = f(x)$ is differentiable at $x = a$ and $x$ changes from $a$ to $a + \Delta x$, the change $\Delta y$ in $f$ is given by
>$$
>\Delta y = f'(a) \Delta x + \varepsilon \Delta x \\
\varepsilon = \dfrac{f(a + \Delta x) - f(a)}{\Delta x} - f'(a)
>$$
>in which $\varepsilon \to 0$ as $\Delta x \to  0$.
#### Proof of the Chain Rule
Let $\Delta x$ be an increment in $\Delta x$ and let $\Delta u$and $\Delta y$ be the corresponding increments in $u$ and $y$
$$
\Delta u = (g'(x_0) + \varepsilon_1) \Delta x \\
\Delta y = (f'(x_0) + \varepsilon_2) \Delta u \\
= (f'(x_0) + \varepsilon_2)(g'(x_0) + \varepsilon_1) \Delta x\\
\dfrac{dy}{dx} = \lim_{\Delta x \to 0}\dfrac{\Delta y}{\Delta x}\\
= \lim_{\Delta x \to 0}(f'(x_0) + \varepsilon_2)(g'(x_0) + \varepsilon_1)\\
= \lim_{\Delta x \to 0}(f'(x_0)g'(x_0) + \varepsilon_2g'(x_0) + \varepsilon_1f'(x_0) + \varepsilon_1\varepsilon_2)
$$
$\varepsilon_2 \to 0$ as $\Delta u \to 0, \varepsilon_1 \to 0$ as $\Delta x \to 0, \Delta u\to 0$ as $\Delta x \to 0$
$$
\therefore \dfrac{dy}{dx} = f'(x_0)g'(x_0) = f'(g(x_0))g'(x_0)
$$
#### Sensitivity to Change
#### Converting Mass to Energy
