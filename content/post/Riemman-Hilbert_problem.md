Introduction
============

Plemelj Formula
===============

Cauchy Type Integral
====================

Scalar Riemann-Hilbert Problem
==============================

Fundamental Knowledge
---------------------

-   $w=u(x,y)+iv(x,y)$ maps point in $z-plane$ to $w-plane$

Closed contour case
-------------------

Given a closed contour $C$ and a function $g(t)\neq 0$ defined on
$C$,which satisfies Hölder condition, find a sectionally analytic
function $\Phi(z)$ such that $$\label{BV}
\Phi^+(t)=g(t)\Phi^-(t),t\in C$$ where
$\Phi^{\pm}(z)\in H(D^{\pm})$,$D^+$ and $D^-$ are inside and outside of
contour $C$ respectively. The equation \[BV\] is also called boundary
value of the Riemann-Hilbert problem.

Here gives the solution to the Riemann-Hilbert problem: $$\label{GS}
\Phi(z)=X(z)P(z)$$ where $X(z)$ called fundamental solution to the RHP
has the following form: $$X(z)=\begin{cases}
e^{\Gamma(z)},z\in D^+ \\
z^{-k}e^{\Gamma(z)},z\in D^-
\end{cases}$$
$$\Gamma(z):=\frac{1}{2\pi i}\int _C\frac{\log(\tau^{-k}g(\tau)\text{d}\tau}{\tau-z}$$
where $k=\text{ind}\,g(t)$, the index of $g(t)$ with respect to contour
$C$.. The general solution \[GS\] is derived from the fundamental
solution multiple by a polynomial with degree no less than 0. The basis
idea to obtain the fundamental solution is applying Plemelj formula,
which is:

$$\begin{aligned}
\Phi^+(t)-\Phi^-(t) &=\phi(t) \label{pfa}\\
\Phi^+(t)+\Phi^-(t) &=\frac{1}{\pi i}\int_{C}\frac{\phi(\tau)\text{d}\tau}{\tau-t}\end{aligned}$$

where $t$ is on the contour.

In fact, using logarithm to transfer multiple to difference will finally
arrived at equation in form of \[pfa\], more details seen the Textbook.

Next the inhomogeneous RHP will be considered, which providing the same
conditions as homogeneous RHP except for boundary value, the
inhomogeneous RHP satisfies: $$\label{iRHP}
\Phi^+(t)=g(t)\Phi^-(t)+f(t),t\in C$$ and $f(t)$ satisfies Hölder
condition.

To solve this problem, first we need solve the homogeneous part, using
the method given for homogeneous RHP, as a result we will get the
fundamental solution $X(z)$ such that $X^+(t)=g(t)X^-(t)$, substitute
$g(t)$ by $\frac{X^+(t)}{X^-(t)}$ to equation \[iRHP\], we will get:
$$\frac{\Phi^+(t)}{X^+(t)}-\frac{\Phi^-(t)}{X^-(t)}=\frac{f(t)}{X^+(t)}$$
Using Plemelj formula, we have :
$$\Phi^{\pm}(z)=\frac{X^{\pm}(z)}{2\pi i}\int_C\frac{f(\tau)\text{d}\tau}{X^+(\tau)(\tau-z)}$$

Hence in general, the inhomogeneous RHP has solution of the following
form:
$$\Phi(z)=X(z)(P(z)+\Psi(z)),\Psi(z)=\frac{1}{2\pi i}\int_C\frac{f(\tau)\text{d}\tau}{X^+(\tau)(\tau-z)}$$

Open contour case
-----------------

Using the limiting of the Cauchy type integral in the end of the open
contour.

Application to singular integral equations
------------------------------------------

1.  Solving singular integral equation

2.  Hilbert problem

3.  Abel integral problem

4.  Integral equation with logarithm kernel

Examples
========

Riemann-Hilbert Problem in solving KdV 
---------------------------------------

In this section, we consider the Korteweg-de Vries (KdV) equation:
$$u_t+6uu_x+u_{xxx}=0$$ Take KdV equation as an example to illustrate
inverse scattering transform (IST) and how the Riemann-Hilbert problem
works in IST. Let’s first begin with the time dependent Schrödinger
Equation: $$\label{sp1}
\mathcal{L}\psi=\lambda \psi$$ where
$\mathcal{L}=\frac{\text{d}^2}{\text{d}x^2}+q(x)$ is called Schrödinger
operator with potential $q(x)$,and $\lambda$ is called eigenvalue of the
spectral problem \[sp1\] .

Our problem is to recover the potential $q(x)$ from scattering data,
which can be obtained from scattering experiments physically. In
general, take $\lambda=-k^2$, the scattering data includes refection
data $R(k)$ and transmission data $T(k)$,so that the solution to \[sp1\]
satisfy: $$\begin{aligned}
\psi(x,k) \rightarrow T(k)e^{-ikx}\,\,\, \text{as }x\rightarrow -\infty  \\
\psi(x,k) \rightarrow R(k)e^{ikx}\,\,\, \text{as }x\rightarrow \infty
\end{aligned}$$ The inverse scattering method requires some boundary
conditions as $x\rightarrow \pm\infty$,also since the equation \[sp1\]
is second order, so the solutions form a 2-dimensional complex vector
space and hence if $\varphi$ is solution to \[sp1\] so is
$\bar{\varphi}$, the complex conjugate, and they are linear independent.
Consider two bases of this complex vector space
$(\varphi(x,k),\bar{\varphi}(x,k)),(\psi(x,k),\bar\psi(x,k))$ which are
determined by: $$\begin{aligned}
\varphi(x,k)\sim e^{-ikx}&,x\rightarrow -\infty \\
\bar\varphi(x,k)\sim e^{ikx}&,x\rightarrow -\infty \\
\psi(x,k)\sim e^{-ikx}&,x\rightarrow \infty\\
\bar\psi(x,k)\sim e^{ikx}&,x\rightarrow \infty
\end{aligned}$$ And we can represent
$\varphi(x,k)=a(k)\psi(x,k)+b(k)\bar\psi(x,k)$

Appendix
========

Sturm-Liouville eigenvalue problem
----------------------------------

Let $p(x)>0,q(x)\geq 0,r(x)\geq 0$ in $I=(a,b),b>a$, and let
$u(x)\in C^2(I)\cap C^1(\bar{I})$ then the equations below:
$$\begin{aligned}
Lu(x)&=-\lambda r(x)u(x) \label{slevp}\\
u(a)&=h_0u'(a)\\
u(b)&=h_1u'(b)\end{aligned}$$ where
$L:={\ensuremath{\frac{\text{d}^{} }{\text{d} x}}}p(x){\ensuremath{\frac{\text{d}^{} }{\text{d} x}}}-q(x)$
and $h_0,h_1$ are constants. We called this problem as Sturm-Liouville
EigenValue Problem (**SLEVP**).

**Note:**$L$ is self-adjoint, i.e $L=L^*$

Also we consider following problem which is called Sturm-Liouville
Boundary Value problem(**SLBVP**) by changing \[slevp\] to
$$\label{slbvp}
Lu(x)=f(x)$$

Using Green’s function to solve some reduced SLEVP
--------------------------------------------------

In this section, we will consider a type of SLEVP with the form of
\[slbvp\].

If $G(x,a)$ solves $L_xG(x,a)=\delta(x-a)$,then the solution to equation
\[slbvp\] has the form: $$\label{slbvpsol}
u(x)=u_0(x)+\int_{a}^{b}G(x,a)f(a)\text{d}a$$ where $u_0(x)$ solve the
homogeneous equation $Lu(x)=0$

We only need to verify \[slbvp\], hence $$\begin{aligned}
Lu(x)&=L\big(u_0+\int_a^bG(x,a)f(a)\text{d}a\big)\\
&=0+\int_a^bf(a)L_xG(x,a)\text{d}a\\
&=\int_a^bf(a)\delta(x-a)\text{d}a\\
&=f(x)\end{aligned}$$

An Application of Green’s function
----------------------------------

Represent the following differential equation as integral equation:
$$\label{se}
m_{xx}(x)-2kim_x(x)=-p(x)m(x)$$ Also in order to get uniqueness, one
boundary value is prescribed: $$\label{boundarycondition}
m\rightarrow 1,x\rightarrow -\infty$$ Then apply the Green’s function
method, we represent \[se\] as: $$\label{integraleq}
m(x)=c_1+c_2e^{2kix}+\int_{-\infty}^{\infty}G(x-a)p(a)m(a)\text{d}a$$
where $G(x-a)$ solves the following differential equation:
$$G_{xx}-2kiG_x=-\delta(x-a)$$ and in \[integraleq\], $c_1+c_2e^{2ki}$
means the general solution of $$G_{xx}-2kiG_x=0$$ which is the
corresponding homogeneous equation of \[se\].

Moreover, applying the boundary condition \[boundarycondition\], we
obtain that $c_1=1,c_2=0$, if $\text{Im }k>0$. Since $m\rightarrow 1$ as
$x\rightarrow -\infty$, $c_2e^{-2kix}$
