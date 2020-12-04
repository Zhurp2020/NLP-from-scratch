# Thomas Calculus
## Chapter 5 Integrals
### 5.1 Area and Estimating with Finite Sums
#### Area
#### Distance Traveled
#### Displacement Versus Distance Traveled
#### Average Value of a Nonnegative Continuous Function
#### Summary
### 5.2 Sigma Notation and Limits of Finite Sums
#### Finite Sums and Sigma Notation
$$
\sum_{k = 1}^na_k = a_1 + a_2 + a_3 + \cdots + a_n
$$
>Algebra Rules for Finite Sums
>1. Sum Rule: 
>$$
>\sum_{k = 1}^n(a_k + b_k) = \sum_{k = 1}^na_k + \sum_{k = 1}^nb_k
>$$
>2. Difference Rule:
>$$
>\sum_{k = 1}^n(a_k - b_k) = \sum_{k = 1}^na_k - \sum_{k = 1}^nb_k
>$$
>3. Constant Multiple Rule:
>$$
>\sum_{k = 1}^nca_k= c\sum_{k = 1}^na_k
>$$
>4. Constant Value Rule:
>$$
>\sum_{k = 1}^nc= nc
>$$

>The first $n$ squares:  
>$$
>\sum_{k = 1}^nk^2= \dfrac{n(n + 1)(2n + 1)}{6}
>$$  
>The first $n$ cubes
>$$
>\sum_{k = 1}^nk^3= (\dfrac{n(n + 1)}{2})^2
>$$ 
#### Limits of Finite Sums
#### Riemann Sums
We begin with an arbitrary bounded function $f$ defined on a closed interval $[a, b]$. We choose $n - 1$ points $\{x_1,x_2,x_3,\cdots,x_{n-1}\}$ between $a$ and $b$ that are in increasing order, so that
$$
a = x_0 < x_1 < x_2 < \cdots < x_{n-1} < x_n = b
$$
The set of all of these points,
$$
P = \{x_0,x_1,x_2,x_3,\cdots,x_{n-1},x_n\}
$$
is called a partition of $[a, b]$. If all $n$ subintervals have equal width, then their common width $\Delta x$ is equal to $\dfrac{b - a}{n}$. In the $k$th subinterval $[x_{k-1}, x_k]$ we select some point $c_k$. Then on each subinterval we stand a vertical rectangle that stretches from the $x$-axis to touch the curve at $(c_k, f(c_k))$. On each subinterval we form the product $f(c_k)\cdot \Delta x_k$. Finally we sum all these products to get
$$
S_P = \sum_{k = 1}^nf(c_k)\Delta x_k
$$
The sum $S_P$ is called a Riemann sum for $f$ on the interval $[a, b]$. We define the norm of a partition $P$, written $||P||$ , to be the largest
of all the subinterval widths.
### 5.3 The Definite Integral
#### Definition of the Definite Integral
>**DEFINITION**   
>Let $f(x)$ be a function defined on a closed interval $[a, b]$. We say that a number $J$ is the definite integral of $f$ over $[a, b]$ and that $J$ is the limit of the Riemann sums $\sum\limits_{k = 1}^nf(c_k)\Delta x_k$ if the following condition is satisfied:  
Given any number $\varepsilon > 0$ there is a corresponding number $\delta > 0$ such that for every partition $P = \{x_0,x_1,x_2,x_3,\cdots,x_{n-1},x_n\}$ of $[a, b]$ with $||P|| < \delta$ and any choice of $c_k$ in $[x_{k-1}, x_k]$, we have
>$$
>|\sum_{k = 1}^nf(c_k)\Delta x_k - J|< \varepsilon
>$$

>A Formula for the Riemann Sum with Equal-Width Subintervals
>$$
>\int_a^b f(x)dx = \lim_{n\to\infty}\sum_{k = 1}^n(a + k\dfrac{b - a}{n})(\dfrac{b - a}{n})
>$$
#### Integrable and Nonintegrable Functions
>**THEOREM 1—Integrability of Continuous Functions**  
If a function $f$ is continuous over the interval $[a, b]$ , or if $f$ has at most finitely
many jump discontinuities there, then the definite integral $\int_a^bf(x)dx$ exists and $f$
is integrable over $[a, b]$.
#### Properties of Definite Integrals
>**THEOREM 2**   
When $f$ and $g$ are integrable over the interval $[a, b]$ , the definite integral satisfies these rules .
> 1. Order of Integration: 
>$$
>\int_a^b f(x)dx =-\int_b^a f(x)dx
>$$
>2. Zero Width Interval: 
>$$
>\int_a^a f(x)dx =0
>$$
>3. Constant Multiple: 
>$$
>\int_a^a kf(x)dx =k\int_a^a f(x)dx
>$$
>4. Sum and Difference: 
>$$
>\int_a^b (f(x)\plusmn g(x))dx =\int_a^b f(x)dx + \int_a^b g(x)dx
>$$
>5. Additivity: 
>$$
>\int_a^b f(x)dx+ \int_b^c f(x)dx=\int_a^c f(x)dx
>$$
>6. Max-Min Inequality:   
If $f$ has maximum value max $f$ and minimum value min $f$ on $[a, b]$ , then
>$$
>(\min f)(b - a) \le \int_a^b f(x)dx\le (\max f)(b - a)
>$$
>7. Domination:   
If $f(x) \ge g(x)$ on $[a, b]$ then $\int_a^b f(x)dx \ge \int_a^b g(x)dx$   
If $f(x) \ge 0$ on $[a, b]$ then $\int_a^b f(x)dx \ge0$  
#### Area Under the Graph of a Nonnegative Function
>**DEFINITION**   
If $y = f(x)$ is nonnegative and integrable over a closed interval $[a, b]$, then the area under the curve $y = f(x)$ over $[a, b]$  is the integral of $f$ from $a$ to $b$,
>$$
>A = \int_a^b f(x)dx
>$$

>$$
>\int_a^b xdx = \dfrac{b^2}{2} - \dfrac{a^2}{2} \\
>\int_a^b cdx = c(b - a) \\
>\int_a^b x^2dx = \dfrac{b^3}{2} - \dfrac{a^3}{2} \\
>$$
Proof:  
For a partition $P = \{0,\dfrac{b}{n},\dfrac{2b}{n},\cdots,\dfrac{nb}{n}\}$ and $c_k=\dfrac{kb}{n}$:
$$
\sum_{k = 1}^nf(c_k)\Delta x = \sum_{k = 1}^n\dfrac{kb}{n}\dfrac{b}{n}\\
=\dfrac{b^2}{n^2}\sum_{k = 1}^nk \\
=\dfrac{b^2}{n^2}\dfrac{n(n+1)}{2} \\
= \dfrac{b^2n^2 + 1}{2n^2} \\
= \dfrac{b^2}{2} + \dfrac{1}{2n^2}
$$
As $n\to\infty$ and $||P||\to0$, 
$$
\int_0^b xdx = \dfrac{b^2}{2}\\
\int_a^b xdx = \int_a^0 xdx + \int_0^b xdx \\
= \dfrac{b^2}{2} - \dfrac{a^2}{2}
$$
#### Average Value of a Continuous Function Revisited
>DEFINITION   
If $f$ is integrable on $[a, b]$ , then its average value on $[a, b]$, which is also called its mean, is
>$$
>av(f) = \dfrac{1}{b - a}\int_a^b f(x)dx
>$$
### 5.4 The Fundamental Theorem of Calculus
#### Mean Value Theorem for Definite Integrals
>THEOREM 3—**The Mean Value Theorem for Definite Integrals**  
If $f$ is continuous on $[a, b]$ , then at some point $c$ in $[a, b]$,
>$$
>f(c) =\dfrac{1}{b - a}\int_a^b f(x)dx
>$$
Proof:  
$$
(\min f)(b - a) \le \int_a^b f(x)dx\le (\max f)(b - a) \\
(\min f) \le \dfrac{1}{b - a}\int_a^b f(x)dx\le (\max f) 
$$  
$f$ is continuous, the Intermediate Value Theorem for Continuous Functions gives the Theorem.
#### Fundamental Theorem, Part 1
>THEOREM 4—The Fundamental Theorem of Calculus, Part 1  
If $f$ is continuous on $[a, b]$, then $F(x) = \int_a^xf(t) dt$ is continuous on $[a, b]$ and differentiable on $(a, b)$ and its derivative is $f(x)$:
>$$
>F'(x) = \dfrac{d}{dx}\int_a^xf(t) dt = f(x)
>$$
Proof:  
$$
F'(x) = \lim_{h\to0}\dfrac{F(x + h) - F(x)}{h} \\
= \lim_{h\to0}\dfrac{\int_a^{x+h}f(t) dt - \int_a^xf(t) dt}{h} \\
= \lim_{h\to0}\dfrac{1}{h}\int_x^{x+h}f(t) dt
$$
The The Mean Value Theorem for Definite Integrals gives that there exists a $c\in[x,x+h]$ such that
$$
f(c) = \dfrac{1}{h}\int_x^{x+h}f(t) dt \\
$$
When $h\to0,x + h \to x, c\to x,f(c)\to f(x)$
$$
F'(x) = \lim_{h\to0}\dfrac{1}{h}\int_x^{x+h}f(t) dt \\
= \lim_{h\to0}f(c) \\
= f(x)
$$
#### Fundamental Theorem, Part 2 (The Evaluation Theorem)
>THEOREM 4 (Continued)—The Fundamental Theorem of Calculus, Part 2   
If $f$ is continuous over $[a, b]$ and $F$ is any antiderivative of $f$ on $[a, b]$ , then
>$$
>\int_a^bf(x) dx = F(b) - F(a) 
>$$
Proof:  
If $G$ is an antiderivative of $f$:
$$
G(x) = \int_a^xf(t) dt \\
F(x) = G(x) + C \\
F(b) - F(a) = G(b) - G(a) \\
= \int_a^bf(t) dt - \int_a^af(t) dt \\
= \int_a^xf(t) dt
$$
#### The Integral of a Rate
>**THEOREM 5—The Net Change Theorem**  
The net change in a differentiable function $F(x)$ over an interval $a \le x \le b$is the integral of its rate of change:
>$$
>F(b) - F(a) = \int_a^bF'(x) dx 
>$$
#### The Relationship Between Integration and Differentiation
#### Total Area
### 5.5 Indefinite Integrals and the Substitution Method
The indefinite integral of the function $f$ with respect to $x$ is the set of all antiderivatives of $f$
$$
\int f(x)d(x) = F(x) + c
$$
#### Substitution: Running the Chain Rule Backwards
>**THEOREM 6—The Substitution Rule**  
If $u = g(x)$ is a differentiable function whose range is an interval $I$, and $f$ is continuous on $I$, then  
>$$
>\int f(g(x))g'(x)dx = \int f(u)du 
>$$
Proof:  
If $F$ is an antiderivative of $f$, the chain rule gives:
$$
\dfrac{d}{dx}F(g(x)) =F'(g(x))g'(x) \\ 
= f(g(x))g'(x)
$$  
Let $u = g(x)$
$$
\int f(g(x))g'(x)dx = \int \dfrac{d}{dx}F(u)dx \\
= F(u) + C \\
= \int f(u)du
$$
#### Trying Different Substitutions
### 5.6 Definite Integral Substitutions and the Area Between Curves
#### The Substitution Formula
>**THEOREM 7—Substitution in Definite Integrals**  
If $g′$'is continuous on the interval $[a, b]$ and $f$ is continuous on the range of $g(x) = u$, then
>$$
>\int_a^b f(g(x))g'(x)dx = \int_{g(a)}^{g(b)} f(u)du 
>$$
#### Definite Integrals of Symmetric Functions
>**THEOREM 8**  
Let $f$ be continuous on the symmetric interval $[-a, a]$.   
(a) If $f$ is even, then $\int_{-a}^a f(x)dx = 2\int_0^a f(x)dx$  
(b) If $f$ is odd, then $\int_{-a}^a f(x)dx = 0$ 

Proof:   
$$
\int_{-a}^a f(x)dx = \int_{-a}^0 f(x)dx + \int_0^a f(x)dx \\
= -\int_0^{-a} f(x)dx + \int_0^a f(x)dx
$$
Let $g(x) = u = -x, g'(x) = \dfrac{du}{dx} = -1,g(0) = 0, g(-a) = a$
$$
\int_{-a}^a f(x)dx = \int_0^{-a} f(-g(x))g'(x)dx + \int_0^a f(x)dx \\
= \int_0^{-a} f(g(x))g'(x)dx + \int_0^a f(x)dx \\
= \int_0^a f(u)du + \int_0^a f(x)dx \\
= 2\int_0^a f(x)dx
$$
#### Areas Between Curves
>**DEFINITION**    
If $f$ and $g$ are continuous with $f(x) \ge g(x)$ throughout $[a, b]$, then the area of the region between the curves $y = f(x)$ and $y = g(x)$ from
$a$ to $b$ is the integral of $(f - g)$ from $a$ to $b$:
>$$
>A = \int_a^b [f(x)-g(x)]dx
>$$
#### Integration with Respect to $y$