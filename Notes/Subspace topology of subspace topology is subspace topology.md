<div class="topSpace"></div>

Date Created: 11/02/2022 18:25:41
Tags: #Type/Proposition #Topic/Topology/Later

Proved by: [[Subspace topology (basis)]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $\tpl{X,\mc{T}}$ be a topological space and let $\tpl{Y,\l.\mc{T}\r|_Y}$ be a subspace thereof. Then for every $Z\subseteq Y$, we have $\l.\l.\mc{T}\r|_Y\r|_Z=\l.\mc{T}\r|_Z$.

```

<i>Proof.</i> It suffices to show that their respective bases $\l.\l.\mc{B}\r|_Y\r|_Z$ and $\l.\mc{B}\r|_Z$ coincide.
* ($\l.\l.\mc{B}\r|_Y\r|_Z\subseteq\l.\mc{B}\r|_Z$). Take $D\in\l.\l.\mc{B}\r|_Y\r|_Z$, so there exists $C\in\l.\mc{B}\r|_Y$ such that $D=C\cap Z$. Similarly, there exists $B\in\mc{B}$ such that $C=B\cap Y$. Observe then that
$$\begin{equation}
    \begin{alignedat}{2}
        D&=\l(B\cap Y\r)\cap Z\ \ \ \ \ \ \ \ &&\textrm{Substitution}\\
        &=B\cap\l(Y\cap Z\r)&&\textrm{Associativity of intersection}\\
        &=B\cap Z&&Z\subseteq Y\\
        &\in\l.\mc{B}\r|_Z.&&\textrm{Definition of }\l.\mc{B}\r|_Z
    \end{alignedat}
\end{equation}$$
* ($\l.\mc{B}\r|_Z\subseteq\l.\l.\mc{B}\r|_Y\r|_Z$). Take $D\in\l.\mc{B}\r|_Z$, so there exists $B\in\mc{B}$ such that $D=B\cap Z$. Observe that
$$\begin{equation}
    \begin{alignedat}{2}
        D=B\cap Z&=B\cap\l(Y\cap Z\r)\ \ \ \ \ \ \ \ &&Z\subseteq Y\\
        &=\l(B\cap Y\r)\cap Z,&&\textrm{Associativity of intersection}
    \end{alignedat}
\end{equation}$$
so set $C\coloneqq B\cap Y\in\l.\mc{B}\r|_Y$ from which we see that $D=C\cap Z\in\l.\l.\mc{B}\r|_Y\r|_Z$.<span style="float:right;">$\blacksquare$</span>
