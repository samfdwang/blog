---
title: "Applying IST to nonlocal mKdV"
date: 2017-08-19T19:46:33-04:00
categories:
  - IST
  - Soliton
tags:
  - Soliton
  - NLS
  - AKNS
  - IST
---
# Introduction
The classical nonlinear schrodinger equation(NLS)


`$$
iq_t(x,t)=q_{xx}(x,t)\pm 2|q(x,t)|^2q(x,t)
$$`

has been deeply studied by physicians and mathematicians due to its wide applications in physical fields. Soliton solutions of the NLS equation however is one the most interesting research. But there's no general techniques to find soliton solutions for all kinds of nonlinear wave equations. Inverse scattering transformation (IST) method is one of the most efficient way to deal with nonlinear equations i.e. the NLS equation. There are many papers discussion this topic. Here I want to mention the celebrated **AKNS system**
`$$
\begin{align}
v_{1,x}&=-ikv_1+q(x,t)v_2\\
v_{2,x}&=ikv_2+r(x,t)v_1
\end{align}
$$`
introduced by and named after Mark J. Ablowitz, David J. Kaup, and Alan C.<!--more-->

Readers are referred to two books written by [Ablowitz](https://sites.google.com/site/ablowitz/), which are [Solitons, Nonlinear  Evolution Equations  and Inverse Scattering](https://www.amazon.com/Nonlinear-Evolution-Equations-Scattering-Mathematical/dp/0521387302), [Solitons  and  the  Inverse  Scattering Transform](http://www.umbc.edu/photonics/Menyuk/Zweck/Ablowitz-Segur_1981.pdf). (you can watch and download the PDF version for the second one.) And Ablowitz also wrote a book about how to apply IST to NLS equation, including continuous and discrete NLS, which is a very beautiful book to read.

Recently, I mean 2016, Ablowitz and Z. H. Musslimani published a paper on Nonlinearity discussing nonlocal nonlinear wave equations, particularly, the Non-local Nonlinear Schrodinger Equation:
`$$
iq_t(x,t)=q_{xx}(x,t)\pm2q(x,t)q^*(-x,t)q(x,t)
$$`
where `$q^*(x,t)$` is the complex conjuation of `$q(x,t)$`.

Very recently, Jia-Liang Ji and Zuo-Nong Zhu, presented a nonlocal mKdV equation:
`$$
\label{nmkdv}
q_t(x,t)+6q(x,t)q(-x,-t)q_x(x,t)+q_{xxx}(x,t)=0\tag{0}
$$`
which can be reduced from AKNS system by implementing `$r(x,t)=-q(-x,-t)$`.
Next I will show how to apply IST to mKdV step by step and finally get `$N-$`soliton solution.

# Apply IST to nonlocal mKdV step by step
**Step 1.** Write down the Lax pair or spectral problem.

Let's consider the following spectral problem:
`$$
\begin{align}
\varphi_x(x,t)&=U\varphi(x,t),\tag{1}\label{lax}\\
\varphi_t(x,t)&=V\varphi(x,t),\tag{2}
\end{align}
$$`
with
`$$
U=
\begin{bmatrix}
-ik & q(x,t)\\
r(x,t) & ik\\
\end{bmatrix},\\
V=-4ik^3\sigma_3+4k^2Q-2ikV_1+V2,\\
\sigma_3=
\begin{bmatrix}
1 & 0\\
0 & -1\\
\end{bmatrix},
Q=
\begin{bmatrix}
0 & q(x,t)\\
r(x,t) &0\\
\end{bmatrix}\\
V_1=(Q^2+Q_x)\sigma_3,\quad\quad V_2=-Q_{xx}+2Q^3+Q_xQ-QQ_x
$$`
The compatibility condition which is `$\varphi_{xt}(x,t)=\varphi_{t,x}(x,t)$` leads to
`$$\label{gmkdv}
q_t(x,t)+q_{xxx}(x,t)-6q(x,t)r(x,t)q_x(x,t)=0,\\
r_t(x,t)+r_{xxx}(x,t)-6r(x,t)q(x,t)r_x(x,t)=0.\tag{3}
$$`
The nonlocal mKdV equation (\ref{nmkdv}) can be reduced from equation (\ref{gmkdv}) by setting `$$\label{rd} r(x,t)=-q(-x,-t)\tag{4}$$`
**Step 2.** Set boundary conditions.(standard procedure of IST)

Fix time `$t=0$`, and define `$\phi(x,k)$` and `$\bar{\phi}(x,t)$` as a pair of eigenfunctions (or solutions) of euqaiton (\ref{lax}), which satisfy the following boundary conditions:
`$$
\phi(x,k)\sim\begin{bmatrix}1\\0\\\end{bmatrix}e^{-ikx},\bar{\phi}(x,k)\sim\begin{bmatrix}0\\1\\\end{bmatrix}e^{ikx},\quad x\rightarrow -\infty
$$`
Similarly, define another pair of solutions of equation (\ref{lax}) satisfying the following boundary conditions:
`$$
\psi(x,k)\sim\begin{bmatrix}0\\1\\\end{bmatrix}e^{ikx},\bar{\psi}(x,k)\sim\begin{bmatrix}1\\0\\\end{bmatrix}e^{-ikx},\quad x\rightarrow +\infty
$$`
**Step 3.** Scattering data and some symmetry relations.

Since `$\{\phi,\bar{\phi}\}$` and `$\{\psi,\bar{\psi}\}$` are linear dependent, we set
`$$
\begin{align}
\phi(x,k)=a(k)\bar{\psi}+b(k)\psi\\
\bar{\phi(x,k)}=\bar{a}(k)\psi+\bar{b}(k)\bar{\psi}
\end{align}
$$`
here `$a(k),b(k),\bar{a}(k),\bar{b}(k)$` are scalars, so we can solve them and will obtain and be expressed by Wronskian
`$$
\begin{align}
a(k)=W[\phi,\psi],b(k)=W[\psi,\bar{\phi}]\\
\bar{a}(k)=W[\bar{\psi},\bar{\phi}],\bar{b}(k)=W[\bar{\phi},\psi]
\end{align}
$$`

Next we need to analysis the region where the solutions are analytic.

(waiting to be updated.....)
