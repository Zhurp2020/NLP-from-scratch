# Thomas Calculus
## Chapter 8 Techniques of Integration
### 8.1 Using Basic Integration Formulas
#### Assorted Integrations
The integrals in Exercises 1–44 are in no particular order. Evaluate each integral using any algebraic method or trigonometric identity you think is appropriate. When necessary, use a substitution to reduce it to a standard form.

1. $\int_0^1\dfrac{16x}{8x^2+2}dx$  
   Let $8x^2+2 = u, \dfrac{du}{dx} = 16x$  
   $\int_0^1\dfrac{16x}{8x^2+2}dx$  
   $= \int_2^{10}\dfrac{1}{u}de$  
   $= \ln u]_2^{10}$  
   $= \ln10 - \ln 2 = \ln 5$
#### Theory and Examples
45. Area. Find the area of the region bounded above by $y = 2 \cos x$ and below by $y = \sec x, -\dfrac{\pi}{4} \le x \le \dfrac{\pi}{4}$.   
   $S = 2\int_0^{\frac{\pi}{4}}(2\cos x - \sec x)dx$  
   $= 2[2\sin x - \ln |\sec x + \tan x|]_0^{\frac{\pi}{4}}$   
   $= 2(\sqrt{2}-\ln(\sqrt{2}+1))$
### 8.2 Integration by Parts
#### Integration by Parts
Evaluate the integrals in Exercises 1–24 using integration by parts.
1. $\int x\sin\dfrac{x}{2}$  
   Let $u(x) = x,v'(x) = \sin\dfrac{x}{2}$  
   $u'(x) = 1, v(x) = -2\cos\dfrac{x}{2}$   
   $\int x\sin\dfrac{x}{2}$  
   $= x\sin\dfrac{x}{2} - \int-2\cos\dfrac{x}{2}dx$  
   $= x\sin\dfrac{x}{2} + 4\sin\dfrac{x}{2} + C$  
#### Using Substitution
Evaluate the integrals in Exercises 25–30 by using a substitution prior to integration by parts.

25. $\int e^{\sqrt{3s+9}}ds$  
    Let $t = \sqrt{3s+9}, \dfrac{dt}{ds} = \dfrac{3}{2\sqrt{3s+9}} = \dfrac{3}{2t}$    
    $\int e^{\sqrt{3s+9}}ds$  
    $= \int\dfrac{2t}{3}e^tdt$     
    Let $u(t) =\dfrac{2t}{3}, v'(t) = e^t$  
    $u'(t) = \dfrac{2}{3}, v(t) = e^t$  
    $\int\dfrac{1}{3}e^tdt$  
    $= \dfrac{2t}{3}e^t-\int \dfrac{2}{3}e^tdt$  
    $= \dfrac{2t}{3}e^t- \dfrac{2}{3}e^t$
#### Evaluating Integrals
Evaluate the integrals in Exercises 31–56. Some integrals do not require integration by parts.

31. $\int x\sec^2 xdx$  
    Let $x = u(x), v'(x) = \sec^2 x$  
    $u'(x) = 1, v(x) = \tan x$  
    $\int x\sec^2 xdx$  
    $= x\tan x- \int \tan xdx$  
    $= x\tan x -\ln |\sec x| + C$  
#### Theory and Examples
57. Finding area. Find the area of the region enclosed by the curve $y = x \sin x$ and the $x$-axis (see the accompanying figure) for  
a. $0 \le x \le \pi.$    
b. $\pi \le x \le 2\pi.$  
c. $2\pi \le x \le 3\pi.$  
d. What pattern do you see here? What is the area between the curve and the $x$-axis for $n\pi \le x \le (n + 1)\pi, n$ an arbitrary nonnegative integer? Give reasons for your answer.   
![](../images/Thomas%20Calculus/8-1.jpg)
$S_a = \int_0^{\pi}x\sin xdx$  
Let $u(x) = x, v'(x) = \sin x$  
$u'(x) = 1, v(x) = -\cos x$  
$\int x\sin xdx$   
$= -x\cos x - \int -\cos x dx$   
$= \sin x - x\cos x$  
$S_a = \pi$  
$S_b = |-2\pi - \pi| = 3\pi$  
$S_c = 3\pi + 2\pi = 5\pi$    
$S_n = |\sin(n+1)\pi - (n+1)\pi\cos(n+1)\pi - \sin n\pi + n\pi \cos n\pi|$  
If $n$ is even:  
$S_n = 0+(n+1)\pi -0 + n\pi = (2n+1)\pi$  
If $n$ is odd:  
$S_n = |0-(n+1)\pi -0 - n\pi| = (2n+1)\pi$  
$S_n = (2n+1)\pi$  
#### Reduction Formulas
In Exercises 67–71, use integration by parts to establish the reduction formula.

67. $\int x^n\cos xdx = x^n\sin x - n\int x^{n-1}\sin xdx$  
    Let $u(x) = x^n, v'(x) = \cos x$  
    $u'(x) =nx^{n-1}, v(x) = \sin x$  
    $\int x^n\cos xdx$ 
    $= x^n\sin x - \int nx^{n-1}\sin xdx$  
    $= x^n\sin x - n\int x^{n-1}\sin xdx$
#### ntegrating Inverses of Functions
Integration by parts leads to a rule for integrating inverses that usually gives good results:
$$
\int f^{-1}(x)dx = \int yf'(y)dy \\
= yf(y) - \int f(y)dy \\
= xf^{-1}(x) - \int f(y)dy \\
$$
The idea is to take the most complicated part of the integral, in this case $f^{-1}(x)$ and simplify it first. For the integral of $\ln x$, we get
$$
\int \ln xdx = \int ye^ydy \\
= ye^y - \int e^ydy \\
= x\ln x - x + C \\
$$   
For the integral of $\cos^{-1} x$ we get
$$
\int \cos^{-1} xdx = \int -y\sin ydy \\
= y\cos y - \int\cos ydy \\
= x\cos^{-1} x - \sin(\cos^{-1} x) + C \\
$$   
Use the formula
$$
\int f^{-1}(x)dx = xf^{-1}(x) - \int f(y)dy
$$
to evaluate the integrals in Exercises 77–80. Express your answers in terms of $x$.

77. $\int\sin^{-1} x$  
    $\int\sin^{-1} x$  
    $= x\sin^{-1} x - \int\sin ydy$  
    $= x\sin^{-1} x + \cos(\sin^{-1} x) + C$ 
### 8.3 Trigonometric Integrals 
#### Powers of Sines and Cosines
Evaluate the integrals in Exercises 1–22.
1. $\int \cos 2x dx$  
   Let $2x = u, \dfrac{du}{dx} = 2$  
   $\int \cos 2x dx$  
   $=\int\dfrac{1}{2}\cos udu$  
   $= \dfrac{1}{2}\sin u$  
   $= \dfrac{1}{2}\sin 2x$  
#### Integrating Square Roots
Evaluate the integrals in Exercises 23–32.

23. $\int_0^{2\pi}\sqrt{\dfrac{1-\cos x}{2}}dx$  
    $\int_0^{2\pi}\sqrt{\dfrac{1-\cos x}{2}}dx$  
    $= \int_0^{2\pi}\sqrt{\sin^2\dfrac{x}{2}}dx$   
    $= \int_0^{2\pi}\sin\dfrac{x}{2}dx$  
    $= [-2\cos\dfrac{x}{2}]_0^{2\pi}$  
    $= 4$
#### Powers of Tangents and Secants
Evaluate the integrals in Exercises 33–50.

33. $\int\sec^2x \tan x dx$  
    Let $u(x) = \sec x, v'(x) = \sec x\tan x$  
    $u'(x) = \sec x\tan x, v(x) = \sec x$  
    $\int\sec^2x \tan x dx$  
    $= \sec^2x - \int\sec^2x \tan xdx$  
    $2\int\sec^2x \tan x dx = \sec^2 x$  
    $\int\sec^2x \tan x dx = \dfrac{1}{2}\sec^2 x + C$
#### Products of Sines and Cosines
Evaluate the integrals in Exercises 51–56.

51. $\int\sin 3x \cos 2x dx$  
    $\int\sin 3x \cos 2x dx$  
    $= \int\dfrac{1}{2}(\sin x+ \sin 5x)dx$  
    $= \dfrac{1}{2}(-\cos x - \dfrac{1}{5}\cos 5x) + C$  
#### Assorted Integrations
Use any method to evaluate the integrals in Exercises 63–68.

63. $\int\dfrac{\sec^3 x}{\tan x}dx$   
    $\int\dfrac{\sec^3 x}{\tan x}dx$  
    $= \int\dfrac{\tan^2x\sec x + \sec x}{\tan x}dx$  
    $= \int\tan x\sec x +\int \csc x dx$  
    $= \sec x + \ln |\csc x +\cot x| + C$
#### Applications
69. Arc length Find the length of the curve  
    $$
    y = \ln(\sin x), \dfrac{\pi}{6} \le x \le \dfrac{\pi}{2}
    $$
    $\dfrac{dy}{dx}= \cos x\dfrac{1}{\sin x} = \cot x$  
    $l = \int_{\frac{\pi}{6}}^\frac{\pi}{2}\sqrt{1+\cot^2 x}dx$  
    $= \int_{\frac{\pi}{6}}^\frac{\pi}{2}\csc xdx$  
    $= \ln(\csc x + \cot x)]_{\frac{\pi}{6}}^\frac{\pi}{2}$  
    $= \ln1 -\ln(\dfrac{1}{2} + \sqrt{3})$  
    $= -\ln(\dfrac{1}{2}+\sqrt{3})$
### 8.4 Trigonometric Substitutions
#### Using Trigonometric Substitutions
Evaluate the integrals in Exercises 1–14.

1. $\int\dfrac{dx}{\sqrt{9 + x^2}}$   
   Let $x = 3\tan\theta, 9+x^2 = 9(1+\tan^2\theta) = 9\sec^2\theta,\dfrac{dx}{d\theta} =3\sec^2\theta, \theta = \arctan\dfrac{x}{3}\in(-\dfrac{\pi}{2},\dfrac{\pi}{2})$  
   $\int\dfrac{dx}{\sqrt{9 + x^2}}$   
   $= \int\dfrac{3\sec^2\theta}{3|\sec \theta|}d\theta$  
   $= \int\sec \theta d\theta$  
   $= \ln|\sec \theta + \tan \theta| + C$  
   $= \ln(\dfrac{\sqrt{x^2 + 9}}{3}+\dfrac{x}{3}) + C$
#### Assorted Integrations
Use any method to evaluate the integrals in Exercises 15–34. Most will require trigonometric substitutions, but some can be evaluated by
other methods.

15. $\int\dfrac{xdx}{\sqrt{9 - x^2}}$  
    Let $x = 3\sin\theta, 9-x^2 = 9(1-\sin^2\theta) = 9\cos^2\theta,\dfrac{dx}{d\theta} =3\cos\theta, \theta = \arcsin\dfrac{x}{3}\in[-\dfrac{\pi}{2},\dfrac{\pi}{2}]$  
   $\int\dfrac{xdx}{\sqrt{9 - x^2}}$   
   $= \int\dfrac{9\sin\theta\cos\theta}{3|\cos \theta|}d\theta$  
   $= \int3\sin\theta d\theta$  
   $= -3\cos \theta + C$   
   $= -3\sqrt{1-\dfrac{x^2}{9}} + C$   
   $= -\sqrt{9-x^2} + C$
#### Complete the Square Before Using Trigonometric Substitutions
For Exercises 49–52, complete the square before using an appropriate trigonometric substitution.
 
49. $\int\sqrt{8-2x-x^2}dx$   
    $\int\sqrt{8-2x-x^2}dx$  
    $= \int\sqrt{-(x+1)^2+9}dx$  
    Let $t = x + 1 = 3\sin\theta, 9-(x+1)^2 = 9(1-\sin^2\theta) = 9\cos^2\theta,\dfrac{dt}{d\theta} =3\cos\theta, \theta = \arcsin\dfrac{t}{3}\in[-\dfrac{\pi}{2},\dfrac{\pi}{2}]$   
    $\int\sqrt{-(x+1)^2+9}dx$  
    $= \int3\cos\theta\sqrt{9\cos^2\theta}d\theta$  
    $= \int9\cos^2\theta d\theta$  
    $= 9\int\dfrac{1+\cos2\theta}{2}d\theta$  
    $= \dfrac{9}{2}(\theta + \dfrac{1}{2}\sin2\theta) + C$   
    $= \dfrac{9}{2}\arcsin\dfrac{x+1}{3}+ \dfrac{9}{4}\cdot2\dfrac{x+1}{3}\sqrt{1-\dfrac{x^2+2x+1}{9}} + C$  
    $= \dfrac{9}{2}\arcsin\dfrac{x+1}{3}+ \dfrac{1}{2}(x + 1)\sqrt{8-2x-x^2} + C$
#### Initial Value Problems
Solve the initial value problems in Exercises 53–56 for $y$ as a function of x.

53. $x\dfrac{dy}{dx} = \sqrt{x^2-4}, x \ge 2, y(2) = 0$  
    $\dfrac{dy}{dx} = \dfrac{\sqrt{x^2-4}}{x}$   
    $y = \int\dfrac{\sqrt{x^2-4}}{x}dx$  
    Let $x = 2\sec \theta, \dfrac{dx}{d\theta} = 2\sec\theta\tan\theta, x^2-4 = 4(\sec^2 -1) = 4\tan^2\theta, \theta = \sec^{-1}\dfrac{x}{2}\in[0,\dfrac{\pi}{2})$  
    $y = \int\dfrac{\sqrt{4\tan^2\theta}}{2\sec\theta}2\sec\theta\tan\theta d\theta$  
    $= \int2\tan^2\theta d\theta$  
    $= 2\int\sec^2\theta -1d\theta$  
    $= 2\tan\theta- 2\theta + C$  
    $= \sqrt{x^2-4} - 2 \sec^{-1}\dfrac{x}{2} + C$  
    $y(2) =-2  \sec^{-1}1 + C = 0$  
    $C = 0$  
    $y = sqrt{x^2-4} - 2 \sec^{-1}\dfrac{x}{2}$
#### Applications and Examples
57. Area. Find the area of the region in the first quadrant that is enclosed by the coordinate axes and the curve $y = \dfrac{\sqrt{9-x^2}}{3}$  
    $x = 0, y = 1, x = 3, y = 0$  
    $S = \int_0^3\dfrac{\sqrt{9-x^2}}{3}dx$  
    Let $x = 3\sin\theta, 9-x^2 = 9(1-\sin^2\theta) = 9\cos^2\theta,\dfrac{dx}{d\theta} =3\cos\theta, \theta = \arcsin\dfrac{x}{3}\in[-\dfrac{\pi}{2},\dfrac{\pi}{2}]$  
    $\int\dfrac{\sqrt{9-x^2}}{3}dx$  
    $= \int\dfrac{\sqrt{9\cos^2\theta}}{3}3\cos\theta d\theta$  
    $= \int3\cos^2\theta d\theta$  
    $= \dfrac{3}{2}\int1+\cos2\theta d\theta$  
    $= \dfrac{3}{2}(\theta + \dfrac{1}{2}\sin2\theta) + C$  
    $= \dfrac{3}{2}(\arcsin\dfrac{x}{3} + \dfrac{x}{3}\sqrt{1-\dfrac{x^2}{9}}) + C$  
    $= \dfrac{3}{2}\arcsin\dfrac{x}{3} + \dfrac{x}{6}\sqrt{9-x^2} + C$  
    $S = [\dfrac{3}{2}\arcsin\dfrac{x}{3} + \dfrac{x}{6}\sqrt{9-x^2}]_0^3$    
    $= \dfrac{3}{2}\dfrac{\pi}{2} + 0 - 0 -0 = \dfrac{3}{4}\pi$
### 8.5 Integration of Rational Functions by Partial Fractions
#### Expanding Quotients into Partial Fractions
Expand the quotients in Exercises 1–8 by partial fractions.
1. $\dfrac{5x - 13}{(x - 3)(x - 2)}$  
   $\dfrac{5x - 13}{(x - 3)(x - 2)} = \dfrac{A}{x - 3} + \dfrac{B}{x - 2}$  
   $5x - 13 = A(x - 2) + B(x -3) = (A + B)x - (2A + 3B)$  
   $\left\{\begin{aligned} A + B &= 5 \\ 2A + 3B &= 13\end{aligned}\right.$  
   $\left\{\begin{aligned} A &= 8 \\ B &= -3\end{aligned}\right.$  
   $\dfrac{5x - 13}{(x - 3)(x - 2)} = \dfrac{8}{x - 3} - \dfrac{3}{x - 2}$
#### Nonrepeated Linear Factors
In Exercises 9–16, express the integrand as a sum of partial fractions and evaluate the integrals.

9. $\int\dfrac{dx}{1-x^2}$  
   $\dfrac{1}{1-x^2} = \dfrac{A}{1-x} + \dfrac{B}{1 + x}$  
   $1 = A + Ax + B - Bx$   
   $\left\{\begin{aligned} A + B &= 1 \\ A - B &= 0\end{aligned}\right.$  
   $\left\{\begin{aligned} A &= \dfrac{1}{2}\\ B &= \dfrac{1}{2}\end{aligned}\right.$  
   $\dfrac{1}{1-x^2} = \dfrac{1}{2}(\dfrac{1}{1-x} + \dfrac{1}{1 + x})$  
   $\int\dfrac{dx}{1-x^2}$  
   $= \dfrac{1}{2}(\int\dfrac{1}{1-x}dx + \int\dfrac{1}{1+x}dx)$  
   $= \dfrac{1}{2}(-\ln |1-x| + \ln|1 + x|) + C$
#### Repeated Linear Factors
In Exercises 17–20, express the integrand as a sum of partial fractions and evaluate the integrals.

17. $\int_0^1\dfrac{x^3dx}{x^2+2x+1}$  
    $\dfrac{x^3dx}{x^2+2x+1} = x - 2 + \dfrac{3x +2}{x^2 + 2x + 1}$
    $\dfrac{3x +2}{(x + 1)^2} = \dfrac{A}{x + 1} + \dfrac{B}{(x + 1)^2}$  
    $3x +2= Ax + A + B$  
    $\left\{\begin{aligned} A &= 3\\ B &= -1\end{aligned}\right.$  
    $\int\dfrac{x^3dx}{x^2+2x+1}$  
    $= \int x -2 + \dfrac{3}{x + 1} - \dfrac{1}{(x + 1)^2}dx$  
    $= \dfrac{1}{2}x^2-2x+3\ln|x + 1| + \dfrac{1}{x + 1} + C$  
    $\int_0^1\dfrac{x^3dx}{x^2+2x+1}$  
    $= \dfrac{1}{2}-2+3\ln 2+ \dfrac{1}{2}-1$  
    $= 3\ln 2 -2$
#### Irreducible Quadratic Factors
In Exercises 21–32, express the integrand as a sum of partial fractions and evaluate the integrals.

21. $\int_0^1\dfrac{dx}{(x+1)(x^2+1)}$  
    $\dfrac{1}{(x+1)(x^2+1)} = \dfrac{A}{x + 1} + \dfrac{Bx + C}{x^2 + 1}$  
    $1 = Ax^2 + A + Bx^2 + (B + C)x + C$  
    $\left\{\begin{aligned} A + B &= 0 \\ B + C &= 0 \\ A +C &= 1\end{aligned}\right.$  
   $\left\{\begin{aligned} A &= \dfrac{1}{2}\\ B &= -\dfrac{1}{2}\\ C &= \dfrac{1}{2}\end{aligned}\right.$  
   $\dfrac{1}{(x+1)(x^2+1)} = \dfrac{1}{2}(\dfrac{1}{x + 1} + \dfrac{1 - x}{x^2 + 1})$  
   $\int\dfrac{dx}{(x+1)(x^2+1)}$  
   $= \dfrac{1}{2}\int\dfrac{1}{x + 1} + \dfrac{1 - x}{x^2 + 1}dx$  
   $= \dfrac{1}{2}(\ln |x + 1| - \int \dfrac{x - 1}{x^2 + 1}dx) + C$  
   Let $u(x) = x -1, v'(x) = \dfrac{1}{x^2 + 1}$  
   $u'(x) = 1, v(x) = \arctan x$  
   $\int \dfrac{x - 1}{x^2 + 1}dx$  
   $= (x-1)\arctan x- \int \arctan x dx$   
   $\int \arctan x dx = x\arctan x - \int\tan(y) dy$  
   $= x\arctan x - \ln |\sec(\arctan x)| + C$  
   $= x\arctan x - \ln \sqrt{x^2 + 1} + C$ 
   $\int \dfrac{x - 1}{x^2 + 1}dx$  
   $= -\arctan x + \ln\sqrt{x^2 + 1} + C$  
   $\int\dfrac{dx}{(x+1)(x^2+1)}$  
   $= \dfrac{1}{2}(\ln |x + 1| + \arctan x - \ln \sqrt{x^2 + 1}) + C$  
   $\int_0^1\dfrac{dx}{(x+1)(x^2+1)}$  
   $= \dfrac{1}{2}(\ln 2 + \dfrac{\pi}{4}- \dfrac{1}{2}\ln 2)$  
   $= \dfrac{1}{4}\ln 2 + \dfrac{\pi}{8}$  
#### Improper Fractions
In Exercises 33–38, perform long division on the integrand, write the proper fraction as a sum of partial fractions, and then evaluate the
integral.
 
33. $\int\dfrac{2x^3-2x^2 + 1}{x^2 -x}dx$  
    $\dfrac{2x^3-2x^2 + 1}{x^2 -x}$  
    $= 2x + \dfrac{1}{x(x -1)}$  
    $\dfrac{1}{x(x -1)} = \dfrac{1}{x -1}-\dfrac{1}{x}$  
    $\int\dfrac{2x^3-2x^2 + 1}{x^2 -x}dx$  
    $= \int 2x + \dfrac{1}{x-1} - \dfrac{1}{x}dx$  
    $= x^2 + \ln|x -1| - \ln |x|$  
#### Evaluating Integrals
Evaluate the integrals in Exercises 39–54.

39. $\int\dfrac{e^tdt}{e^{2t} + 3e^t + 2}$  
    Let $x = e^t$  
    $\int\dfrac{e^tdt}{e^{2t} + 3e^t + 2}= \int\dfrac{x}{(x + 2)(x + 1)}dx$  
    $\dfrac{x}{(x + 2)(x + 1)} = \dfrac{A}{x+2} + \dfrac{B}{x+1}$  
    $\left\{\begin{aligned} A + B &= 1  \\ A +2B &= 0\end{aligned}\right.$  
   $\left\{\begin{aligned} A &= 2\\ B &= -1\\ \end{aligned}\right.$  
   $\dfrac{x}{(x + 2)(x + 1)} = (\dfrac{2}{x+2} - \dfrac{1}{x+1})$  
   $\int\dfrac{x}{(x + 2)(x + 1)}dx$  
   $= \int \dfrac{2}{x+2} - \dfrac{1}{x+1}dx$  
   $= 2\ln|x + 2| - \ln |x+ 1|$  
   $\int\dfrac{e^tdt}{e^{2t} + 3e^t + 2}= 2\ln|e^t + 2| - \ln |e^t+ 1|$
#### nitial Value Problems
Solve the initial value problems in Exercises 67–70 for $x$ as a function of $t.$

67. $(t^2 - 3t + 2)\dfrac{dx}{dt} = 1 (t > 2), x(3) = 0$  
    $\dfrac{dx}{dt}= \dfrac{1}{t^2 - 3t + 2} = \dfrac{1}{t - 2} - \dfrac{1}{t - 1}$  
    $x = \int\dfrac{1}{t - 2} - \dfrac{1}{t - 1}dt$  
    $= \ln |t - 2| - \ln |t - 1| + C$  
    $x(3) = \ln 1 - \ln 2 + C = 0, C = \ln 2$  
    $x = \ln |t - 2| - \ln |t - 1| + \ln 2$  
#### Applications and Examples
In Exercises 71 and 72, find the volume of the solid generated by revolving the shaded region about the indicated axis.

71. The $x$-axis  
    ![](../images/Thomas%20Calculus/8-2.jpg)  
    $V = \int_{\frac{1}{2}}^{\frac{5}{2}}\pi \dfrac{9}{3x - x^2}dx$  
    $\dfrac{9}{x(3-x)} = 3(\dfrac{1}{x} + \dfrac{1}{3-x})$  
    $\int \dfrac{9}{3x - x^2}dx$  
    $= 3\int\dfrac{1}{x} + \dfrac{1}{3-x}dx$    
    $= 3(\ln |x| - \ln |3-x|) + C$  
    $V = 3\pi(\ln \dfrac{5}{2} + \ln \dfrac{1}{2} - \ln \dfrac{1}{2} + \ln \dfrac{5}{2})$  
    $= 6\pi\ln\dfrac{5}{2}$
### 8.6 Integral Tables and Computer Algebra Systems
#### Using Integral Tables
Use the table of integrals at the back of the book to evaluate the integrals in Exercises 1–26.
1. $\int\dfrac{dx}{x\sqrt{x-3}}$  
   $\int\dfrac{dx}{x\sqrt{x-3}}$  
   $= \dfrac{2}{\sqrt{b}}\tan^{-1}\sqrt{\dfrac{x-3}{b}} + C$
#### Substitution and Integral Tables
In Exercises 27–40, use a substitution to change the integral into one you can find in the table. Then evaluate the integral.

27. $\int\dfrac{x^3 + x + 1}{(x^2 + 1)^2}dx$   
    $\int\dfrac{x^3 + x + 1}{(x^2 + 1)^2}dx$  
    $= \int\dfrac{x}{x^2 + 1} + \dfrac{1}{(x^2 + 1)^2}dx$  
    Let $u = x^2 + 1, \dfrac{du}{dx} = 2x$  
    $\int\dfrac{x}{x^2 + 1}dx$  
    $= \int\dfrac{1}{2}\dfrac{du}{u}$  
    $= \dfrac{1}{2}\ln |u| + C$  
    $\int \dfrac{1}{(x^2 + 1)^2}dx$  
    $= \dfrac{x}{2(x^2 + 1)} + \dfrac{1}{2}\arctan x + C$  
    $\int\dfrac{x^3 + x + 1}{(x^2 + 1)^2}dx$
    $= \dfrac{1}{2}\ln(x^2 + 1) + \dfrac{x}{2(x^2 + 1)} + \dfrac{1}{2}\arctan x + C$
#### Using Reduction Formulas
Use reduction formulas to evaluate the integrals in Exercises 41–50.

41. $\int\sin^52x dx$  
    $\int\sin^52x dx$  
    $= \dfrac{\sin^42x}{5} + \dfrac{4}{5}\int\sin^3 2xdx$  
    $= \dfrac{\sin^42x}{5} + \dfrac{4}{5}(\dfrac{\sin^22x}{3} + \dfrac{2}{3}\int\sin 2xdx)$  
    $= \dfrac{\sin^42x}{5} + \dfrac{4}{15}\sin^2 2x - \dfrac{4}{15}\cos 2x + C$
#### Applications
57. Surface area. Find the area of the surface generated by revolving the curve $y = \sqrt{x^2 + 2},0 \le x \le \sqrt{2}$ about the $x$-axis.  
    $\dfrac{dy}{dx} = \dfrac{x}{\sqrt{x^2 + 2}}$ 
    $S = \int_0^{\sqrt{2}}2\pi\sqrt{x^2 + 2}\sqrt{1 + \dfrac{x^2}{x^2 + 2}}dx$  
    $= 2\pi\int_0^{\sqrt{2}}\sqrt{2x^2 + 2}dx$  
    $= 2\sqrt{2}\pi\int_0^{\sqrt{2}}\sqrt{x^2 + 1}dx$     
    $\int\sqrt{x^2 + 1}dx$    
    $= \dfrac{x}{2}\sqrt{1 + x^2} + \dfrac{1}{2}\ln (x + \sqrt{x^2 + 1}) + C$  
    $S = 2\sqrt{2}\pi [\dfrac{\sqrt{2}}{2}\sqrt{3}+\dfrac{1}{2}\ln(\sqrt{2} + \sqrt{3}) - \dfrac{1}{2}\ln 1]$  
    $= (2\sqrt{3}+\sqrt{2}\ln(\sqrt{2}+\sqrt{3}))\pi$
#### COMPUTER EXPLORATIONS
In Exercises 65 and 66, use a CAS to perform the integrations.

65. Evaluate the integrals  
a. $\int x \ln xdx$  b. $\int x^2 \ln xdx$ c. $\int x^3 \ln xdx$  
d. What pattern do you see? Predict the formula for $\int x^4 \ln xdx$ and then see if you are correct by evaluating it with a CAS.
e. What is the formula for $\int x^n \ln xdx,n\ge 1$? Check your answer using a CAS.  
a. Let $u(x) = \ln x, v'(x)= x$  
$u'(x) = \dfrac{1}{x}, v(x) = \dfrac{1}{2}x^2$  
$\int x \ln xdx$    
$= \dfrac{1}{2}x^2\ln x - \int\dfrac{1}{2}xdx$   
$=\dfrac{1}{2}x^2\ln x- \dfrac{1}{4}x^2$   
b. Let $u(x) = \ln x, v'(x)= x^2$  
$u'(x) = \dfrac{1}{x}, v(x) = \dfrac{1}{3}x^3$  
$\int x \ln xdx$    
$= \dfrac{1}{3}x^3\ln x - \int\dfrac{1}{3}x^2dx$   
$=\dfrac{1}{3}x^3 - \dfrac{1}{9}x^3$  
c. Let $u(x) = \ln x, v'(x)= x^3$  
$u'(x) = \dfrac{1}{x}, v(x) = \dfrac{1}{4}x^4$  
$\int x \ln xdx$    
$= \dfrac{1}{4}x^4\ln x - \int\dfrac{1}{4}x^3dx$   
$=\dfrac{1}{4}x^4\ln x - \dfrac{1}{16}x^4$  
d. $\dfrac{1}{5}x^5\ln x - \dfrac{1}{25}x^5$  
e. $\dfrac{1}{n+1}x^{n + 1}\ln x - \dfrac{1}{(n+1)^2}x^{n + 1}$
