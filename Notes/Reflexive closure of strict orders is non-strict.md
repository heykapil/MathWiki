<div class="topSpace"></div>

Date Created: 01/02/2022 11:05:40
Tags: #Type/Proposition #Topic/Set_Theory/Later

Proved by: [[Reflexive closure of connected relation is connected]], [[Reflexive closure is the smallest reflexive relation]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $X$ be a set and let $\prec$ and $<$ be strict partial and total orders on $X$, respectively. Then $\preceq\,\coloneqq\rfcl\prec$ and $\leq\,\coloneqq\rfcl<$ are non-strict partial and total orders on $X$, respectively.

```

<i>Proof.</i> It suffices to show that $\preceq$ is a partial order on $X$ since the reflexive closure of connected relations remain connected. To do so, we check that $\preceq$ is transitive and antisymmetric on $X$; reflexivity is already ensured.
* (Transitive): Take $x_1,x_2,x_3\in X$ with such that $x_1\preceq x_2$ and $x_2\preceq x_3$. $If $x_1=x_2$ or $x_2=x_3$, then $x_1\preceq x_3$ by substitution.$. Otherwise, if $x_1\prec x_2$ and $x_2\prec x_3$, then $x_1\prec x_3$ since $\prec$ is transitive on $X$. It follows that $\tpl{x_1,x_3}\in\,\prec\,\subseteq\,\prec\cup\id_X=\rfcl\prec\,=\,\preceq.$
* (Antisymmetric): Take $x_1,x_2\in X$ such that $x_1\preceq x_2$ and $x_2\preceq x_1$. Observe that
$$\begin{equation}
    \begin{alignedat}{2}
        x_1\preceq x_2\land x_2\preceq x_1&\Leftrightarrow\l(x_1\prec x_2\land x_1=x_2\r)\land\l(x_2\prec x_1\lor x_1=x_2\r)\ \ \ \ \ \ \ \ &&\preceq\,=\rfcl\prec\,=\,\prec\cup\id_X\\
        &\Leftrightarrow x_1=x_2\lor\l(x_1\prec x_2\land x_2\prec x_1\r),&&\textrm{Distribution of }\lor\textrm{ over }\land
    \end{alignedat}
\end{equation}$$
but the latter case implies, from the transitivity of $\prec$ on $X$, that $x_1\prec x_1$. This contradicts the fact that $\prec$ is irreflexive of $X$, so $x_1=x_2$.<span style="float:right;">$\blacksquare$</span>
