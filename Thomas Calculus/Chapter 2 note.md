# Thomas Calculus
## Chapter 2 Limits and Continuity
### 2.1 Rates of Change and Tangent Lines to Curves
#### Average and Instantaneous Speed
> **Average Speed**  
> When $f(t)$ measures the distance traveled at time $t$,  
> Average speed over $[t_1,t_2]$  
> $$
> = \dfrac{f(t_2) - f(t_1)}{t_2 - t_1}
>$$
#### Average Rates of Change and Secant Lines
>**DEFINITION** The average rate of change of $y = f(x)$ with respect to $x$ over the interval $[x_1,x_2]$ is
>$$
>\dfrac{\Delta y}{\Delta x} = \dfrac{f(x_2) - f(x_1)}{x_2 - x_1} = \dfrac{f(x_1 + h) - ƒ(x_1)}{h}, h \ne 0
>$$   
![](../images/Thomas%20Calculus/2-1.jpg)
#### Defining the Slope of a Curve
![](../images/Thomas%20Calculus/2-2.jpg)
#### Rates of Change and Tangent Lines
### 2.2 Limit of a Function and Limit Laws
#### Limits of Function Values
#### An Informal Description of the Limit of a Function 
Suppose that $f(x)$ is defined on an open interval about $c$, except possibly at $c$ itself. If $f(x)$ is arbitrarily close to the number $L$ for all $x$ sufficiently close to $c$, other than $c$ itself, then we say that $f$ approaches the limit $L$ as $x$, approaches $c$
$$
\lim_{x\to c}f(x) = L
$$
#### The Limit Laws
>**THEOREM 1—Limit Laws**  
>If $L$, $M$, $c$, and $k$ are real numbers and $\lim\limits_{x\to c}f(x) = L$ and $\lim\limits_{x\to c}g(x) = M$, then
>1. Sum Rule: 
>  $$
>  \lim_{x\to c}(f(x) + g(x))= L + M
>  $$
>2. Diference Rule: 
>  $$
>  \lim_{x\to c}(f(x) - g(x))= L - M
>  $$
>3. Constant Multiple Rule: 
>  $$
>  \lim_{x\to c}(kf(x))= kL 
>  $$
>4. Product Rule: lim
>  $$
>  \lim_{x\to c}(f(x)g(x))= L \cdot M
>  $$
>5. Quotient Rule: lim
>  $$
>  \lim_{x\to c}\dfrac{f(x)}{g(x)}= \dfrac{L}{M}, M \ne 0
>  $$
>6. Power Rule: 
>  $$
>  \lim_{x\to c}[f(x)]^n = L^n
>  $$
>7. Root Rule: 
>  $$
>  \lim_{x\to c}\sqrt[n]{f(x)}= \sqrt[n]{L} = L^{\frac{1}{n}}
>  $$ 
> , $n$ a positive integer  
(If $n$ is even, we assume that $f(x) \ge 0$ for $x$ in an interval containing $c$.)
#### Evaluating Limits of Polynomials and Rational Functions
>**THEOREM 2—Limits of Polynomials**  
>If $P(x) = a_nx^n + a_{n-1}x^n-1 + \cdots + a_0$, then
>  $$
>  \lim_{x\to c}P(x)= a_nc^n + a_{n-1}x^c-1 + \cdots + a_0
>  $$ 

>**THEOREM 3—Limits of Rational Functions**
>If $P(x)$ and $Q(x)$ are polynomials and $Q(c) \ne 0$, then
>  $$
>  \lim_{x\to c}\dfrac{P(x)}{Q(x)} = \dfrac{P(c)}{Q(c)}
>  $$ 
#### Eliminating Common Factors from Zero Denominators
#### Using Calculators and Computers to Estimate Limits
#### The Sandwich Theorem
>**THEOREM 4—The Sandwich Theorem**  
>Suppose that $g(x) \le f(x) \le h(x)$ for all $x$ in some open interval containing $c$, except possibly at $x = c$ itself. Suppose also that $\lim\limits_{x\to c}g(x) = \lim\limits_{x\to c}h(x) = L$,Then
>$$
>\lim\limits_{x\to c}f(x) = L
>$$
![](../images/Thomas%20Calculus/2-3.jpg)
