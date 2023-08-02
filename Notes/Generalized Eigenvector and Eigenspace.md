---
mathLink: auto
---

<div class="topSpace"></div>

Date Created: 16/03/2023 10:25:46
Tags: #Type/Definition #Topic/Module_Theory/Later

Types: <i>Not Applicable</i>
Examples: <i>Not Applicable</i>
Constructions: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

Properties: [[Generalized eigenspaces are disjoint]]
Sufficiencies: <i>Not Applicable</i>
Equivalences: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

``` ad-Definition
title: Definition.

Let $T:V\to V$ be a linear operator on a $K$-vector space $V$. For $\lambda\in K$, the subspace
$$\begin{equation}
    \hat{E}_\lambda\coloneqq\l\{v\in V\st\ex n\in\N^+:\l(\lambda\id_V-T\r)^nv=0\r\}
\end{equation}$$
is called the <b>generalized eigenspace of $T$ corresponding to $\lambda$</b>. A vector $v\in\hat{E}_\lambda$ is said to be a <b>generalized eigenvector of $T$ corresponding to $\lambda$</b>.

```

<b>Remark.</b> Clearly $E_\lambda\subseteq\hat{E}_\lambda$. Also, there are no ‘generalized eigenvalues’, since, if $\hat{E}_\lambda\neq\l\{0\r\}$, then $\lambda$ is an eigenvalue in the regular sense. Indeed, let $0\neq v\in\hat{E}_\lambda$, so there exists a smallest $n\in\N^+$ such that $\l(\lambda\id_V-T\r)^nv=0$. Then $0\neq v'\coloneqq\l(\lambda\id_V-T\r)^{n-1}v$, so $\l(\lambda-\id_VT\r)v'=0$. Thus $\lambda$ is an eigenvalue in the usual sense.<span style="float:right;">$\blacklozenge$</span>

---

<b>Remark.</b> We may further generalize the notion of an eigenspace of $T$. Indeed, for any $f\in K\l[x\r]$, let
$$\begin{equation}
    K_T^f\coloneqq\l\{v\in V\st f\l(T\r)v=0\r\}\ \ \ \ \ \ \ \ \textrm{and}\ \ \ \ \ \ \ \ \hat{K}_T^f\coloneqq\l\{v\in V\st\ex n\in\N^+:f\l(T\r)^nv=0\r\}
\end{equation}$$
be the <b>$f$-kernel of $T$</b> and <b>generalized $f$-kernel of $T$</b>, respectively. We then see that eigenspaces (generalized or not) are obtained by taking $f\l(T\r)\coloneqq\cchi_T$.<span style="float:right;">$\blacklozenge$</span>

---

<b>Remark.</b> It is clear that $\hat{K}_T^f$ is a subspace of $V$. To show that it is $T$-invariant, note that if $f\l(T\r)^nv=0$, then $f\l(T\r)^n\l(Tv\r)=T\l(f\l(T\r)^nv\r)=0$ where the first equality holds since $T$ commutes with all powers of $T$.<span style="float:right;">$\blacklozenge$</span>
