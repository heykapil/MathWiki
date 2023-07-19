---
mathLink: $T$ diagonalizable $\Rightarrow$ $\cchi_T$ splits
---

<div class="topSpace"></div>

Date Created: 08/03/2023 16:43:04
Tags: #Type/Proposition #Later/Module_Theory

Proved by: [[Leibniz Formula]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $V$ be a finite-dimensional $K$-vector space and consider a linear operator $T:V\to V$. If $D\coloneqq\l[T\r]_\mc{B}=\diag\l(\lambda_1,\dots,\lambda_n\r)$ for some basis $\mc{B}$ of $V$, then
$$\begin{equation}
    \cchi_T\!\l(\lambda\r)=\prod_{i=1}^{n}\l(\lambda-\lambda_i\r).
\end{equation}$$

```

<i>Proof.</i> We shall prove that $\cchi_D\!\l(\lambda\r)=\prod_{i=1}^{n}\l(\lambda-\lambda_i\r)$, from which the result follows since $\cchi_T\!\l(\lambda\r)=\det\l(\lambda\id_V-T\r)=\det\l(\lambda I-D\r)=\cchi_D\!\l(\lambda\r)$.
* Let $D'\coloneqq\diag\l(\lambda-\lambda_1,\dots,\lambda-\lambda_n\r)$. By the Leibniz formula for determinants, we see that
$$\begin{equation}
    \cchi_D\!\l(\lambda\r)=\det\l(\lambda I-D\r)=\det D'=\sum_{\sigma\in S_n}\sgn\l(\sigma\r)d'_{\sigma\l(1\r)1}\cdots d'_{\sigma\l(n\r)n}.
\end{equation}$$
But every $\sigma\neq\id_{S_n}$ is such that $\sigma\l(i\r)=j$ for some $i\neq j$, in which case $d'_{\sigma\l(i\r)i}=0$. Thus the only non-zero term in the sum is occurs when $\sigma=\id_{S_n}$, so
$$\begin{equation}
    \cchi_D\!\l(\lambda\r)=\prod_{i=1}^{n}d'_{ii}=\prod_{i=1}^{n}\l(\lambda-\lambda_i\r).\qedin
\end{equation}$$
