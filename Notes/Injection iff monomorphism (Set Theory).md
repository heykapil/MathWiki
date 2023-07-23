---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 20/02/2022 19:16:39
Tags: #Type/Proposition #Topic/Category_Theory/Later

Proved by: [[Left-invertible iff injection]], [[Left-invertible implies monomorphism]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Consider the category $\catset$ and let $f:X\to Y$ be a function. Then $f$ is an injection iff $f$ is a monomorphism.

```

<i>Proof.</i> ($\Rightarrow$): The forward direction is proven since, being an injection, $f$ has a left-inverse.

($\Leftarrow$): Let $Z$ be a singleton; that is, let $Z\coloneqq\l\{z\r\}$ for some set $z$. Take $x_1,x_2\in X$ and define the functions
$$\begin{equation}
    \alpha_1,\alpha_2:Z\to X\ \ \ \ \textrm{mapping}\ \ \ \ \alpha_1\l(z\r)\coloneqq x_1\ \ \ \ \textrm{and}\ \ \ \ \alpha_2\l(z\r)\coloneqq x_2.
\end{equation}$$
Observe then that

$\begin{alignat}{2}
    f\circ\alpha_1=f\circ\alpha_2\ \ \ \ &\Rightarrow\ \ \ \ \alpha_1=\alpha_2&&f\textrm{ is a monomorphism}\\
    \l(f\circ\alpha_1\r)\l(z\r)=\l(f\circ\alpha_2\r)\l(z\r)\ \ \ \ &\Rightarrow\ \ \ \ \alpha_1\l(z\r)=\alpha_2\l(z\r)\ \ \ \ \ \ \ \ &&z\in Z\\
    f\l(\alpha_1\l(z\r)\r)=f\l(\alpha_2\l(z\r)\r)\ \ \ \ &\Rightarrow\ \ \ \ x_1=x_2&&\textrm{Composition of functions; substitution}\\
    f\l(x_1\r)=f\l(x_2\r)\ \ \ \ &\Rightarrow\ \ \ \ x_1=x_2.&&\textrm{Substitution}\qedin
\end{alignat}$
