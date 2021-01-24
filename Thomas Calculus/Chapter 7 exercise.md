# Thomas Calculus
## Chapter 7 Transcendental Functions
### 7.1 Inverse Functions and Their Derivatives
#### Identifying One-to-One Functions Graphically
Which of the functions graphed in Exercises 1–6 are one-to-one, and which are not?
1. ![](../images/Thomas%20Calculus/7-5.jpg)   
   One to one
#### Graphing Inverse Functions
Each of Exercises 11–16 shows the graph of a function $y = f(x).$ Copy the graph and draw in the line $y = x$. Then use symmetry with respect to the line $y = x$ to add the graph of $f^{-1}$ to your sketch. (It is not necessary to find a formula for $f^{-1}$) Identify the domain and range of $f^{-1}$

11. ![](../images/Thomas%20Calculus/7-6.jpg)
    D: $(0,1]$R:$[0,\infty)$
#### Formulas for Inverse Functions
Each of Exercises 19–24 gives a formula for a function $y = f(x)$ and shows the graphs of $f$ and $f^{-1}$ . Find a formula for $f^{-1}$ in each case.

19. $f(x) = x^2 + 1, x \ge 0$  
    ![](../images/Thomas%20Calculus/7-7.jpg)   
    $x^2 = y - 1$  
    $x\ge 0, x = \sqrt{y - 1}$  
    $f^{-1}(x) = \sqrt{x - 1}, x\ge 1$
#### Derivatives of Inverse Functions
Each of Exercises 25–34 gives a formula for a function $y = f(x)$. In each case, find $f^{-1}(x)$ and identify the domain and range of $f^{-1}$. As a check, show that $f(f^{-1}(x)) = f^{-1}(f(x)) = x$

25. $f(x) = x^5$  
    $f^{-1}(x) = \sqrt[5]{x}$  
    $f(f^{-1}(x)) = (\sqrt[5]{x})^5 = x$  
    $f^{-1}(f(x)) = \sqrt[5]{x^5}= x$
#### Inverses of Lines
45. a. Find the inverse of the function $f(x) = mx$, where $m$ is a constant different from zero.  
b. What can you conclude about the inverse of a function $y = f(x)$ whose graph is a line through the origin with a nonzero slope $m$?  
a. $f^{-1}(x) = \dfrac{1}{m}x$
#### Increasing and Decreasing Functions
49. Show that increasing functions and decreasing functions are one-to-one. That is, show that for any $x_1$ and $x_2$ in $I, x_2 \le x_1$ implies $f(x_2) \ne f(x_1).$  
    If for some $x_1$ and $x_2$ in $I, x_2 \le x_1$ implies $f(x_2) = f(x_1),$ the function is neither decreasing nor increasing in $I$
#### Theory and Applications
55. If $f(x)$ is one-to-one, can anything be said about $g(x) = -f(x)$? Is it also one-to-one? Give reasons for your answer
    It is also one-to-one
#### COMPUTER EXPLORATIONS
In Exercises 61–66, you will explore some functions and their inverses together with their derivatives and linear approximating functions at specified points. Perform the following steps using your CAS:  
a. Plot the function $y = f(x)$  together with its derivative over the given interval. Explain why you know that $f$ is one-to-one over the interval.   
b. Solve the equation $y = f(x)$ for $x$ as a function of $y$, and name the resulting inverse function $g$.  
c. Find the equation for the tangent line to $f$ at the specified point $(x0, f(x_0)).$  
d. Find the equation for the tangent line to $g$ at the point $(f(x_0), x_0)$ located symmetrically across the 45° line $y = x$ (which is the graph of the identity function). Use Theorem 1 to find the slope of this tangent line.  
e. Plot the functions $f$ and $g$, the identity, the two tangent lines, and the line segment joining the points $(x0, f(x_0)).$ and $(f(x_0), x_0)$ Discuss the symmetries you see across the main diagonal.

61. $y = \sqrt{3x - 2},\dfrac{2}{3} \le x \le 4, x_0 = 3$  
    a. $\dfrac{dy}{dx} = \dfrac{1}{2\sqrt{3x-2}}\cdot3 = \dfrac{3}{2\sqrt{3x-2}}$  
    b. $3x - 2=y^2$  
    $x = \dfrac{y^2+2}{3}$  
    $g(x) = \dfrac{x^2+2}{3}$  
    c. $f(3) = \sqrt{7}$   
    $f'(3) = \dfrac{3}{2\sqrt{7}} = \dfrac{3}{14}\sqrt{7}$  
    $y = \dfrac{3}{14}\sqrt{7}x+\dfrac{5}{14}\sqrt{7}$  
    d. $g'(\sqrt{7}) = \dfrac{1}{f'(g(\sqrt{7}))} = \dfrac{2}{3}\sqrt{7}$   
    $y = \dfrac{2}{3}\sqrt{7}x-\dfrac{5}{3}$
### 7.2 Natural Logarithms
#### Using the Algebraic Properties—Theorem 2
1. Express the following logarithms in terms of $\ln 2$ and $\ln 3$.  
a. $\ln 0.75$ b. $\ln \dfrac{4}{9}$ c. $\ln \dfrac{1}{2}$  
d. $\ln \sqrt[3]{9}$ e. $\ln 3\sqrt{2}$ f. $\ln \sqrt{13.5}$   
a. $\ln 0.75 = \ln \dfrac{3}{4} = \ln 3 - \ln 2^2 = \ln 3 - 2\ln2$  
b. $\ln \dfrac{4}{9} = 2\ln 2 - 2\ln 3$  
c. $\ln \dfrac{1}{2} = \ln1 - \ln 2 = -\ln 2$  
d. $\ln \sqrt[3]{9} = \ln 3^{\frac{2}{3}} = \dfrac{2}{3}\ln 3$  
e. $\ln 3\sqrt{2} = \ln3 + \dfrac{1}{2}\ln 2$  
f. $\ln \sqrt{13.5} = \ln (\dfrac{27}{2})^{\frac{1}{2}} = \dfrac{1}{2}(3\ln 3 - \ln 2)$  
#### Finding Derivatives
In Exercises 7–38, find the derivative of $y$ with respect to $x, t,$ or $\theta$, as appropriate.

7. $y = \ln 3x$  
   $\dfrac{dy}{dx} = \dfrac{3}{3x} = \dfrac{1}{x}$  
#### Evaluating Integrals
Evaluate the integrals in Exercises 39–56.

39. $\int_{-3}^{-2}\dfrac{dx}{x}$  
    $\int_{-3}^{-2}\dfrac{dx}{x} = -[\ln x]_2^3 = -\ln \dfrac{3}{2}$
#### Logarithmic Differentiation
In Exercises 57–70, use logarithmic differentiation to find the derivative of $y$ with respect to the given independent variable.

57. $y = \sqrt{x(x + 1)}$  
    $\ln y = \ln \sqrt{x(x + 1)}$  
    $\dfrac{d}{dx}\ln y = \dfrac{d}{dx} \ln \sqrt{x(x + 1)}$  
    $\dfrac{1}{y}\dfrac{dy}{dx}= \dfrac{d}{dx} \dfrac{1}{2}\ln (x^2+x)$  
    $\dfrac{dy}{dx} = \dfrac{y}{2}\dfrac{1}{x^2 + x}(2x+1)$  
    $= \dfrac{\sqrt{x(x + 1)}(2x+1)}{2x^2+2x}$
#### Theory and Applications
71. Locate and identify the absolute extreme values of  
a. $\ln (\cos x)$ on $[-\dfrac{\pi}{4},\dfrac{\pi}{3}]$,  
b. $\cos (\ln x)$ on $[\dfrac{1}{2},2]$.  
a. $\dfrac{d}{dx}\ln (\cos x) = -\dfrac{\sin x}{\cos x} = 0$  
$\sin x = 0, x = 0$  
$f(0) = \ln 1 = 0$  
$f(-\dfrac{\pi}{4}) = \ln \dfrac{\sqrt{2}}{2} = -\dfrac{1}{2}\ln 2$  
$f(\dfrac{\pi}{3}) = \ln \dfrac{1}{2} = -\ln 2$  
$f(x)_{\max} = f(0) = 0$  
$f(x)_{\min} = f(\dfrac{\pi}{3}) = -\ln 2$   
b. $\dfrac{d}{dx} \cos (\ln x) = -\dfrac{\sin\ln x}{x} = 0$  
$\sin\ln x = 0, \ln x =0, x = 1$  
$f(1) = \cos 0 = 1$  
$f(\dfrac{1}{2}) =\cos\ln \dfrac{1}{2} = -\ln 2$  
$f(2) = \cos\ln 2$  
$f(x)_{\max} = f(1) = 1$  
$f(x)_{\min} = f(\dfrac{1}{2}) = f(2) = \cos\ln 2$ 
#### Identifying Extrema
In Exercises 75 and 76:  
a. Find the open intervals on which the function is increasing and decreasing.  
b. Identify the function’s local and absolute extreme values, if any, saying where they occur.  

75. $g(x) = x (\ln x)^2$  
    D:$x > 0$   
    $\dfrac{dg}{dx} = x\dfrac{d}{dx}(\ln x)^2 + (\ln x)^2$  
    $= \dfrac{2x\ln x}{x} + (\ln x)^2 = 0$  
    $\ln x = 0$ or $\ln x = -2$  
    $x = 1$ or $x = \dfrac{1}{e^2}$  
    $\dfrac{1}{e^2}< x < 1, -2 < \ln x <0, \dfrac{dg}{dx} < 0, g$ is decreasing  
    $0 < x < \dfrac{1}{e^2}$ or $x > 1, \ln x < -2$ or $\ln x > 0, \dfrac{dg}{dx}> 0, g$ is increasing  
    $g(1) = 0, g(\dfrac{1}{e^2}) = \dfrac{4}{e^2}$  
    $g(x)_{\min} = g(1) = 0$  
    local maxima: $g(\dfrac{1}{e^2})= \dfrac{4}{e^2}$
### 7.3 Exponential Functions
#### Solving Exponential Equations
In Exercises 1–4, solve for $t$.
1. a. $e^{-0.3t} = 27$ b. $e^{kt} =\dfrac{1}{2}$ c. $e^{\ln 0.2 t} =0.4$  
   a. $-0.3t = \ln 27$  
   $t = - \dfrac{10}{3}\ln 27$  
   b. $kt = \ln \dfrac{1}{2}$  
   $t = -\dfrac{1}{k}\ln 2$  
   c. $\ln 0.2t = \ln 0.4$  
   $0.2t =  0.4$  
   $t = 2$  
#### Finding Derivatives
In Exercises 7–26, find the derivative of $y$ with respect to $x, t$, or $\theta$, as appropriate.

7. $y = e^{-5x}$  
   $\dfrac{dy}{dx} = -5e^{-5x}$
#### Finding Integrals
Evaluate the integrals in Exercises 33–54.

33. $\int(e^{3x} + 5e^{-x}) dx$  
    $\int(e^{3x} + 5e^{-x}) dx = \dfrac{1}{3}e^{3x}-5e^{-x} + C$
#### Initial Value Problems
Solve the initial value problems in Exercises 55–58.

55. $\dfrac{dy}{dt} = e^t\sin (e^t - 2), y(\ln 2) = 0$  
    $\int e^t\sin (e^t - 2)dx$  
    Let $e^t - 2 = u, \dfrac{du}{dx} = e^t$  
    $\int e^t\sin (e^t - 2)dx = \int\sin udu$  
    $= -\cos u + C$  
    $y = -\cos(e^t-2) + C$  
    $y(\ln 2) = -\cos 0 + C = 0, C = 1$  
    $y = -\cos(e^t-2) + 1$  
#### Differentiation
In Exercises 59–86, find the derivative of y with respect to the given independent variable.

59. $y = 2^x$  
    $\dfrac{dy}{dx} = e^{x\ln 2}$  
    $= \ln 2 e^{x\ln 2}$
#### Integration
Evaluate the integrals in Exercises 87–96.

87. $\int 5^xdx$  
    $\int 5^xdx = \int e^{x\ln 5}dx$  
    $= \dfrac{1}{\ln 5}e^{x\ln 5} + C$
#### Logarithmic Differentiation
In Exercises 115–122, use logarithmic differentiation to find the derivative of $y$ with respect to the given independent variable.

115. $y = (x + 1)^x$  
     $\ln y = \ln (x + 1)^x = x\ln(x+1)$  
     $\dfrac{1}{y}\dfrac{dy}{dx} = x\dfrac{1}{x+1} + \ln(x+1)$  
     $\dfrac{dy}{dx} = \dfrac{x}{x+1}(x+1)^x+\ln(x+1)\ln (x + 1)^x$  
     $= x(x+1)^{x-1}+x\ln^2(x+1)$
#### Theory and Applications
129. Find the absolute maximum and minimum values of $f(x) =e^x - 2x$ on $[0, 1]$  
     $f'(x) = e^x-2 = 0$  
     $x = \ln 2$  
     $f(\ln 2) = 2-2\ln 2$  
     $f(1) = e-2, f(0) = 1$  
     $f(x)_{\max} = f(0) = 1$  
     $f(x)_{\min} = f(\ln 2) = 2-2\ln 2$
### 7.4 Exponential Change and Separable Differential Equations
#### Verifying Solutions
In Exercises 1–4, show that each function $y = f(x)$ is a solution of the accompanying differential equation.

1. $2y' + 3y = e^{-x}$  
a. $y = e^{-x}$ b. $y = e^{-x}+ e^{-\frac{3}{2}x}$  
c. $y = e^{-x} + Ce^{-\frac{3}{2}x}$  
    a.  $y' = -e^{-x}$  
    $2y' + 3y = e^{-x}$  
    b. $y' = -e^{-x} - \dfrac{3}{2}e^{-\frac{3}{2}x}$  
    $2y' + 3y = -2e^{-x} - 3e^{-\frac{3}{2}x} + 3e^{-x} + 3e^{-\frac{3}{2}x} = e^{-x}$  
    c. $y' = -e^{-x} - \dfrac{3}{2}Ce^{-\frac{3}{2}x}$  
    $2y' + 3y = -2e^{-x} - 3Ce^{-\frac{3}{2}x} + 3e^{-x} + 3Ce^{-\frac{3}{2}x} = e^{-x}$
#### Initial Value Problems
In Exercises 5–8, show that each function is a solution of the given initial value problem.

|Differential equation|initial equation|solution candidate|
|:-:|:-:|:-:|
|5. $y' + y = \dfrac{2}{1+4e^{2x}}$|$y(-\ln 2) = \dfrac{\pi}{2}$|$y = e^{-x}\tan^{-1}(2e^{x})$|
$y(-\ln 2) = 2\tan^{-1}1 = \dfrac{\pi}{2}$  
$y' = -e^{-x}\tan^{-1}(2e^{x}) + e^{-x}\dfrac{1}{\sec^2(\tan^{-1}(2e^{x}))}2e^{x}$  
$= -e^{-x}\tan^{-1}(2e^{x}) + 2\cos^2(\tan^{-1}(2e^{x}))$  
$y' + y = -e^{-x}\tan^{-1}(2e^{x}) + 2\cos^2(\tan^{-1}(2e^{x}))+ e^{-x}\tan^{-1}(2e^{x})$  
$= \dfrac{2}{1+4e^{2x}}$
#### Separable Differential Equations
Solve the differential equations in Exercises 9–22.

9. $2\sqrt{xy}\dfrac{dy}{dx}= 1, x, y > 0$  
    $\dfrac{dy}{dx} = \dfrac{1}{2\sqrt{x}}\dfrac{1}{\sqrt{y}}$  
    $\dfrac{1}{\sqrt{y}}dy = \dfrac{1}{2\sqrt{x}}dx$  
    $\int\dfrac{1}{\sqrt{y}}dy = \int\dfrac{1}{2\sqrt{x}}dx$  
    $2\sqrt{y} + C_1 = \sqrt{x} + C_2$  
    $\sqrt{y} = \dfrac{1}{2}(\sqrt{x}+C_2-C_1)$  
    $y = \dfrac{1}{4}(\sqrt{x}+C_2-C_1)^2$
#### Applications and Examples
The answers to most of the following exercises are in terms of logarithms and exponentials. A calculator can be helpful, enabling you to express the answers in decimal form.

23. Human evolution continues. The analysis of tooth shrinkage by C. Loring Brace and colleagues at the University of Michigan’s Museum of Anthropology indicates that human tooth size is continuing to decrease and that the evolutionary process has not yet come to a halt some 30,000 years ago. In northern Europeans, for example, tooth size reduction now has a rate of 1% per 1000 years.  
a. If $t$ represents time in years and $y$ represents tooth size, use the condition that $y = 0.99y_0$ when $t = 1000$ to find the value of $k$ in the equation $y = y_0e^{kt}$. Then use this value of $k$ to answer the following questions.  
b. In about how many years will human teeth be 90% of their present size?  
c. What will be our descendants’ tooth size 20,000 years from now (as a percentage of our present tooth size)?  
a. $y(1000) = y_0e^{1000k} = 0.99y_0$   
    $1000k = \ln \dfrac{99}{100}$  
    $k = \dfrac{1}{1000}\ln \dfrac{99}{100}$  
b. $y(t) = y_0e^{t\frac{1}{1000}\ln \frac{99}{100}} = 0.9y_0$  
$t\dfrac{1}{1000}\ln \dfrac{99}{100} = \ln \dfrac{9}{10}$    
$t = 1000\dfrac{\ln\frac{9}{10}}{\ln\frac{99}{100}}$   
c. $y(20000) = e^{20\ln \frac{99}{100}}y_0$
### 7.5 Indeterminate Forms and L’Hôpital’s Rule
#### Finding Limits in Two Ways
In Exercises 1–6, use l’Hôpital’s Rule to evaluate the limit. Then
evaluate the limit using a method studied in Chapter 2.
1. $\lim\limits_{x\to-2}\dfrac{x + 2}{x^2 - 4}$  
   $\dfrac{d}{dx}(x+2) = 1, \dfrac{d}{dx}(x^2 - 4 )= 2x$    
   $\lim\limits_{x\to-2}\dfrac{x + 2}{x^2 - 4} = \lim\limits_{x\to-2}\dfrac{1}{2x} = -\dfrac{1}{4}$  
   $\lim\limits_{x\to-2}\dfrac{x + 2}{x^2 - 4} = \lim\limits_{x\to-2}\dfrac{x+2}{(x+2)(x-2)} = \lim\limits_{x\to-2}\dfrac{1}{x-2}= -\dfrac{1}{4}$  
#### Applying l’Hôpital’s Rule
Use l’Hôpital’s rule to find the limits in Exercises 7–50.

7. $\lim\limits_{x\to2}\dfrac{x - 2}{x^2 - 4}$  
   $\dfrac{d}{dx}(x-2) = 1, \dfrac{d}{dx}(x^2 - 4) = 2x$ 
   $\lim\limits_{x\to2}\dfrac{x - 2}{x^2 - 4} =\lim\limits_{x\to2}\dfrac{1}{2x} = \dfrac{1}{4}$  
#### Indeterminate Powers and Products
Find the limits in Exercises 51–66.

51. $\lim\limits_{x\to1^+}x^{\frac{1}{1-x}}$  
    Let $f(x) = x^{\frac{1}{1-x}}$   
    $\ln f(x) = \ln x^{\frac{1}{1-x}} = \dfrac{1}{1-x}\ln x$  
    $\dfrac{d}{dx}\ln x = \dfrac{1}{x}$  
    $\dfrac{d}{dx}(1-x) = -1$   
    $\lim\limits_{x\to1^+}\dfrac{\ln x}{1-x} = \lim\limits_{x\to1^+}\dfrac{\frac{1}{x}}{-1} = -1$  
    $\lim\limits_{x\to1^+}x^{\frac{1}{1-x}} = e^{-1} = \dfrac{1}{e}$
#### Theory and Applications
L’Hôpital’s Rule does not help with the limits in Exercises 67–74. Try it—you just keep on cycling. Find the limits some other way.

67. $\lim\limits_{x\to\infty}\dfrac{\sqrt{9x+1}}{\sqrt{x+1}}$  
    $\lim\limits_{x\to\infty}\dfrac{\sqrt{9x+1}}{\sqrt{x+1}} = \lim\limits_{x\to\infty}\sqrt{9-\dfrac{9}{x+1}} = \sqrt{9} = 3$
### 7.6 Inverse Trigonometric Functions
#### Common Values
Use reference triangles like those in Examples 1 and 3 to find the angles in Exercises 1–8.
1. a. $\tan^{-1} 1$ b. $\arctan (-\sqrt{3})$ c. $\tan^{-1} \dfrac{1}{\sqrt{3}}$  
   a. $\tan^{-1} 1 = \dfrac{\pi}{4}$  
   b. $\arctan (-\sqrt{3} = -\dfrac{\pi}{3}$  
   c. $\tan^{-1} \dfrac{1}{\sqrt{3}} = \dfrac{\pi}{6}$ 
#### Evaluations
Find the values in Exercises 9–12.

9. $\sin(\cos^{-1}\dfrac{\sqrt{2}}{2}))$
   $\sin(\cos^{-1}\dfrac{\sqrt{2}}{2})) = \dfrac{\sqrt{2}}{2}$
#### Limits
Find the limits in Exercises 13–20. (If in doubt, look at the function’s graph.)

13. $\lim\limits_{x\to1^-}\sin^{-1}x$ 
    $\lim\limits_{x\to1^-}\sin^{-1}x = \dfrac{\pi}{2}$
#### Finding Derivatives
In Exercises 21–42, find the derivative of y with respect to the appropriate variable.

21. $y = \cos^{-1}(x^2)$  
    $\dfrac{dy}{dx} = -\dfrac{2x}{\sqrt{1-x^4}}$  
#### Evaluating Integrals
Evaluate the integrals in Exercises 47–70.

47. $\int\dfrac{dx}{\sqrt{9-x^2}}$   
    $\int\dfrac{dx}{\sqrt{9-x^2}} = \sin^{-1}\dfrac{x}{3} + C$
#### L’Hôpital’s Rule
Find the limits in Exercises 97–104.

97. $\lim\limits_{x\to0}\dfrac{\sin^{-1}5x}{x}$  
    $\dfrac{d}{dx}\sin^{-1}5x = \dfrac{5}{\sqrt{1-25x^2}}, \dfrac{d}{dx}x = 1$  
    $\lim\limits_{x\to0}\dfrac{\sin^{-1}5x}{x} = \lim\limits_{x\to0}\dfrac{\frac{5}{\sqrt{1-25x^2}}}{1} = 5$  
#### Integration Formulas
Verify the integration formulas in Exercises 105–108.

105. $\int\dfrac{\tan^{-1}xdx}{x^2} = \ln x - \dfrac{1}{2}\ln(1+x^2)-\dfrac{\tan^{-1}x}{x} + C$  
     $\dfrac{d}{dx}(\ln x - \dfrac{1}{2}\ln(1+x^2)-\dfrac{\tan^{-1}x}{x} + C)$  
     $= \dfrac{1}{x} - \dfrac{1}{2}\dfrac{1}{1+x^2}2x - \dfrac{x\frac{1}{1+x^2}- \tan^{-1}x}{x^2}$  
     $= \dfrac{1}{x} - \dfrac{x}{1+x^2}- \dfrac{\frac{1}{1+x^2}}{x} + \dfrac{\tan^{-1}x}{x^2}$  
     $= \dfrac{1+x^2-x^2-1}{x(1+x^2)} + \dfrac{\tan^{-1}x}{x^2}$  
     $= \dfrac{\tan^{-1}x}{x^2}$  
#### Initial Value Problems
Solve the initial value problems in Exercises 109–114.

109. $\dfrac{dy}{dx} = \dfrac{1}{\sqrt{1-x^2}}, y(0) = 0$  
     $\int\dfrac{1}{\sqrt{1-x^2}}dx = \sin^{-1}x + C$  
     $y(0) = C = 0$  
     $y = \sin^{-1}x$
#### Applications and Theory
113. You are sitting in a classroom next to the wall looking at the blackboard at the front of the room. The blackboard is 12 ft long and starts 3 ft from the wall you are sitting next to.   
     a. Show that your viewing angle is
     $$
     \alpha = \cot^{-1}\dfrac{x}{15} - \cot^{-1}\dfrac{x}{3}
     $$
     if you are $x$ ft from the front wall.  
     b. Find $x$ so that $\alpha$ is as large as possible.  
     a.$\alpha = \cot^{-1}\dfrac{x}{15} - \cot^{-1}\dfrac{x}{3}$  
     b.$\dfrac{d}{dx}\alpha = -\dfrac{1}{1+\frac{x^2}{225}}\dfrac{1}{15} + \dfrac{1}{1+\frac{x^2}{9}}\dfrac{1}{3}$  
     $= \dfrac{3}{x^2+9} - \dfrac{15}{225+x^2} = 0$  
     $675+3x^2 = 15x^2+135$  
     $12x^2 = 540$  
     $x = \sqrt{45} = 3\sqrt{5}$ feet