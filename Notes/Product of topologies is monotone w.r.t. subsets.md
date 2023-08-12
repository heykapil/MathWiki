<div class="topSpace"></div>

Date Created: 11/02/2022 11:24:27
Tags: #Type/Proposition #Topic/Topology/Later

Proved by: [[Product topology (basis; component from bases)]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $\mc{T}_1$ and $\mc{T}_2$ be topologies on a set $X$ and let $\mc{O}_1$ and $\mc{O}_2$ be topologies on a set $Y$. Then
$$\begin{equation}
    \mc{T}_1\subseteq\mc{T}_2\land\mc{O}_1\subseteq\mc{O}_2\ \ \ \ \Leftrightarrow\ \ \ \ \mc{T}_1\times\mc{O}_1\subseteq\mc{T}_2\times\mc{O}_2.
\end{equation}$$

```

<i>Proof.</i> Let $\mc{B}_1,\mc{B}_2,\mc{C}_1,\mc{C}_2,\pow _1,\pow _2$ be bases for the topologies $\mc{T}_1$, $\mc{T}_2$, $\mc{O}_1$, $\mc{O}_2$, $\mc{T}_1\times\mc{O}_1$, and $\mc{T}_2\times\mc{O}_2$, respectively.
* ($\Rightarrow$): Take $p\in X\times Y$ and $P_1\in\pow _1$ containing $p$, so there exist $x\in X$ and $y\in Y$ such that $p=\tpl{x,y}$, and there exist $B_1\in\mc{B}_1$ and $C_1\in\mc{C}_1$ such that $P_1=B_1\times C_1$. Since $\mc{T}_1\subseteq\mc{T}_2$, there exists $B_2\in\mc{B}_2$ such that $x\in B_2\subseteq B_1$. Similarly, since $\mc{O}_1\subseteq\mc{O}_2$, there exists $C_2\in\mc{C}_2$ such that $y\in C_2\subseteq C_1$. Set $P_2\coloneqq B_2\times C_2$ from which it follows that $p=\tpl{x,y}\in P_2\subseteq P_1$. The result follows.
* ($\Leftarrow$): Take $B_1\in\mc{B}_1$ and $C_1\in\mc{C}_1$ containing $x\in X$ and $y\in Y$, respectively. Then $\tpl{x,y}\in B_1\times C_1\in\pow _1$, so, by hypothesis, there exists $P_2\in\pow _2$ such that $\tpl{x,y}\in P_2\subseteq B_1\times C_1$. Since there exist $B_2\in\mc{B}_2$ and $C_2\in\mc{C}_2$ such that $P_2=B_2\times C_2$, we have that $\tpl{x,y}\in B_2\times C_2\subseteq B_1\times C_1$. Observe that $B_2,C_2\neq\em$, so we have $x\in B_2\subseteq B_1$ and $y\in C_2\subseteq C_1$. The result follows.<span style="float:right;">$\blacksquare$</span>
