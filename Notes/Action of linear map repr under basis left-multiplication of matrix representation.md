---
mathLink: Action of linear map $\Leftrightarrow^\textrm{repr.}_\textrm{bases}$ left-multiplication of matrix representation
---

<div class="topSpace"></div>

Date Created: 19/05/2022 17:10:55
Tags: #Type/Proposition #Later/Module_Theory

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $V$ and $W$ be finite-dimensional $K$-vector spaces, say with $n\coloneqq\dim V$ and $m\coloneqq\dim W$, and fix two choices of bases $\mc{B}\coloneqq\l\{b_1,\dots,b_n\r\}$ and $\mc{C}\coloneqq\l\{c_1,\dots,c_m\r\}$ of $V$ and $W$, respectively. Then, for every linear map $T:V\to W$ and $v\in V$, we have $\l[T\l(v\r)\r]_\mc{C}=\l[T\r]_\mc{B}^\mc{C}\l[v\r]_\mc{B}$.

```

<b>Remark.</b> Letting $A\coloneqq\l[T\r]_\mc{B}^\mc{C}$, this relationship can be interpreted by saying that the diagram
![[Images/2022-05-29_220733/image.svg|170]]

commutes. Thus, after identifying $V\iso K^n$ and $W\iso K^m$ via the maps $\phi_\mc{B}$ and $\phi_\mc{C}$, respectively, we may identify $T$ with the left-multiplication map $L_A$. This is useful since it allows us to reduce abstract statements about $T$ to maps between tuple spaces.<span style="float:right;">$\blacklozenge$</span>

---

<b>Remark.</b> In particular, if $V=K^n$ and $W=K^m$ and $\mc{B}$ and $\mc{C}$ are the standard bases, then $T\l(\vec{v}\r)=\l[T\r]_\mc{B}^\mc{C}\vec{v}$.<span style="float:right;">$\blacklozenge$</span>

---

<i>Proof.</i> Fix $v\in V$. For any linear map $f:\dom f\to V$ (with $\dom f$ being an $\l|\mc{A}\r|$-dimensional vector space), we have that $\l[T\circ f\r]_\mc{A}^\mc{C}=\l[T\r]_\mc{B}^\mc{C}\l[f\r]_\mc{A}^\mc{B}$, so it suffices to find suitable $\dom f$, $\mc{A}$, and $f$ such that $\l[T\circ f\r]_\mc{A}^\mc{C}=\l[T\l(v\r)\r]_\mc{C}$ and $\l[f\r]_\mc{A}^\mc{B}=\l[v\r]_\mc{B}$. Observe that
$$\begin{equation}
    \l[T\circ f\r]_\mc{A}^\mc{C}\in\mat{m\times\l|\mc{A}\r|}{K}\ \ \ \ \ \ \ \ \textrm{and}\ \ \ \ \ \ \ \ \l[T\l(v\r)\r]_\mc{C}\in\mat{m\times1}{K},
\end{equation}$$
so we need $\l|\mc{A}\r|=1$; set $\mc{A}\coloneqq\l\{\alpha\r\}$ for some $\alpha\in\dom f$. Hence we have $\l[f\r]_\mc{A}^\mc{B}=\l[f\l(\alpha\r)\r]_\mc{B}$, so we need $f\l(\alpha\r)=v$. Indeed, a simple choice of $f$ is
$$\begin{equation}
    f:K\to V \ \ \ \ \ \ \ \ \textrm{mapping}\ \ \ \ \ \ \ \ k\mapsto v
\end{equation}$$
where $K$ is regarded as a vector space over itself; it is obviously linear. Observe that $\mc{A}=\l\{1\r\}$ is a basis for $K$, so
$$\begin{equation}
    \l[T\circ f\r]_\mc{A}^\mc{C}=\l[\l(T\circ f\r)\l(1\r)\r]_\mc{C}=\l[T\l(f\l(1\r)\r)\r]_\mc{C}=\l[T\l(v\r)\r]_\mc{C}.\qedin
\end{equation}$$
