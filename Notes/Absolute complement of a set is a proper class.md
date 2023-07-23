<div class="topSpace"></div>

Date Created: 18/01/2022 13:30:01
Tags: #Type/Proposition #Topic/Set_Theory/Later

Proved by: [[Russel's Paradox]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition (Informal).

Let $u$ be a set. The expression $\operatorname{comp}\l(u\r)\coloneqq\l\{x\st x\not\in u\r\}$ is a proper class.

```

<i>Proof.</i> Suppose, for sake of contradiction, that $\operatorname{comp}\l(u\r)$ is a set; in particular, $u\cup\operatorname{comp}\l(u\r)$ is also a set. Take any set $x$; we claim that $x\in u\cup\operatorname{comp}\l(u\r)$ and thus the union is in fact the universal class, contradicting the fact that the union of two sets is a set. This claim can be seen by the equivalences
$$\begin{equation}
    \begin{alignedat}{2}
        x\in u\cup\operatorname{comp}\l(u\r)&\Leftrightarrow x\in u\lor x\in\operatorname{comp}\l(u\r)\ \ \ \ \ \ \ \ &&\textrm{Definition of union}\\
        &\Leftrightarrow x\in u\lor x\not\in u,&&\textrm{Definition of absolute complement}
    \end{alignedat}
\end{equation}$$
where the last formula is always true, independently from $x$.<span style="float:right;">$\blacksquare$</span>
