# Thomas Calculus
## Chapter 10 Infinite Sequences and Series
### 10.1 Sequences
#### Finding Terms of a Sequence
Each of Exercises 1–6 gives a formula for the $n$th term $a_n$ of a
sequence ${a_n}$ Find the values of $a_1, a_2, a_3$, and $a_4$.

1. $a_n =\dfrac{1-n}{n^2}$  
   $a_1 = 0, a_2 = -\dfrac{1}{4},a_3 = -\dfrac{2}{9},a_4 =-\dfrac{3}{16}$  
#### Finding a Sequence’s Formula
In Exercises 13–30, find a formula for the nth term of the sequence.

13. $1, -1, 1, -1, 1,\cdots$  
    $1\cdot(-1)^{n-1}$
#### Convergence and Divergence
Which of the sequences 5an6 in Exercises 31–100 converge, and which diverge? Find the limit of each convergent sequence.

31. $a_n = 2 + (0.1)^n$   
    converge,$\lim\limits_{n\to\infty}a_n = 2$
#### Recursively Defined Sequences
In Exercises 101–108, assume that each sequence converges and find its limit.

101. $a_1 = 2, a_{n+1} = \dfrac{72}{1 + a_n}$  
     Let $\lim\limits_{n\to\infty}a_n = A$  
     $\lim\limits_{n\to\infty}a_{n+1} = \lim\limits_{n\to\infty}\dfrac{72}{1 + a_n}$  
     $A = \dfrac{72}{1 + A}$   
     $A^2 + A -72 = 0$  
     $A_1 = -9, A_2 = 8$  
     $a_1 = 2, a_n >0$  
     $\lim\limits_{n\to\infty}a_n = 8$
#### Theory and Examples
109. The first term of a sequence is $x_1 = 1$. Each succeeding term is the sum of all those that come before it:  
     $$
     x_{n+1} = x_1 + x_2 + \cdots + x_n
     $$
     Write out enough early terms of the sequence to deduce a general formula for $x_n$ that holds for $n \ge 2$  
     $x_1 = 1$  
     $x_2 = x_1 = 1$  
     $x_3 = x_1 + x_2 = 2x_2$  
     $x_4 = x_1 + x_2 + x_3 = 2x_3$  
     $x_5 = x_1 + x_2 + x_3 + x_4= 2x_4$  
     $x_n = x_1 + x_2 + x_4 + x_5 + \cdots + x_{n-1} = 2x_{n-1}$  
     ${x_n} = 2^{n-2}, n\ge 2$
#### COMPUTER EXPLORATIONS
Use a CAS to perform the following steps for the sequences in Exercises 147–158.  
a. Calculate and then plot the first 25 terms of the sequence. Does the sequence appear to be bounded from above or below? Does it appear to converge or diverge? If it does converge, what is the limit $L$?  
b. If the sequence converges, find an integer $N$ such that $|a_n - L| \le 0.01$ for $n \ge N$. How far in the sequence do you have to get for the terms to lie within $0.0001$ of $L$?

147. $a_n = \sqrt[n]{n}$  
     converges, $a_n\to 1$  
     $|\sqrt[n]{n} - 1| < 0.01$  
     $\sqrt[n]{n}< 1.01$  
     $n = 700$  
     $\sqrt[n]{n}< 1.0001, n = 1000000$
### 10.2  Infinite Series
#### Finding $n$th Partial Sums
In Exercises 1–6, find a formula for the $n$th partial sum of each series
and use it to find the series’ sum if the series converges.
1. $2 + \dfrac{2}{3} + \dfrac{2}{9} + \dfrac{2}{27} + \cdots + \dfrac{2}{3^{n-1}} + \cdots$  
   $S_n = \dfrac{2(1-(\frac{1}{3})^n)}{1-\frac{1}{3}} =3(1-(\frac{1}{3})^n)$  
   $\sum a_n = 3$
#### Series with Geometric Terms
In Exercises 7–14, write out the first eight terms of each series to show how the series starts. Then find the sum of the series or show
that it diverges.

7. $\sum\limits_{n = 0}^{\infty}\dfrac{(-1)^n}{4^n}$  
   $a_0 =1,a_1 = -\dfrac{1}{4},a_2 = \dfrac{1}{16},a_3 = -\dfrac{1}{64},a_4 = \dfrac{1}{4^4},a_5 = -\dfrac{1}{4^5},a_6 = \dfrac{1}{4^6},a_7 = -\dfrac{1}{4^7}$  
   $\sum a_n = \dfrac{1}{1+\frac{1}{4}} = \dfrac{4}{5}$
#### Repeating Decimals
Express each of the numbers in Exercises 23–30 as the ratio of two integers.

23. $0.\bar{23} = 0.23 23 23\cdots$  
    $\dfrac{23}{99}$  
#### Using the nth-Term Test
In Exercises 31–38, use the nth-Term Test for divergence to show that the series is divergent, or state that the test is inconclusive.

31. $\sum\limits_{n = 1}^{\infty}\dfrac{n}{10 + n}$    
    $\lim\limits_{n\to\infty}\dfrac{n}{10 + n} = 1$, diverges  
#### Telescoping Series
In Exercises 39–44, find a formula for the $n$th partial sum of the series and use it to determine if the series converges or diverges. If a series converges, find its sum.

39. $\sum\limits_{n = 1}^{\infty}(\dfrac{1}{n} - \dfrac{1}{n + 1})$  
    $S_n = 1-\dfrac{1}{2} + \dfrac{1}{2} - \dfrac{1}{3} + \dfrac{1}{3} - \dfrac{1}{4} + \cdots +\dfrac{1}{n} - \dfrac{1}{n+1}$   
    $= 1-\dfrac{1}{n+1}$  
    $\sum a_n = 1$
#### Convergence or Divergence
Which series in Exercises 53–76 converge, and which diverge? Give reasons for your answers. If a series converges, find its sum.

53. $\sum\limits_{n = 0}^{\infty}(\dfrac{1}{\sqrt{2}})^n$  
    converges, $\sum a_n = \dfrac{1}{1-\frac{1}{\sqrt{2}}} = \dfrac{\sqrt{2}}{\sqrt{2} -1}$
#### Geometric Series with a Variable $x$
In each of the geometric series in Exercises 77–80, write out the first few terms of the series to find $a$ and $r$, and find the sum of the series. Then express the inequality $|r| < 1$ in terms of $x$ and find the values of $x$ for which the inequality holds and the series converges.

77. $\sum\limits_{n = 0}^{\infty}(-1)^nx^n$  
    $a_0 = 1, a_1 = -x, a_2 = x^2$  
    $r = -x$  
    $\sum a_n = \dfrac{1}{1+x}$  
    $-1 < x < 1$
#### Theory and Examples
87. The series in Exercise 5 can also be written as  
    $$
    \sum_{n = 1}^{\infty}\dfrac{1}{(n+1)(n + 2)}\quad\mathsf{and}\quad\sum\limits_{n = -1}^{\infty}\dfrac{1}{(n+3)(n + 4)}
    $$
    Write it as a sum beginning with (a) $n = -2$, (b) $n = 0$, (c) $n = 5$  
    a. $\sum\limits_{n = -2}^{\infty}\dfrac{1}{(n+4)(n + 5)}$  
    b. $\sum\limits_{n = -1}^{\infty}\dfrac{1}{(n+2)(n + 3)}$  
    c. $\sum\limits_{n = 5}^{\infty}\dfrac{1}{(n-3)(n - 2)}$
### 10.3 The Integral Test
#### Applying the Integral Test
Use the Integral Test to determine if the series in Exercises 1–12 converge or diverge. Be sure to check that the conditions of the Integral Test are satisfied.

1. $\sum\limits_{n = 1}^{\infty}\dfrac{1}{n^2}$   
   For $x \ge 1, f(x) = \dfrac{1}{x^2}$is continuous, positive and decreasing  
   $\int_{1}^{\infty}\dfrac{1}{x^2}dx = \lim\limits_{b\to\infty}[-\dfrac{1}{x}]_1^b = \lim\limits_{b\to\infty}(-\dfrac{1}{b} +1) = 1$ converges, the series converges
#### Determining Convergence or Divergence
Which of the series in Exercises 13–46 converge, and which diverge? Give reasons for your answers. (When you check an answer, remember that there may be more than one way to determine the series’ convergence or divergence.)

13. $\sum\limits_{n = 1}^{\infty}\dfrac{1}{10^n}$   
   For $x \ge 1, f(x) = \dfrac{1}{10^x}$is continuous, positive and decreasing  
   $\int_{1}^{\infty}\dfrac{1}{10^x}dx$ converges, the series converges
#### Theory and Examples
For what values of $a$, if any, do the series in Exercises 47 and 48 converge?

1.  $\sum\limits_{n = 1}^{\infty}(\dfrac{a}{n + 2} - \dfrac{1}{n+4})$  
     $\dfrac{a}{n + 2} - \dfrac{1}{n+4}$  
     $= \dfrac{an +4a -n -2}{n^2 +6n +8}$  
     $= \dfrac{(a-1)n +4a-2}{(n + 3)^2 -1}$  
     $a - 1 \le 0, a \le 1$ 
### 10.4 Comparison Tests
#### Direct Comparison Test
In Exercises 1–8, use the Direct Comparison Test to determine if each series converges or diverges.
1. $\sum\limits_{n = 1}^{\infty}\dfrac{1}{n^2 + 30}$  
   $\dfrac{1}{n^2 + 30} < \dfrac{1}{n^2}$  
   $\sum\dfrac{1}{n^2}$ converges, the series converges
#### Limit Comparison Test
In Exercises 9–16, use the Limit Comparison Test to determine if each series converges or diverges.

9. $\sum\limits_{n = 1}^{\infty}\dfrac{n-2}{n^3 - n^2+ 3}$  
    $\lim\limits_{n\to\infty}\dfrac{\frac{n-2}{n^3 - n^2+ 3}}{\frac{1}{n^2}}$  
    $= \lim\limits_{n\to\infty}\dfrac{n^3-2n^2}{n^3 - n^2+ 3} = 1 > 0$  
    $\sum\dfrac{1}{n^2}$converges, the series converges
#### Determining Convergence or Divergence
Which of the series in Exercises 17–56 converge, and which diverge? Use any method, and give reasons for your answers.

17. $\sum\limits_{n = 1}^{\infty}\dfrac{1}{2\sqrt{n} + \sqrt[3]{n}}$  
    $\dfrac{1}{2\sqrt{n} + \sqrt[3]{n}} < \dfrac{1}{2\sqrt{n}} < \dfrac{1}{\sqrt{n}}$  
    $\int_1^{\infty}\dfrac{1}{\sqrt{x}}dx = \lim\limits_{b\to\infty}[2\sqrt{x}]_1^{b} = \lim\limits_{b\to\infty}(2\sqrt{b} -2),$ diverges  
    $\sum\dfrac{1}{\sqrt{n}}$ diverges, the series diverges.
#### Theory and Examples
57. Prove (a) Part 2 and (b) Part 3 of the Limit Comparison Test.  
    a. For $\varepsilon = 1,$ there is an integer $N$ such that   
    $|\dfrac{a_n}{b_n}| < 1$ whenever $n > N$   
    $-1 < \dfrac{a_n}{b_n} < 1, -b_n < a_n < b_n$  
    By the direct comparison test, if $\sum b_n$ converges, $\sum a_n$ converges  
    b. For $\varepsilon = 1,$ there is not an integer $N$ such that   
    $|\dfrac{a_n}{b_n}| < 1$ whenever $n > N$  
    For some $N, |\dfrac{a_n}{b_n}| > 1$  
    $a_n > b_n, or an < -b_n$  
    By the direct comparison test, if $\sum b_n$ diverges, $\sum a_n$ diverges
#### COMPUTER EXPLORATIONS
73. It is not yet known whether the series  
    $$
    \sum\limits_{n = 1}^{\infty}\dfrac{1}{n^3\sin^2n}
    $$
    converges or diverges. Use a CAS to explore the behavior of the series by performing the following steps.  
    a. Define the sequence of partial sums 
    $$
    s_k = \sum\limits_{n = 1}^{k}\dfrac{1}{n^3\sin^2n}
    $$
    What happens when you try to ind the limit of $s_k$ as $k \to\infty$? Does your CAS find a closed form answer for this limit?
    b. Plot the first 100 points $(k, s_k)$ for the sequence of partial sums. Do they appear to converge? What would you estimate the limit to be?  
    c. Next plot the first 200 points $(k, s_k)$. Discuss the behavior in your own words.   
    d. Plot the first 400 points $(k, s_k)$ What happens when $k = 355$? Calculate the number $\dfrac{355}{133}$. Explain from you calculation what happened at $k = 355$. For what values of $k$ would you guess this behavior might occur again?