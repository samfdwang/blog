+++
title= "Note 1: Introduction to Theory of Distribution"
date = 2017-09-22T11:59:07-04:00
tags=["PDE","note.fa"]
categories=["PDE"]
[header]
image = "headers/distribution.jpg"
+++
This note is based on the lecture notes from PDE course taught by Dr. Khavinson.
{{% toc %}}
## Motivation of Theory of Distribution
Traditional function theory has 3 obstacles: differentiation, integration and convergence. That's the motivation of theory of distribution, which makes it possible to smoothly and systematically deal with those kind ill function (traditional point of view). In fact, distribution theory allow us to do more and it has fruitful results in linear partial differential equations.
### Differentiation problem
**Example** (Weierstrass' nowhere differentiable function) Show that
`$$h(t)=\sum_{0}^\infty\frac{\sin((r!)^2t)}{r!}\in C(\Pi=\{x\in \mathbb{R}:|x|=1\})$$`
and `$h(t)$` is nonwhere differentiable.

(Proof is left to reader.)

### Integral problem
Give a example that the fundamental theory doesn't hold, i.e. given a `$f(x)$` is differentiable a.e., but
`$$f(x)\neq f(a)+\int_{a}^xf'(z)dz$$`

### Convergence problem
`$f_n\rightarrow f, \text{ pointwise a.e.}$` doesn't always implies `$f_n'\rightarrow f'$`, give a example.

## Test functions and Distribution
**DEF 1.** Let `$X\subset \mathbb{R}^n$`, those functions in vector space `$C_c^\infty(X)$` are called *test functions*.

**Example**: Consider `$\psi(x)=\begin{cases}e^{\frac{1}{1-|x|^2}}&,|x|\leq 1\\ 0&,|x|>1\end{cases}$`, then `$\psi\in C_c^\infty(\mathbb{R}^n)$` with `$\text{supp}\psi=\text{ unit ball}$`.

`del me at last`
