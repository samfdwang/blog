---
title: "Harmonic functions"
date: 2018-06-06T14:53:02-04:00
math : true
tags:
  - Harmonic-Function
categories:
    - Inequality
---

# Note 1.
## Harmonic funtions
1. `$H^p$` space is a **disk** if the corresponding coniditon is bounded:
	: `$$M_p(r,f)=\{\frac{1}{2\pi}\int_{0}^{2\pi}|f(re^{i\theta})|^p\}^{1/p}$$`
	: `$$M_\infty(r,f)=\max_{0\leq \theta\leq 2\pi}|f(re^{i\theta})|$$`

2. `$H^q\subset H^p$` iff `$0<p<q\leq \infty$`
3. **Possion integral** on the disk
	: `$$u(z)=u(re^{i\theta})=\frac{1}{2\pi}\int_{0}^{2\pi}P(r,\theta-t)u(e^{i\theta})dt$$`
	: `$$P(r,\theta)=\frac{1-r^2}{1-2r\cos{\theta}+r^2}$$`
4. **Poisson-Stieltjes integrals**:
	: `$$u(z)=\frac{1}{2\pi}\int_{0}^{2\pi}P(r,\theta-t)d\mu(t)$$`
5. **Theorem 1**: the following three class of functions in `$|z|<1$` are identical:
  - (i). Poisson-Stieltjes integrals;
  - (ii). difference of two positive harmonic functions;
  - (iii). `$h^1$`, replace function in $H^1$ with real harmonic function.
6. **Helly selection theorem**: if uniformly bounded sequence `$\mu_{k}$` is uniformly bounded variation over interval `$[a,b]$`, then there exists a subseq `$\mu_{k_j}$` such that it converges everywhere in `$[a,b]$` to a bounded variation function `$\mu$` and for every continuous function `$\varphi(t)$`,
`$$\lim_{j\rightarrow\infty}\int_{a}^b\varphi(t)d\mu_{k_j}(t)=\int_a^b\varphi(t)d\mu(t)$$`

7. **Herglotz representation**
