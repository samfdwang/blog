+++
title = "Transfer a second order ODE to Volterra integral equation"
date = 2018-06-11T18:09:30-04:00
draft = false

# Tags and categories
# For example, use `tags = []` for no tags, or the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = ["volterra integral equation","Strum-Louville Equation","ODE"]
categories = ["integral equation"]

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
[header]
image = ""
caption = ""

+++
## Volterra integral eqaution
Usually there are two types of Volterra integral eqaution named as first kind and second kind.(Here we consider the linear Volterra integral equation only) In what follows, `$x(t)$` is the function to be solved.
+ *First kind Volterra integral equation*
`\[f(x)=\int_{a}^t K(t,s)x(t)dt\]`
where  `$K(t,s)$`  is called *kernel*.
+ *Second kind Volterra integral equation*
`\[x(t)=f(t)+\int_{a}^tK(t,s)x(s)ds\]`

## Strum-Louville problem
Let's consider the model equation: `$Y''(x,\lambda)+\lambda^2Y(x,\lambda)=V(x)Y(x,\lambda)$` .
You may find this kind of equation in Lax pair of the nonlinear differential equations. In this note, we are going to transfer this equation to second kind Volterra integral equation, so that we can use the method of successive approximations to find the solution and moreover analysis the analyticity with respect to parameter `$\lambda$` . Basically, what I am doing here is rephrasing the proof in Marchenko's book *The Inverse Problem of Scattering Theory*,theorem 1.2.1.

**Theorem 1** *If for some `$1>\epsilon\geq 0$` ,*
`\[\int_{0}x^{1-\epsilon}|V(x)|dx<\infty\]`
*then our model eqaution has a fundamental system of solutions `$G(x,\lambda)$` and `$H(x,\lambda)$` for each fixed value of `$\lambda$` ,satisfying the asymptotic relation:*
`\[\begin{aligned}
\begin{aligned}
        G(x,\lambda)&=x[I+o(x^\epsilon)],&G'(x,\lambda)&=I+o(x^\epsilon);\\
H(x,\lambda)&=I+o(x^\epsilon),&H'(x,\lambda)&=o(x^{-1+\epsilon}).
       \end{aligned}
 \qquad (x\rightarrow 0)
\end{aligned}\]`
*Moreover for each fixed value of `$x\geq 0$` , `$G$` is an entire function w.r.t. `$\lambda$` *

Now I will summarize the proof in following steps:
## Steps of the proof
1. [Find the corresponding volterra integral equation](#Find-the corresponding-volterra-integral-equation)
2. [Example2](#example2)
3. [Third Example](#third-example)

### Find the corresponding Volterra integral equation
As for how to find its corresponding integral equation, I didn't find good literature. Here are some possible useful thoughts.
#### Green's function (refer Ablowitz Solitons, Nonlinear Evolution Equations and inverse scttering)
In Ablowitz's book, they use Green's technique to deal with second order differential equations, like the model equation. Here we take equation `$v_{xx}+k^2v=-uv$` as example, first consider a transformation `$v(x,k)=m(x)$`
## Example2
## Third Example
