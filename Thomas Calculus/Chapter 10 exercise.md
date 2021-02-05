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
### 10.5 Absolute Convergence; The Ratio and Root Tests
#### Using the Ratio Test
In Exercises 1–8, use the Ratio Test to determine if each series converges absolutely or diverges.
1. $\sum\limits_{n = 1}^{\infty}\dfrac{2^n}{n!}$   
   $\lim\limits_{n\to\infty}|\dfrac{\frac{2^{n+1}}{(n+1)!}}{\frac{2^n}{n!}}|$  
   $= \lim\limits_{n\to\infty}|\dfrac{2}{n + 1}| = 0 < 1$  
   The series absolutely converges. 
#### Using the Root Test
In Exercises 9–16, use the Root Test to determine if each series converges absolutely or diverges.

9. $\sum\limits_{n = 1}^{\infty}\dfrac{7}{(2n + 5)^n}$  
   $\lim\limits_{n\to\infty}\sqrt[n]{|\dfrac{7}{(2n + 5)^n}|}$  
   $= \lim\limits_{n\to\infty}\dfrac{\sqrt[n]{7}}{|2n + 5|} = 0 < 1$  
   The series absolutely converges.
#### Determining Convergence or Divergence
In Exercises 17–46, use any method to determine if the series converges or diverges. Give reasons for your answer.

17. $\sum\limits_{n = 1}^{\infty}\dfrac{n^{\sqrt{2}}}{2^n}$   
    $\lim\limits_{n\to\infty}|\dfrac{\frac{(n + 1)^{\sqrt{2}}}{2^{n + 1}}}{\frac{n^{\sqrt{2}}}{2^n}}|$  
    $= \lim\limits_{n\to\infty}|(\dfrac{n + 1}{n})^{\sqrt{2}}\dfrac{1}{2}| = \dfrac{1}{2} < 1$  
    converges
#### Convergence or Divergence
Which of the series in Exercises 57–64 converge, and which diverge? Give reasons for your answers.

57. $\sum\limits_{n = 1}^{\infty}\dfrac{2^n n!n!}{(2n)!}$  
    $\lim\limits_{n\to\infty}|\dfrac{\frac{2^{n + 1} (n + 1)!(n + 1)!}{(2n + 2)!}}{\frac{2^n n!n!}{(2n)!}}|$  
    $= \lim\limits_{n\to\infty}|\dfrac{2(n + 1)^2}{(2n + 2)(2n + 1)}| = \dfrac{1}{2} < 1$  
    converges
#### Theory and Examples
67. Neither the Ratio Test nor the Root Test helps with $p$-series. Try them on
    $$
    \sum\limits_{n = 1}^{\infty}\dfrac{1}{n^p}
    $$
    and show that both tests fail to provide information about convergence.  
    $\lim\limits_{n\to\infty}|\dfrac{\frac{1}{(n + 1)^p}}{\frac{1}{n^p}}|$  
    $= \lim\limits_{n\to\infty}|(\dfrac{n}{n + 1})^p| = 1$  
    $\lim\limits_{n\to\infty}\sqrt[n]{|\dfrac{1}{n^p}|}$  
    $= \lim\limits_{n\to\infty}\dfrac{1}{|n^{\frac{p}{n}}|} = 1$ 
### 10.6 Alternating Series and Conditional Convergence 
#### Determining Convergence or Divergence
In Exercises 1–14, determine if the alternating series converges or diverges. Some of the series do not satisfy the conditions of the Alternating Series Test.
1. $\sum\limits_{n = 1}^{\infty}(-1)^{n + 1}\dfrac{1}{\sqrt{n}}$   
   $\dfrac{1}{\sqrt{n}} \ge \dfrac{1}{\sqrt{n + 1}}$ for $n \ge 1$  
   $\dfrac{1}{\sqrt{n}} > 0$  
   $\dfrac{1}{\sqrt{n}} \to 0$  
   converges
#### Absolute and Conditional Convergence
Which of the series in Exercises 15–48 converge absolutely, which converge, and which diverge? Give reasons for your answers.

15. $\sum\limits_{n = 1}^{\infty}(-1)^{n + 1}(0.1)^n$  
    $(0.1)^n \ge (0.1)^{n + 1}$ for $n \ge 1$  
   $(0.1)^n > 0$  
   $(0.1)^n \to 0$  
   converges
#### Error Estimation
In Exercises 49–52, estimate the magnitude of the error involved in using the sum of the first four terms to approximate the sum of the entire series.

49. $\sum\limits_{n = 1}^{\infty}(-1)^{n + 1}\dfrac{1}{n}$  
    $E < \dfrac{1}{5}$  
    $\dfrac{7}{12} < L < \dfrac{47}{60}$  
    $L + \dfrac{1}{4} > 0$
#### Theory and Examples
85. a. The series
    $$
    \dfrac{1}{3} -\dfrac{1}{2} + \dfrac{1}{9} -\dfrac{1}{4} + \dfrac{1}{27} - \dfrac{1}{8} + \cdots + \dfrac{1}{3^n} - \dfrac{1}{2^n} + \cdots
    $$
    does not meet one of the conditions of Theorem 14. Which one?  
    b. Use Theorem 17 to find the sum of the series in part (a)  
    a. $\dfrac{1}{3^n} - \dfrac{1}{2^n} < 0$  
    b. $\sum | \dfrac{1}{3^n} - \dfrac{1}{2^n}| = \dfrac{1}{2^n} - \dfrac{1}{3^n}$ converges  
    $\sum \dfrac{1}{3^n} - \dfrac{1}{2^n} = \sum \dfrac{1}{3^n} - \sum\dfrac{1}{2^n} = \dfrac{1}{1-\frac{1}{3}} - \dfrac{1}{1-\dfrac{1}{2}} = -\dfrac{1}{2}$
### 10.7 Power Series
#### Intervals of Convergence
In Exercises 1–36, (a) find the series’ radius and interval of convergence. For what values of $x$ does the series converge (b) absolutely, (c) conditionally?
1. $\sum\limits_{n = 1}^{\infty}x^n$  
   $\lim\limits_{n\to\infty}\sqrt[n]{|x^n|} = |x|$  
   $-1 < x < 1$, converges  
   $x = \plusmn1$, diverges  
   $R = 1, I = (-1,1)$  
   For $(-1,1)$, converges absolutely
#### Using the Geometric Series
49. In Example 2 we represented the function $f(x) =\dfrac{2}{x}$ as a power series about $x = 2.$ Use a geometric series to represent $f(x)$ as a power series about $x = 1$, and find its interval of convergence.  
    $\dfrac{c_1}{1-a(x-1)} = \dfrac{2}{x}$  
    $2 - 2ax + 2a = c_1x, a = -1, c_1 = 2$  
    $\dfrac{2}{x} = 2-2(x-1)+2(x-1)^2 - 2(x-1)^3 + \cdots = \sum\limits_{n = 0}^{\infty}2(1-x)^{n}$  
    $|1-x| < 1, -1 < 1-x < 1, 0 < x < 2$
#### Theory and Examples
53. For what values of $x$ does the series  
    $$
    1-\dfrac{1}{2}(x-3)+\dfrac{1}{4}(x-3)^2 + \cdots + (-\dfrac{1}{2})^n(x-3)^{n} +\cdots
    $$
    converge? What is its sum? What series do you get if you differentiate the given series term by term? For what values of $x$ does the new series converge? What is its sum?  
    $|-\dfrac{x-3}{2}| < 1$  
    $1 < x < 5$  
    $\sum (-\dfrac{1}{2})^n(x-3)^{n} = \dfrac{1}{1+\frac{x-3}{2}} =\dfrac{2}{x-1}$  
    $\dfrac{d}{dx}\sum\limits_{n = 0}^{\infty} (-\dfrac{1}{2})^n(x-3)^{n} = \sum\limits_{n = 1}^{\infty} n(-\dfrac{1}{2})^n(x-3)^{n-1}$  
    converges in $(1,5)$   
    $s_n = 1(-\dfrac{1}{2}) + 2(-\dfrac{1}{2})^2(x-3) + 3(-\dfrac{1}{2})^3(x-3)^2 + \cdots + n(-\dfrac{1}{2})^n(x-3)^{n-1}$   
    $-\dfrac{x-3}{2}s_n = 1(-\dfrac{1}{2})^2(x-3) + 2(-\dfrac{1}{2})^3(x-3)^2 + \cdots + (n-1)(-\dfrac{1}{2})^n(x-3)^{n-1} + n(-\dfrac{1}{2})^{n + 1}(x-3)^n$  
    $(1 + \dfrac{x-3}{2})s_n = -\dfrac{1}{2} + (-\dfrac{1}{2})^2(x-3) + (-\dfrac{1}{2})^3(x-3)^2 + \cdots + (-\dfrac{1}{2})^n(x-3)^{n-1} - (-\dfrac{1}{2})^{n + 1}(x-3)^n$  
    $\lim\limits_{n\to\infty}(1 + \dfrac{x-3}{2})s_n = \dfrac{1}{1+\frac{x-3}{2}}$   
    $\sum\limits_{n = 1}^{\infty} n(-\dfrac{1}{2})^n(x-3)^{n-1} = (\dfrac{2}{x-1})^2$
### 10.8 Taylor and Maclaurin Series
#### Finding Taylor Polynomials
In Exercises 1–10, find the Taylor polynomials of orders 0, 1, 2, and 3 generated by $f$ at $a$.
1. $f(x) = e^{2x}, a = 0$   
   $f'(x) = 2^{2x}, f''(x) = 4^{2x}, f'''(x) = 8^{2x}$
   $f(0) = 1$  
   $f(0) + f'(0)x = x + 1$  
   $f(0) + f'(0)x + \dfrac{f''(0)}{2!}x^2 = \dfrac{1}{2}x^2 + x + 1$  
   $f(0) + f'(0)x + \dfrac{f''(0)}{2!}x^2 + \dfrac{f'''(0)}{3!}x^3 = \dfrac{1}{6}x^3 + \dfrac{1}{2}x^2 + x + 1$
#### Finding Taylor Series at $x = 0$ (Maclaurin Series)
Find the Maclaurin series for the functions in Exercises 11–24.

11. $e^{-x}$  
    $f^{(n)}(x) = (-1)^ne^{-x},f^{(n)}(0) = 1$   
    $f(0) + f'(0)x + \dfrac{f''(0)}{2!}x^2 + \dfrac{f'''(0)}{3!}x^3 + \cdots + \dfrac{f^{(n)}(0)}{n!}x^n + \cdots$  
    $= 1 + \dfrac{1}{2!}x^2 + \dfrac{1}{3!}x^3 + \cdots + \dfrac{f''(0)}{n!}x^n + \cdots$  
#### Finding Taylor and Maclaurin Series
In Exercises 25–34, find the Taylor series generated by ƒ at x = a.

25. $f(x) = x^3 - 2x + 4, a = 2$  
    $f'(x) = 3x^2 - 2$  
    $f''(x) = 6x$  
    $f'''(x) = 6$  
    $f(2) + f'(2)x + \dfrac{f''(2)}{2!}x^2 + \dfrac{f'''(3)}{3!}x^3$  
    $= (x-2)^3 + 6(x-2)^2 + 10(x-2) + 8$
#### Theory and Examples
41. Use the Taylor series generated by $e^x$ at $x = a$ to show that  
    $$
    e^x = e^a[1 + (x-a) + \dfrac{(x-a)^2}{2!} + \cdots]  
    $$  
    $f^{(n)}(x) = e^x, f^{(n)}(a) = e^a$  
    $f(a) + f'(a)(x-a) + \dfrac{f''(a)}{2!}(x-a)^2 + \dfrac{f'''(a)}{3!}(x-a)^3 + \cdots + \dfrac{f''(a)}{n!}(x-a)^n + \cdots$  
    $= e^a[1 + (x-a) + \dfrac{(x-a)^2}{2!} + \cdots]$
### 10.9 Convergence of Taylor Series
#### Finding Taylor Series
Use substitution (as in Example 4) to find the Taylor series at $x = 0$ of the functions in Exercises 1–12.
1. $e^{-5x}$  
   $= \dfrac{1}{(e^x)^5}$  
   $= \dfrac{1}{(1 + x + \frac{1}{2}x^2+ \frac{1}{3!}x^3 + \cdots)^5}$
#### Error Estimates
39. Estimate the error if $P_3(x) = x-\dfrac{x^3}{6}$ is used to estimate the value of $\sin x$ at $x = 0.1$  
    At $x = 0$  
    $f'(x) = 1$  
    $f''(x)  = 0$  
    $f'''(x) = -1$  
    $f''''(t) = \sin t < 1$ for $t\in(0,0.1)$
    $|E| \le \dfrac{0.1^4}{4!}$  
#### Theory and Examples
47. Use the identity $\sin^2x = \dfrac{1 - \cos 2x}{2}$ to obtain the Maclaurin series for $\sin^2x$. Then differentiate this series to obtain the Maclaurin series for $2 \sin x \cos x$. Check that this is the series for $\sin 2x$.  
    $f'(x) = \sin 2x$  
    $f''(x) = 2\cos 2x$  
    $f'''(x) = -4\sin 2x$  
    $f(0) + f'(0)x + \dfrac{f''(0)}{2!}x^2 + \dfrac{f'''(0)}{3!}x^3 + \cdots$  
    $= x^2 - \dfrac{1}{24}x^4 + \dfrac{2}{45}x^6 + \cdots$  
    $2\sin x\cos x$  
    $2x - \dfrac{1}{6}x^3 + \dfrac{4}{15}x^5 + \cdots$
#### COMPUTER EXPLORATIONS
Taylor’s formula with $n = 1$ and $a = 0$ gives the linearization of a function at $x = 0.$ With $n = 2$ and $n = 3$ we obtain the standard quadratic and cubic approximations. In these exercises we explore the errors associated with these approximations. We seek answers to two questions:  
a. For what values of $x$ can the function be replaced by each approximation with an error less than $10^{-2}$?   
b. What is the maximum error we could expect if we replace the function by each approximation over the specified interval?  
Using a CAS, perform the following steps to aid in answering questions (a) and (b) for the functions and intervals in Exercises 57–62.   
Step 1: Plot the function over the specified interval.   
Step 2: Find the Taylor polynomials $P_1(x), P_2(x),$ and $P_3(x)$ at $x = 0$.  
Step 3: Calculate the $(n + 1)$st derivative $f^{(n+1)}(c)$ associated with the remainder term for each Taylor polynomial. Plot the derivative as a function of $c$ over the specified interval and estimate its maximum absolute value, $M$.  
Step 4: Calculate the remainder $R_n(x)$ for each polynomial. Using the estimate $M$ from Step 3 in place of $f^{(n+1)}(c)$, plot $R_n(x)$ over the specified interval. Then estimate the values of $x$ that answer question (a).  
Step 5: Compare your estimated error with the actual error $E_n(x) = |f(x) - P_n(x)|$ by plotting $E_n(x)$ over the specified interval. This will help answer question (b).  
Step 6: Graph the function and its three Taylor approximations together. Discuss the graphs in relation to the information discovered in Steps 4 and 5.  
57. $f(x) = \dfrac{1}{\sqrt{1+x}}, |x| < \dfrac{3}{4}$   
    $f'(x) = -\dfrac{1}{2(1+x)^{\frac{3}{2}}}$  
    $f''(x) = \dfrac{3}{4(1+x)^{\frac{5}{2}}}$  
    $f'''(x) = -\dfrac{15}{8(1+x)^{\frac{7}{2}}}$  
    $f''''(x) = \dfrac{105}{16(1+x)^{\frac{9}{2}}}$  
    $P_1(x) = 1 -\dfrac{1}{2}x$  
    $P_2(x) = 1-\dfrac{1}{2}x + \dfrac{3}{8}x^2$  
    $P_3(x) = 1-\dfrac{1}{2x} + \dfrac{3}{8}x^2 - \dfrac{5}{16}x^3$  
    $f''''(x) < M = 3360$  
    $R_1(x) = M\dfrac{x^2}{2}$  
    $R_2(x) = M\dfrac{|x^3|}{6}$  
    $R_3(x) = M\dfrac{|x^4|}{24}< \dfrac{1}{100}$  
    $|x| < 0.09$
### 10.10 Applications of Taylor Series
#### Binomial Series
Find the first four terms of the binomial series for the functions in Exercises 1–10.
1. $(1 + x)^{\frac{1}{2}}$  
   $(1 + x)^{\frac{1}{2}}$   
   $= 1 + \dfrac{1}{2}x + \dfrac{-\frac{1}{4}}{2!}x^2 + \dfrac{\frac{8}{3}}{3!}x^3$  
   $= \dfrac{4}{9}x^3 - \dfrac{1}{8}x^2 + \dfrac{1}{2}x + 1$
#### Approximations and Nonelementary Integrals
In Exercises 15–18, use series to estimate the integrals’ values with an error of magnitude less than $10^{-5}$. (The answer section gives the integrals’ values rounded to seven decimal places.)

15. $\int_0^{0.6}\sin x^2dx$  
    $\int_0^{0.6}\sin x^2dx = \dfrac{0.6^3}{3!} - \dfrac{0.6^7}{7\cdot3!} + \dfrac{0.6^11}{11\cdot5!} - \cdots$  
    $\dfrac{0.6^{11}}{11\cdot5!} < 10^{-5}$  
    $\int_0^{0.6}\sin x^2dx \approx 0.0353$
#### Indeterminate Forms
Use series to evaluate the limits in Exercises 29–40.

29. $\lim\limits_{x\to0}\dfrac{e^x-(1+x)}{x^2}$   
    $\dfrac{e^x-(1+x)}{x^2}$  
    $= \dfrac{1 + x + \frac{x^2}{2} + \cdots -1 -x}{x^2}$  
    $= \dfrac{1}{2} + \dfrac{x}{3!} + \dfrac{x^2}{4!} + \cdots$  
    $\lim\limits_{x\to0}\dfrac{e^x-(1+x)}{x^2} = \dfrac{1}{2}$
#### Using Table 10.1
In Exercises 41–52, use Table 10.1 to find the sum of each series.

41. $1 + 1 + \dfrac{1}{2!} + \dfrac{1}{3!} + \dfrac{1}{4!} + \cdots$  
    $e$
#### Theory and Examples
53. Replace $x$ by $-x $in the Taylor series for $\ln (1 + x)$ to obtain a series for $\ln (1 - x)$. Then subtract this from the Taylor series for $\ln (1 + x)$ to show that for $|x| < 1$,  
    $$
    \ln \dfrac{1 + x}{1-x} = 2(x + \dfrac{x^3}{3} + \dfrac{x^5}{5}) + \cdots
    $$
    $\ln (1 + x) = x - \dfrac{x^2}{2} + \dfrac{x^3}{3} - \cdots$  
    $\ln (1-x) = -x - \dfrac{x^2}{2} - \dfrac{x^3}{3} - \cdots$  
    $\ln \dfrac{1 + x}{1-x} = 2x + \dfrac{2}{3}x^3 + \dfrac{2}{5}x^5 + \cdots$  
    $= 2(x + \dfrac{x^3}{3} + \dfrac{x^5}{5}) + \cdots$  
#### Euler’s Identity
67. Use Equation (4) to write the following powers of $e$ in the form $a + bi$.  
a. $e^{-i\pi}$b. $e^{\frac{i}{4}\pi}$  c. $e^{-\frac{i}{2}\pi}$  
a. $e^{-i\pi} = -1$  
b. $e^{\frac{i}{4}\pi} = \dfrac{\sqrt{2}}{2} + \dfrac{\sqrt{2}}{2}i$  
c. $e^{-\frac{i}{2}\pi} = -i$