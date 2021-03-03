# Thomas Calculus
## Chapter 13 Vector-Valued Functions and Motion in Space
### 13.1 Curves in Space and Their Tangents
#### Limits and Continuity
>**DEFINITION**    
Let $\mathbf{r}(t) = f(t)\mathbf{i} + g(t)\mathbf{j} + h(t)\mathbf{k}$ be a vector function with domain $D$, and let $L$ be a vector. We say that $\mathbf{r}$ has limit $\mathbf{L}$ as $t$ approaches $t_0$ and write  
>$$
>\lim_{t\to t_0}\mathbf{r}(t) = \mathbf{L}
>$$
>if, for every number $\varepsilon > 0$, there exists a corresponding number $\delta < 0$ such that for all $t\in D$
>$$
>|\mathbf{r}(t) - L| < \varepsilon\quad\mathsf{whenever}\quad0 < |t - t_0| < \delta
>$$

>**DEFINITION**   
A vector function $\mathbf{r}(t)$ is continuous at a point $t = t_0$ in its domain if $\lim\limits_{t\to t_0}\mathbf{r}(t) = \mathbf{r}(t_0)$. The function is continuous if it is continuous at every point in its domain.
#### Derivatives and Motion
>**DEFINITION**  
The vector function $\mathbf{r}(t) = f(t)\mathbf{i} + g(t)\mathbf{j} + h(t)\mathbf{k}$ has a derivative (is differentiable) at $t$ if $f, g,$ and $h$ have derivatives at $t$. The derivative is the vector function  
>$$
>\mathbf{r}'(t) = \dfrac{d\mathbf{r}}{dt}=\lim_{\Delta t\to 0}\dfrac{\mathbf{r}(t + \Delta t)}{\Delta t} = \dfrac{df}{dt}\mathbf{i} + \dfrac{dg}{dt}\mathbf{j} + \dfrac{dh}{dt}\mathbf{k}
>$$
#### Differentiation Rules
#### Vector Functions of Constant Length
### 13.2 Integrals of Vector Functions; Projectile Motion
#### Integrals of Vector Functions
>**DEFINITION**   
The indefinite integral of $\mathbf{R}$ with respect to $t$ is the set of all antiderivatives of $\mathbf{r}$, denoted by $\int \mathbf{r}(t) dt$. If $\mathbf{R}$ is any antiderivative of $\mathbf{R}$, then
>$$
>\int \mathbf{r}(t)dt = \mathbf{R}(t) + \mathbf{C}
>$$

>**DEFINITION**   
If the components of $\mathbf{r}(t) = f(t)\mathbf{i} + g(t)\mathbf{j} + h(t)\mathbf{k}$ are integrable
over $[a, b]$ , then so is $\mathbf{r}$, and the definite integral of $\mathbf{r}$ from $a$ to $b$ is 
>$$
>\int_a^b \mathbf{r}(t)dt = \int_a^b f(t)dt\mathbf{i} + \int_a^bg(t)dt\mathbf{j} + \int_a^bh(t)dt\mathbf{k}
>$$ 
#### The Vector and Parametric Equations for Ideal Projectile Motion
>Ideal Projectile Motion Equation
>$$
>\mathbf{r} = (v_0\cos\alpha)t\mathbf{i} + ((v_0\sin\alpha) t - \dfrac{1}{2}gt^2)\mathbf{j} 
>$$

>Height, Flight Time, and Range for Ideal Projectile Motion  
For ideal projectile motion when an object is launched from the origin over a horizontal surface with initial speed $v_0$ and launch angle $\alpha$   
Maximum height:
>$$
>y_{\max} = \dfrac{(v_0\sin\alpha)^2}{2g}
>$$
>Flight time:
>$$
>t = \dfrac{2v_0\sin\alpha}{g}
>$$
>Range:
>$$
>t = \dfrac{v_0^2}{g}\sin2\alpha
>$$
#### Projectile Motion with Wind Gusts
