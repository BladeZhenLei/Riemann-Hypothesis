<h2>Preliminary</h2>
In 1859, Bertrand Riemann published his only paper on number theory 'On the Number of Prime Numbers less than a Given Quantity', at the end, he proposed a question that later on became the most famous unsolved problem in the history of mathematics.
<p/>

<h3>Prime Numbers</h3>
It all starts with counting how many prime numbers exist in the universe, $p=\lbrace 2, 3, 5, 7, 11, ... \rbrace,$ the answer is <strong>infinitely many</strong> (see Euclid's proof)! 
<p/>

If we take a look at number $n$, and we use a function $\pi(n)$ to describe how many primes are there smaller than or equal to $n$, then this is called the <strong>prime counting function</strong>. 
<p/>
For example, $\pi(10)$ $=count$ $prime$ $\leq 10$ $=count$ $\lbrace 2, 3, 5, 7 \rbrace$ $=4$.
<p/>

In 18th century, Gauss and Legendre gave the approximation of $\pi(n)$ as it increases, namely ${\pi(n)}{\sim}{\frac{n}{log(n)}},$ meaning that $\pi(n)$ is proportional, or more precisely, <strong>asymptotic</strong> to $\frac{n}{log(n)},$ in the sense ${\lim_{n\to\infty}}{\frac{\pi(n)}{\frac{n}{log(n)}}}=1.$
<p/>
The plot below shows $\pi(n)$ (blue) and $\frac{n}{log(n)}$ (red) against $n$ for $0\leq{n}\leq{1000}$.
<p align="center"><img src= "https://user-images.githubusercontent.com/66701331/183235741-25934d76-cb71-48b8-aca9-6998e33cfc69.png" width="500" height="300"> <p/>
and we call this the <strong>Prime Number Theorem (PNT).</strong> <p/>

<h3>Zeta Function</h3>

Consider the sum 
$$\zeta(s)=\sum_{n=1}^{\infty}\frac{1}{n^s}=\frac{1}{1^s}+\frac{1}{2^s}+\frac{1}{3^s}+\cdot\cdot\cdot,$$
its simplest case takes place when $s=1$, the harmonic series
$$\sum_{n=1}^{\infty}\frac{1}{n}=\frac{1}{1}+\frac{1}{2}+\frac{1}{3}+\cdot\cdot\cdot,$$
this clearly diverges (review from calculus).
Now, we also know that for any real number $s>1$, this sum automatically converges to a real value.
<p/>
For example, $$\zeta(1.1)=\sum_{n=1}^{\infty}\frac{1}{n^{1.1}}\approx10.584.$$
In 1730s, Euler proofed that the following holds
$$\zeta(s)=\sum_{n=1}^{\infty}\frac{1}{n^s}=\prod_{prime}\frac{1}{1-p^{-s}}=\frac{1}{1-2^{-s}}\cdot\frac{1}{1-3^{-s}}\cdot\frac{1}{1-5^{-s}}\cdot\cdot\cdot\cdot,$$
for all real numbers $s>1$, where the sum is converted into a product over all prime numbers.<p/>

Now if we let $s=a+bi$ where $re(s)=a$ and $im(s)=b$, then this sum $\zeta(s)$ is called the <strong>Riemann Zeta Function</strong>, defined for $re(s)>1$ to have the regular sense of convergence.
<p/>

Although at first glance, $\zeta(s)$ diverges for ${re(s)}\leq{1}$, however, by performing what is called the <strong>analytic continuation</strong>, we are able to extend its domain with another definite expression (however this is done is unimportant because only one correct expression will be found).

<h3> The Hypothesis </h3>
The particular method Riemann used in his 1859 paper was a coutour integral, by going from $+\infty$ (above the real axis), around the origin, and then back to $+\infty$ (below the real axis),
<p align="center"><img src= "https://user-images.githubusercontent.com/66701331/183797725-2ff4c51d-2f6f-45dc-b2b0-d47715a91830.png" width="300" height="100"> <p/>
and yielded 
$$\zeta(s)=\frac{\Gamma(1-s)}{2{\pi}{i}}\int_{-\infty}^{+\infty}\frac{(-z)^{s}}{z(e^z-1)}\,dz.$$
This form of the Riemann Zeta Function is 'meromorphic', meaning analytic (convergent) everywhere except at a <strong>simple pole (singularity)</strong>, namely $re(s)=1$.
From the above expression Riemann was able to derive a Functional Equation that satistfies
$$\zeta(s)=2\Gamma(1-s)(2\pi)^{s-1}sin(\frac{\pi{s}}{2})\zeta(1-s),$$
and this is called the <strong>Riemann Functional Equation</strong>.
Now, the above expression shows that $\zeta(s)$ has zeros at $s=-2n$, they are so obvious that we call them the <strong>trivial zeros</strong>.
<p/>
However, through some very complicated calculations, more zeros are found with approximately $$\lbrace{s_1=\frac{1}{2}+14.134i, s_2=\frac{1}{2}+21.022i, s_3=\frac{1}{2}+25.010i, ...\rbrace},$$ they behave without any pattern (except that they have the same real part) and are called the <strong>non-trivial zeros</strong>.
<p/>
The famous <strong>Riemann Hypothesis (RH)</strong> is asserting: 
<p align="center"><strong>"All non-trivial zeros of the Riemann Zeta Function are located on the critical line where $re(s)=\frac{1}{2}$."</strong>
</p>
We can visualize a parametric plot of $\zeta(\frac{1}{2}+ix)$ with its real part against imaginary part (for ${0}\leq{x}\leq{100}$).
<p align="center"><img src= "https://user-images.githubusercontent.com/66701331/183802614-4c643272-1418-4376-82d5-5a5b80bdaaaf.png" width="500" height="450"> <p/>  
The most intriguing part of the Riemann Hypothesis is that these non-trivial zeros can be used to estimate the Prime Number Theorem with exceptional precision far beyond the asymptotic approximation!

<p align="center"><img src= "https://user-images.githubusercontent.com/66701331/189258075-c1e13ad0-59ff-4e1f-b5c7-51413d4c729a.gif" width="500" height="300"> <p/>


<p align="center"><strong>"(...to be continued...)<p/>
<html lang="en">
<head>
<meta http-equiv="content-type" content="text/html; charset=utf-8">
<script type="text/javascript" charset="utf-8" src="
https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>
</head>
