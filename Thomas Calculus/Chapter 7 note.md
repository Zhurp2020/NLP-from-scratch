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