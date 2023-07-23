<div class="topSpace"></div>

Date Created: 23/01/2022 21:01:35
Tags: #Type/Proposition #Topic/Topology/Later

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $\tpl{X,\mc{T}}$ be a topological space and fix $Y\subseteq X$. Suppose that for each $y\in Y$ there exists an open set $U\in\mc{T}$ containing $y$ such that $U\subseteq Y$. Then $Y\in\mc{T}$. Formally,
$$\begin{equation}
    \l(\fa y\in Y,\ex U\in\mc{T}:y\in U\land U\subseteq Y\r)\Rightarrow Y\in\mc{T}.
\end{equation}$$

```

<i>Proof.</i> For all $y\in Y$, let $U_y$ by any open set satisfying the hypothesis. We claim that $Y=\bigcup_{y\in Y}U_y$; since each $U_y$ is open, we see that $Y$ is open too.
* ($Y\subseteq\bigcup_{y\in Y}U_y$): Take $y_0\in Y$, so, by hypothesis, there exists an open set $U_{y_0}$ such that $y_0\in U_{y_0}$. Thus the forward inclusion holds by definition of the union.
* ($\bigcup_{y\in Y}U_y\subseteq Y$): Take $y_0\in\bigcup_{y\in Y}U_y$, so there exists $y\in Y$ such that $y_0\in U_y$. Since $U_y\subseteq Y$, we see that $y_0\in Y$.<span style="float:right;">$\blacksquare$</span>
