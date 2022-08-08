# Riemann Hypothesis in a Nutshell
## Preliminary
It all starts with counting how many prime numbers exist in the universe, i.e. $$p=\lbrace 2, 3, 5, 7, 11, ... \rbrace,$$
the answer is <strong>'infinitely many'</strong> (see Euclid's proof)!
<p/>
If we take a look at number $n$, and we use a function $\pi(n)$ to describe how many primes are there smaller than or equal to $n$, then this is called the <strong>prime counting function</strong>. For example, $\pi(10)$ $=count$ $prime$ $\leq 10$ $=count$ $\lbrace 2, 3, 5, 7 \rbrace$ $=4$.
<p/>
Gauss and Legendre gave the approximation of $\pi(n)$ as $n$ gets to $\infty$, namely 
$$\pi(n)\sim\frac{n}{log(n)},$$
meaning that $\pi(n)$ is proportional, or more precisely, <strong>asymptotic</strong> to $\frac{n}{log(n)},$
in the sense
$$\lim_{n\to\infty}\frac{\pi(n)}{\frac{n}{log(n)}}=1.$$
The plot below shows $\pi(n)$ (blue) and $\frac{n}{log(n)}$ (red) against $n$ for $0\leq{n}\leq{1000}$.
<p align="center"><img src= "https://user-images.githubusercontent.com/66701331/183235741-25934d76-cb71-48b8-aca9-6998e33cfc69.png" width="500" height="300"> <p/>
and we call this the <strong>Prime Number Theorem (PNT).</strong>

## Background
Consider the sum 
$$\zeta(s)=\sum_{n=1}^{\infty}\frac{1}{n^s}=\frac{1}{1^s}+\frac{1}{2^s}+\frac{1}{3^s}+...,$$
its simplest case takes place when $s=1$, the harmonic series
$$H(s)=\sum_{n=1}^{\infty}\frac{1}{n}=\frac{1}{1}+\frac{1}{2}+\frac{1}{3}+...,$$
this clearly diverges (review from calculus).
Now, we also know that for any real $s>1$ this automatically converges to a real value, for example
$$\sum_{n=1}^{\infty}\frac{1}{n^{1.1}}\approx10.584.$$
<p/>
In 1730s, Euler proofed that for all real $s>1$ we have
$$\zeta(s)=\sum_{n=1}^{\infty}\frac{1}{n^s}=\prod_{prime}\frac{1}{p^{-s}}=\frac{1}{2^{-s}}\cdot\frac{1}{3^{-s}}\cdot\frac{1}{5^{-s}}\cdot...,$$
where the sum is converted into a product over all prime numbers.
<p/>
Now, in the complex number case, we would have $s=a+bi$ where $re(s)=a$ and $im(s)=b$, then as usual the sum $\zeta(s)$ wil have a simple pole (singularity) at $re(s)=1$, and the region $0<re(s)<1$ is <strong>not convergent<\strong>. 
<p/>
In 1859, Bertrand Riemann published his only paper on number theory 'On the Number of Prime Numbers less than a Given Quantity' that later on became the most famous unsolved problem in mathematical history. In short, the <strong>Riemann Hypothesis (RH)</strong> can be viewed as an (suprisingly precise) approximation of the <strong>PNT</strong>.
<p/>
The point $$
region where $s<$
(to be continued...)
