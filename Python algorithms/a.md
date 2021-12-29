$$
L(i,j) = \begin{cases}
    0 &i = 0\quad\mathsf{or}\quad j = 0  \\ 
    1 + L(i-1,j-1) & a_j = b_j \\
    \max(L(i-1,j),L(i,j-1))&\mathsf{otherwise}
\end{cases}
$$
![](../images/python%20algorithm/9.jpg)