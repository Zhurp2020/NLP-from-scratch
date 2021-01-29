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
### 8.7 Numerical Integration
#### Estimating Definite Integrals
The instructions for the integrals in Exercises 1–10 have two parts, one for the Trapezoidal Rule and one for Simpson’s Rule.  
i. Using the trapezoidal rule  
a. Estimate the integral with $n = 4$ steps and find an upper bound for $|E_T|$.  
b. Evaluate the integral directly and find $|E_T|$  
c. Use the formula $\dfrac{|E_T|}{true\quad value} * 100$ to express $|E_T|$ as a percentage of the integral’s true value.  
ii. Using simpson’s rule  
a. Estimate the integral with $n = 4$ steps and find an upper bound for $|E_S|$ .  
b. Evaluate the integral directly and find $|E_S|$  
c. Use the formula $\dfrac{|E_S|}{true\quad value} * 100$ to express  $|E_S|$ as a percentage of the integral’s true value.
1. $\int_1^2xdx$  
   i. a. $T = \dfrac{\frac{1}{4}}{2}(1 + 2\dfrac{5}{4} + 2\dfrac{3}{2} + 2\dfrac{7}{4} + 2)$  
   $= \dfrac{1}{8}12$  
   $= \dfrac{3}{2}$  
   $f'' = 0, M = 1$  
   $|E_T| \le \dfrac{1}{192}$  
   b. $\int_1^2xdx = [\dfrac{1}{2}x^2]_1^2 =\dfrac{3}{2}$   
   c. $0\%$  
   ii a. $S = \dfrac{\frac{1}{4}}{3}(1 + 4\dfrac{5}{4} + 2\dfrac{3}{2} + 4\dfrac{7}{4} + 2)$  
   $= \dfrac{1}{12}18 = \dfrac{3}{2}$  
   $|E_S| \le \dfrac{1}{46080}$  
#### Estimating the Number of Subintervals
In Exercises 11–22, estimate the minimum number of subintervals needed to approximate the integrals with an error of magnitude less than $10^{-4}$ by (a) the Trapezoidal Rule and (b) Simpson’s Rule. (The integrals in Exercises 11–18 are the integrals from Exercises 1–8.)  

11. $\int_1^2xdx$  
    $|E_T| \le \dfrac{1}{12n^2} \le 10^{-4}$  
    $n^2 \ge \dfrac{1}{12*10^{-4}}, n \ge 29$  
    $|E_S| \le \dfrac{1}{180n^2} \le 10^{-4}$  
    $n^4 \ge \dfrac{1}{180*10^{-4}}, n \ge 3$
#### Estimates with Numerical Data
23. Volume of water in a swimming poo.l A rectangular swimming pool is 30 ft wide and 50 ft long. The accompanying table shows the depth $h(x)$ of the water at 5-ft intervals from one end of the pool to the other. Estimate the volume of water in the pool using the Trapezoidal Rule with $n = 10$ applied to the integral  
    $$
    \int_0^{50}30h(x)dx
    $$

| position (ft)$x$ | Depth (ft)$h(x)$ | position (ft)$x$ | Depth (ft)$h(x)$ |
| :------------: | :------------: | :------------: | :------------: |
|       0        |      6.0       |       30       |      11.5      |
|       5        |      8.2       |       35       |      11.9      |
|       10       |      9.1       |       40       |      12.3      |
|       15       |      9.9       |       45       |      12.7      |
|       20       |      10.5      |       50       |      13.0      |
|       25       |      11.0      |
$T = 15990$  
#### Theory and Examples
27. Usable values of the sine-integral function. The sine-integral function,
$$  
si(x)=\int_0^x\dfrac{\sin t}{t}dt
$$
is one of the many functions in engineering whose formulas cannot be simplified. There is no elementary formula for the antiderivative of $\dfrac{\sin t}{t}$. The values of $Si(x)$, however, are readily estimated by numerical integration.  
Although the notation does not show it explicitly, the function being integrated is 
$$
f(t) = 
\left\{\begin{aligned}
    \dfrac{\sin t}{t} &,t \ne 0 \\
    1                 &,t = 0
\end{aligned}\right.
$$  
the continuous extension of $\dfrac{\sin t}{t}$ to the interval $[0, x]$ . The function has derivatives of all orders at every point of its domain. Its graph is smooth, and you can expect good results from Simpson’s Rule.  
a. Use the fact that $|f^{(4)}|\le 1$ on $[0, \dfrac{\pi}{2}]$ to give an upper bound for the error that will occur if
$$  
si(\dfrac{\pi}{2})=\int_0^{\frac{\pi}{2}}\dfrac{\sin t}{t}dt
$$
is estimated by Simpson’s Rule with $n = 4.$  
b. Estimate $si(\dfrac{\pi}{2})$ by Simpson’s Rule with $n = 4.$  
c. Express the error bound you found in part (a) as a percentage of the value you found in part (b).  
a. $|E_S| \le \dfrac{(\frac{\pi}{2})^3}{180*4^4} = \dfrac{\pi^5}{368640}$  
b. $S = \dfrac{\frac{\pi}{8}}{3}(1 + 4\dfrac{\sin\frac{\pi}{8}}{\frac{\pi}{8}} + 2\dfrac{\sin\frac{\pi}{4}}{\frac{\pi}{4}} + 4\dfrac{\sin\frac{3\pi}{8}}{\frac{3\pi}{8}} + \dfrac{\sin\frac{\pi}{2}}{\frac{\pi}{8}})$  
$\approx 1.62$  
c.$0.05\%$
#### Applications
32. The length of one arch of the curve $y = \sin x$ is given by
    $$
    L = \int_0^{\pi}\sqrt{1+\cos^2x}dx
    $$
    Estimate $L$ by Simpson’s Rule with $n = 8.$
    $L = \dfrac{\frac{\pi}{8}}{3}(1+4\sqrt{1+\cos^2\dfrac{\pi}{8}} + 2\sqrt{1+\cos^2\dfrac{\pi}{4}} + 4\sqrt{1+\cos^2\dfrac{3\pi}{8}} + 2\sqrt{1+\cos^2\dfrac{\pi}{2}} + 4\sqrt{1+\cos^2\dfrac{5\pi}{8}} + 2\sqrt{1+\cos^2\dfrac{3\pi}{4}} + 4\sqrt{1+\cos^2\dfrac{7\pi}{8}} + \sqrt{1+\cos^2\pi})$  
    $\approx 3.65$
### 8.8 Improper Integrals 
#### Evaluating Improper Integrals
The integrals in Exercises 1–34 converge. Evaluate the integrals without using tables.
1. $\int_0^{\infty}\dfrac{dx}{1+x^2}$  
   $\int_0^{\infty}\dfrac{dx}{1+x^2}$  
   $= \lim\limits_{b\to\infty}\int_0^{b}\dfrac{dx}{1+x^2}$  
   $= \lim\limits_{b\to\infty}[\arctan x]_0^{b}$  
   $= \lim\limits_{b\to\infty}\arctan b = \dfrac{\pi}{2}$  
#### Testing for Convergence
In Exercises 35–68, use integration, the Direct Comparison Test, or the Limit Comparison Test to test the integrals for convergence. If more than one method applies, use whatever method you prefer.   

35. $\int_{\frac{1}{2}}^2\dfrac{dx}{x\ln x}$   
    $\int_{\frac{1}{2}}^2\dfrac{dx}{x\ln x}$  
    $= \int_{\frac{1}{2}}^{1}\dfrac{dx}{x\ln x} + \int_{1}^2\dfrac{dx}{x\ln x}$    
    $= \lim\limits_{b\to1^-}\int_{\frac{1}{2}}^{b}\dfrac{dx}{x\ln x} + \lim\limits_{a\to1^+}\int_{a}^{2}\dfrac{dx}{x\ln x}$  
    $= \lim\limits_{b\to1^-}\ln |\dfrac{\ln b}{\ln \frac{1}{2}}| +\lim\limits_{a\to1^+}\ln |\dfrac{\ln 2}{\ln a}|$    
    Does not converge
#### Theory and Examples
69. Find the values of $p$ for which each integral converges.   
a. $\int_1^2\dfrac{dx}{x(\ln x)^p}$  
b. $\int_1^{\infty}\dfrac{dx}{x(\ln x)^p}$   
a.  when $p= 1,$ does not converge, when $p \ne 1$  
    $\int_{\frac{1}{2}}^2\dfrac{dx}{x(\ln x)^p}$  
    $= \int_{\frac{1}{2}}^{1}\dfrac{dx}{x(\ln x)^p} + \int_{1}^2\dfrac{dx}{x(\ln x)^p}$    
    $= \lim\limits_{b\to1^-}\int_{\frac{1}{2}}^{b}\dfrac{dx}{x(\ln x)^p} + \lim\limits_{a\to1^+}\int_{a}^{2}\dfrac{dx}{x(\ln x)^p}$  
    $= \lim\limits_{b\to1^-}\dfrac{(\ln b)^{1-p} - (\ln \frac{1}{2})^{1-p}}{1-p} +\lim\limits_{a\to1^+}\dfrac{(\ln 2)^{1-p} - (\ln a)^{1-p}}{1-p}$, converges  
b. when $p= 1,$ does not converge, when $p \ne 1$  
    $\int_{\frac{1}{2}}^{\infty}\dfrac{dx}{x(\ln x)^p}$  
    $= \lim\limits_{b\to1^-}\dfrac{(\ln b)^{1-p} - (\ln \frac{1}{2})^{1-p}}{1-p} +\lim\limits_{a\to\infty}\dfrac{(\ln 2)^{1-p} - (\ln a)^{1-p}}{1-p}$  
    $p > 1,$ converges  
    $p < 1,$ does not converge. 
#### COMPUTER EXPLORATIONS
In Exercises 87–90, use a CAS to explore the integrals for various values of p (include noninteger values). For what values of $p$ does the integral converge? What is the value of the integral when it does converge? Plot the integrand for various values of $p$.

87. $\int_0^ex^p\ln xdx$
### 8.9 Probability 
#### Probability Density Functions
In Exercises 1–8, determine which are probability density functions and justify your answer.
1. $f(x) = \dfrac{1}{18}x$ over $[4, 8]$  
   $\int_4^8f(x)dx$  
   $= \dfrac{1}{9}x^2]_4^8$  
   $= \dfrac{16}{3}$ not a pdf. 
#### Exponential Distributions
29. Digestion time. The digestion time in hours of a fixed amount of food is exponentially distributed with a mean of 1 hour. What is the probability that the food is digested in less than 30 minutes?    
    $f(x) = e^{-x}$  
    $P = \int_0^{\frac{1}{2}}f(x)dx$  
    $= 1- \dfrac{1}{\sqrt{e}}$
#### Normal Distributions
39. cholesterol levels. The serum cholesterol levels of children aged 12 to 14 years follows a normal distribution with mean $m = 162$ mg/dl and standard deviation $s = 28$ mg/dl. In a population of 1000 of these children, how many would you expect to have serum cholesterol levels between 165 and 193? between 148 and 167?  
    $f(x) = \dfrac{1}{28\sqrt{2\pi}}e^{-\frac{(x-162)^2}{1568}}$  
    $P_1 = \int_{165}^{193}f(x)dx \approx 0.32$  
    $P_2 = \int_{148}^{167}f(x)dx \approx 0.36$
#### Discrete Random Variables
53. A fair coin is tossed four times and the random variable $X$ assigns the number of tails that appear in each outcome.  
a. Determine the set of possible outcomes.  
b. Find the value of $X$ for each outcome.   
c. Create a probability bar graph for $X$, as in Figure 8.21. What is the probability that at least two heads appear in the four tosses of the coin?  
a. $\{HTTT, HHTT, HHHT, HHHH, TTTT, TTTH, TTHH, THHH, THTH, HTHT,HTTH,THHT,HTHH, HHTH, THTT, TTHT\}$  
b. $\{3,2,1,0,4,3,2,1,2,2,2,2,1,1,3,3,\}$   
c. $P = \dfrac{3}{8}+ \dfrac{1}{4} + \dfrac{1}{16} = \dfrac{11}{16}$  
### Practice Exercises
#### Integration by Parts
Evaluate the integrals in Exercises 1–8 using integration by parts.
1. $\int\ln (x + 1) dx$  
   Let $u(x) = \ln(x + 1), v'(x) = 1$  
   $u'(x) = \dfrac{1}{x + 1}, v(x) = x$  
   $\int\ln (x + 1) dx$  
   $= x\ln(x + 1) - \int\dfrac{x}{x + 1}dx$  
   $= x\ln(x + 1) - \int1 - \dfrac{1}{x + 1}dx$  
   $= x\ln(x + 1) - x + \ln(x + 1) + C$
#### Partial Fractions
Evaluate the integrals in Exercises 9–28. It may be necessary to use a substitution first.

9. $\int\dfrac{xdx}{x^2-3x+2}$  
   $\dfrac{x}{x^2-3x+2} = \dfrac{2}{x - 2} - \dfrac{1}{x - 1}$  
   $\int\dfrac{xdx}{x^2-3x+2}$  
   $= \int\dfrac{2}{x - 2} - \dfrac{1}{x - 1}dx$  
   $= 2\ln|x-2| - \ln |x-1| + C$
#### Trigonometric Substitutions
Evaluate the integrals in Exercises 29–32 (a) without using a trigonometric substitution, (b) using a trigonometric substitution.

29. $\int\dfrac{ydy}{\sqrt{16-y^2}}$   
    Let $u= 16-y^2, \dfrac{du}{dy} = -2y$  
    $\int-\dfrac{1}{2}\dfrac{1}{\sqrt{u}}du$  
    $= -\sqrt{u}+ C$  
    $= -\sqrt{16-y^2} + C$   
    Let $y = 4\sin\theta, 16-y^2 = 16(1-\sin^2\theta) = 16\cos^2\theta,\dfrac{dy}{d\theta} =4\cos\theta, \theta = \arcsin\dfrac{y}{4}\in[-\dfrac{\pi}{2},\dfrac{\pi}{2}]$  
    $\int\dfrac{ydy}{\sqrt{16-y^2}}$  
    $= \int\dfrac{4\sin\theta}{4\cos\theta}4\cos\theta d\theta$  
    $= 4\int\sin\theta d\theta$  
    $= -4\cos\theta + C$  
    $= -4\sqrt{1-\dfrac{x^2}{16}} + C$  
    $= -\sqrt{16-y^2} + C$
#### Trigonometric Integrals
Evaluate the integrals in Exercises 37–44.

37. $\int\sin^3x\cos^4xdx$  
    $\sin^3x = \sin^2x\sin x = (1-\cos^2x)\sin x$  
    $\int\sin^3x\cos^4xdx$  
    $= \int(1-\cos^2x)\sin x\cos^4xdx$  
    Let $u = \cos x,\dfrac{du}{dx} = -\sin x$  
    $\int(1-\cos^2x)\sin x\cos^4xdx$  
    $= \int-(1-u^2)u^4du$  
    $= \int u^6du - \int u^4du$  
    $= \dfrac{1}{7}u^7 - \dfrac{1}{5}u^5 + C$  
    $= \dfrac{1}{7}\cos^7 x - \dfrac{1}{5}\cos^5 x + C$  
#### Numerical Integration
45. According to the error-bound formula for Simpson’s Rule, how many subintervals should you use to be sure of estimating the value of
    $$
    \ln 3 = \int_1^3\dfrac{1}{x}dx
    $$
    by Simpson’s Rule with an error of no more than $10^{-4}$ in absolute value? (Remember that for Simpson’s Rule, the number of subintervals has to be even.)   
    $f' = -\dfrac{1}{x^2}, f'' = \dfrac{2}{x^3} \le 2$  
    $|E_S| \le \dfrac{3*32}{180n^4} \le 10^{-4}$  
    $n \ge 10$  
#### Improper Integrals
Evaluate the improper integrals in Exercises 53–62.

53. $\int_0^3\dfrac{dx}{\sqrt{9-x^2}}$  
    $\int_0^3\dfrac{dx}{\sqrt{9-x^2}}$  
    $= \lim\limits_{b\to3^-}\int_0^b\dfrac{dx}{\sqrt{9-x^2}}$  
    $= \lim\limits_{b\to3^-}\arcsin\dfrac{b}{3}$  
    $= \dfrac{\pi}{2}$
#### Assorted Integrations
Evaluate the integrals in Exercises 69–136. The integrals are listed in random order so you need to decide which integration technique to use.

69. $\int xe^{2x}dx$  
    Let $u(x) = x, v'(x) = e^{2x}$  
    $u'(x) = 1, v(x) = \dfrac{1}{2}e^{2x}$  
    $\int xe^{2x}dx$  
    $= \dfrac{x}{2}e^{2x} - \int \dfrac{1}{2}e^{2x}dx$  
    $= \dfrac{x}{2}e^{2x} - \dfrac{1}{4}e^{2x}  + C$
### Additional and Advanced Exercises
#### Evaluating Integrals
Evaluate the integrals in Exercises 1–6.
1. $\int\arcsin^2 xdx$  
   Let $u(x) = \arcsin^2 x, v'(x) = 1$  
   $u'(x) =\dfrac{2}{\sqrt{1-x^2}}\arcsin x, v(x) = x$   
   $\int\arcsin^2 xdx$  
   $= x\arcsin^2 x - 2\int x\dfrac{1}{\sqrt{1-x^2}}\arcsin xdx$   
   Let $u(x) = \arcsin x, v'(x)= \dfrac{x}{\sqrt{1-x^2}}$  
   $u'(x) = \dfrac{1}{\sqrt{1-x^2}}, v(x) = -\sqrt{1-x^2}$  
   $\int x\dfrac{1}{\sqrt{1-x^2}}\arcsin xdx$  
   $= -\sqrt{1-x^2}\arcsin^2 x + \int 1dx$    
   $= -\sqrt{1-x^2}\arcsin^2 x + x + C$
   $\int\arcsin^2 xdx$  
   $= x\arcsin^2 x + 2\sqrt{1-x^2}\arcsin^2 x-2x + C$
#### Applications
11. Finding arc length Find the length of the curve
    $$
    y = \int_0^x\sqrt{cos 2t}dt, 0 \le x \le \dfrac{\pi}{4}
    $$  
    $\dfrac{dy}{dt} = \sqrt{cos 2x}$  
    $l = \int_0^{\frac{\pi}{4}}\sqrt{1+\cos 2x}dx$   
    $= \int_0^{\frac{\pi}{4}}\sqrt{2\cos^2x}dx$  
    $= \sqrt{2}[\sin x]_0^{\frac{\pi}{4}}$  
    $= 1$
#### The Substitution $z = \tan \dfrac{x}{2}$
The substitution
$$
z = \tan \dfrac{x}{2}
$$
reduces the problem of integrating a rational expression in $\sin x$ and $\cos x$ to a problem of integrating a rational function of $z$. This in turn can be integrated by partial fractions.   
From the accompanying figure
![](../images/Thomas%20Calculus/8-3.jpg)  
we can read the relation
$$
\tan \dfrac{x}{2} = \dfrac{\sin x}{1 + \cos x}
$$
To see the effect of the substitution, we calculate
$$
\cos x = \dfrac{1-z^2}{1+z^2}
$$
and 
$$
\sin x = \dfrac{2z}{1+z^2}
$$
Finally, $x = 2 \arctan z,$ so
$$
dx = \dfrac{2dz}{1+z^2}
$$
Use the substitutions in Equations (1)–(4) to evaluate the integrals in Exercises 33–40. Integrals like these arise in calculating the average angular velocity of the output shaft of a universal joint when the input and output shafts are not aligned.

33. $\int\dfrac{dx}{1-\sin x}$  
    Let $z = \tan \dfrac{x}{2},\sin x = \dfrac{2z}{1+z^2},dx = \dfrac{2dz}{1+z^2}$  
    $\int\dfrac{dx}{1-\sin x}$  
    $= \int\dfrac{1}{1-\frac{2z}{1+z^2}}\dfrac{2dz}{1+z^2}$  
    $= \int\dfrac{1+z^2}{(1-z)^2}\dfrac{2dz}{1+z^2}$  
    $= \int\dfrac{2dz}{(1-z)^2}$  
    $= \dfrac{2}{1-z}$  
    $= \dfrac{2}{1-\tan\frac{x}{2}}$
#### The Gamma Function and Stirling’s Formula
Euler’s gamma function $\Gamma(x)$ (“gamma of x”; $\Gamma$ is a Greek capital g) uses an integral to extend the factorial function from the nonnegative integers to other real values. The formula is 
$$
\Gamma(x) = \int_0^{\infty}t^{x-1}e^{-t}dt, x>0
$$
For each positive $x$, the number $\Gamma(x)$ is the integral of $t^{x-1}e^{-t}dt$ with respect to $t$ from 0 to $\infty$. Figure 8.28 shows the graph of $\Gamma$ near the origin. You will see how to calculate $Γ(\dfrac{1}{2})$ if you do Additional Exercise 23 in Chapter 15.  
![](../images/Thomas%20Calculus/8-4.jpg)  

43. if $n$ is a nonnegative integer, $\Gamma(n + 1) = n!$  
    a. Show that $\Gamma(1) = 1$  
    b. Then apply integration by parts to the integral for $\Gamma(n + 1)$to show that $\Gamma(x + 1) = x\Gamma(x)$. This gives
    $$
    \Gamma(2) = 1\Gamma(1) = 1 \\
    \Gamma(3) = 2\Gamma(2) = 2 \\
    \Gamma(4) = 3\Gamma(3) = 6 \\
    \cdots \\
    \Gamma(n+1) = n\Gamma(n) = n!
    $$
    c. Use mathematical induction to verify Equation (5) for every nonnegative integer $n$.  
    $\Gamma(1) = \int_0^{\infty}t^0e^{-t}dt$  
    $= \int_0^{\infty}\dfrac{1}{e^t}dt$  
    $= \lim\limits_{b\to\infty}(-\dfrac{1}{e^b} + 1) = 1$  
    b. $\Gamma(x + 1) = \int_0^{\infty}t^{x}e^{-t}dt$  
    Let $u(t) = t^{x},v'(t) = e^{-t}$  
    $u'(t) = xt^{x-1}, v(t) = -e^{-t}$  
    $\Gamma(x + 1) = [-t^{x}e^{-t}]_0^{\infty}+ x\int_0^{\infty} t^{x-1}e^{-t}dt$  
    $= \lim\limits_{b\to\infty}-\dfrac{b^x}{e^b} + x\Gamma(x)$  
    $= x\Gamma(x)$  
    c. For $n = 1, \Gamma(1) = 1!$  
    Suppose for $n = k,k \ge 2,\Gamma(k) = (k-1)!$  
    For $n = k+1, \Gamma(k +1) = k\Gamma(k) = k!$  
    For $n \ge 1, \Gamma(n+1) = n!$