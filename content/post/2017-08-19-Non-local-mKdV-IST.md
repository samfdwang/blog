---
title: "Applying IST to nonlocal mKdV"
date: 2017-08-19T19:46:33-04:00
tags:
	- IST
	- mKdV
	- soliton
---
# Introduction
The classical nonlinear schrodinger equation(NLS)
\[
iq_t(x,t)=q_{xx}(x,t)\pm 2|q(x,t)|^2q(x,t)
\]

has been deeply studied by physicians and mathematicians due to its wide applications in physical fields. (in a word, a lot of applications, however I, as a math PhD, don't completely understand the physical background of NLS.). Soliton solutions of the NLS equation however is one the most interesting research. But there's no general techniques to find soliton solutions for all kinds of nonlinear wave equations. Inverse scattering transformation (IST) method is one of the most efficient way to deal with nonlinear equations i.e. the NLS equation. There are many papers discussion this topic. Here I want to mention the celebrated **AKNS system**
\[
\begin{align}
v_{1,x}&=-ikv_1+q(x,t)v_2\\
v_{2,x}&=ikv_2+r(x,t)v_1
\end{align}
\]
introduced by and named after Mark J. Ablowitz, David J. Kaup, and Alan C.

Readers are referred to two books written by [Ablowitz](https://sites.google.com/site/ablowitz/), which are [Solitons, Nonlinear  Evolution Equations  and Inverse Scattering](https://www.amazon.com/Nonlinear-Evolution-Equations-Scattering-Mathematical/dp/0521387302), [Solitons  and  the  Inverse  Scattering Transform](http://www.umbc.edu/photonics/Menyuk/Zweck/Ablowitz-Segur_1981.pdf). (you can watch and download the PDF version for the second one.) And Ablowitz also wrote a book about how to apply IST to NLS equation, including continuous and discrete NLS, which is a very beautiful book to read.

Recently, I mean 2016, Ablowitz and Z. H. Musslimani published a paper on Nonlinearity discussing nonlocal nonlinear wave equations, particularly, the Non-local Nonlinear Schrodinger Equation:
\[
iq_t(x,t)=q_{xx}(x,t)\pm2q(x,t)q^*(-x,t)q(x,t)
\]
where `$q^*(x,t)$` is the complex conjuation of `$q(x,t)$`.

Very recently, Jia-Liang Ji and Zuo-Nong Zhu, presented a nonlocal mKdV equation:
\[
q_t(x,t)+6q(x,t)q(-x,-t)q_x(x,t)+q_{xxx}(x,t)=0
\]
which can be reduced from AKNS system by implementing `$r(x,t)=-q(-x,-t)$`. 

# Apply IST to nonlocal mKdV step by step
