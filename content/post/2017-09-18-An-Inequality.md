---
title: "An Inequality proved by Jensen Inequality"
date: 2017-09-18T14:46:01-04:00
math : true
tags:
  - Inequality
categories:
    - Inequality
---
Statement of the problem:
suppose `$x\in \mathbb{R}^n$` and `$\sum_{i=1}^nx_i=0$`, show that
`$$
\text{max} x_j>\frac{\|x\|_2}{n}
$$`
My proof is as following.
After reordering and relabeling the `$x_i$`, we can finally have:

`$$x_1+\cdots+x_k=x_{k+1}+\cdots+x_n$$`

where left side consists of positive numbers while the right side consists of non-positive numbers.
Then we have
`$$
\begin{split}
\|x\|_2^2 &= x_1^2+\cdots+x_n^2\\
&\leq x_1^2+\cdots+x_k^2+(x_{k+1}+\cdots+x_n)^2\\
&=x_1^2+\cdots+x_k^2+(x_1+\cdots+x_k)^2\\
&\leq x_1^2+\cdots+x_k^2+k(x_1^2+\cdots+x_k^2)\\
&=(1+k)(x_1^2+\cdots+x_k^2)\\
\end{split}
$$`
Hence
`$$
\frac{\|x\|_2}{n}\leq \frac{(1+k)^{1/2}\|\bar{x}\|_2}{n}\leq \frac{\sqrt{(1+k)k}x^*}{n}<x^*
$$`
where `$\bar{x}=(x_1,x_2,...,x_k)$` and `$x^*$` stands for maximum of `$x$`, and here we have used `$k(k+1)<n^2$` for all `$k<n,k,n\in \mathbb{N}$`
