<div class="topSpace"></div>

Date Created: 11/01/2023 15:53:00
Tags: #Type/Proposition #Topic/Ring_Theory

Proved by: <i>Not Applicable</i>
References: [[Maximal implies prime]]
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $R$ be an integral domain and let $a\in R\comp\l\{0\r\}$. Then the following properties hold.
* $a$ is prime iff $\gen{a}$ is a prime ideal.
* $a$ is irreducible iff $\gen{a}$ is maximal in the set of all proper principal ideals of $R$.
* $a$ is prime implies $a$ is irreducible.

```

<b>Remark.</b> In particular, this proves that $a$ is prime iff $a$ is irreducible in a PID. The forwards direction always holds, so let $a$ be irreducible. Then $\gen{a}$ is maximal (since $R$ is a PID), so $\gen{a}$ is a prime ideal. Hence $a$ is prime.<span style="float:right;">$\blacklozenge$</span>

---

<i>Proof.</i>
* Observe that
$$\begin{equation}
    \begin{aligned}
        a\textrm{ is prime}&\Leftrightarrow a\not\in R^\times\land\fa b,c\in R:a\divides\!\l(bc\r)\Rightarrow\l(a\divides b\lor a\divides c\r) \\
        &\Leftrightarrow\gen{a}\neq R\land\fa b,c\in R:bc\in\gen{a}\Rightarrow\l(b\in\gen{a}\lor c\in\gen{a}\r) \\
        &\Leftrightarrow\gen{a}\textrm{ is a prime ideal}.
    \end{aligned}
\end{equation}$$

* For the forwards direction, say $b\in R$ is such that $\gen{a}\subseteq\gen{b}\subset R$. Since $\gen{a}\subseteq\gen{b}$, we see that $b\divides a$ and hence $a=bc$ for some $c\in R$. But $a$ is irreducible, so either $b\in R^\times$ or $c\in R^\times$. Note that $\gen{b}\neq R$, so $c\in R^\times$. Thus $a\sim b$, so $\gen{a}=\gen{b}$. Conversely, Take $b,c\in R$ such that $a=bc$. Then $b\divides a$, so $\gen{a}\subseteq\gen{b}$ and thus either $\gen{a}=\gen{b}$ or $\gen{b}=R$. In the latter case, $b\in R^\times$. In the former, we see that $a\sim b$ and hence $a=bu$ for some $u\in R^\times$. Then $bc=bu$, so $c=u\in R^\times$.
* Write $a=bc$ for some $b,c\in R$, so, since $a$ is prime, either $a\divides b$ or $a\divides c$. W.l.o.g., assume $a\divides b$, so $b=ad$ for some $d\in R$. Then $a=bc=acd$, so $cd=1$ and hence $c\in R^\times$.<span style="float:right;">$\blacksquare$</span>
