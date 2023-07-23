<div class="topSpace"></div>

Date Created: 20/01/2022 13:14:26
Tags: #Type/Proposition #Topic/Set_Theory/Later

Proved by: [[Replacement image of a set is a set]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: [[Cartesian product is a set (Kuratowski)]]
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $X$ and $Y$ be sets. Then there exists a unique set $z$ whose elements are exactly the sets $u$ for which there exists $x$ in $X$ and $y$ in $Y$ such that $u=\tpl{x,y}$. Formally,
$$\begin{equation}
    \fa X\fa Y\ex!z\l[u\in z\Leftrightarrow\ex x\in X,\ex y\in Y:u=\tpl{x,y}\r].
\end{equation}$$

```

<b>Remark.</b> Note that this proof does not rely on the specific Kuratowski definition of the ordered pair.<span style="float:right;">$\blacklozenge$</span>

---

<i>Proof.</i> This proof consists of three steps:
1. Fix $s\in X$. We shall construct the set
$$\begin{equation}
    \l\{s\r\}\times Y\coloneqq\l\{v\st\ex y\in Y:v=\tpl{x,y}\r\}.
\end{equation}$$
To do so, let $\phi\l(y,v\r)\Leftrightarrow v=\tpl{s,y}$; we wish to prove that $\fa y\in Y:\ex!v:v=\tpl{s,y}$. But this is trivial; certainly such a set exists, and it is unique because if there exist some other $v'$ such that $v'=\tpl{s,y}$, then $v'=v$. Thus we can form the replacement image of $Y$ under $\phi\l(y,v\r)$, which is precisely the set $\l\{s\r\}\times Y$.

2. Using the same technique, we shall construct the set
$$\begin{equation}
    \l\{\l\{x\r\}\times Y\st x\in X\r\}\coloneqq\l\{w\st\ex x\in X:w=\l\{x\r\}\times Y\r\}.
\end{equation}$$
To do so, let $\psi\l(x,w\r)\Leftrightarrow w=\l\{x\r\}\times Y$; we wish to prove that $\fa x\in X,\ex!w:w=\l\{x\r\}\times Y$. Again, this is trivial. Therefore, we can form the replacement image of $X$ under $\psi\l(x,w\r)$, which is precisely the set $\l\{\l\{x\r\}\times Y\st x\in X\r\}$.
3. Consider the set $z\coloneqq\bigcup\l\{\l\{x\r\}\times Y\st x\in X\r\}$. The result follows from the following chain of equivalences:

$\begin{alignat}{2}
    u\in z&\Leftrightarrow u\in\bigcup\l\{\l\{x\r\}\times Y\st x\in X\r\}&&\textrm{Definition of }z\\
    &\Leftrightarrow\ex w\in\l\{\l\{x\r\}\times Y\st x\in X\r\}:u\in w\ \ \ \ \ \ \ \ &&\textrm{Definition of union}\\
    &\Leftrightarrow\ex x\in X:w=\l\{x\r\}\times Y\land u\in w&&\textrm{Definition of }\l\{\l\{x\r\}\times Y\st x\in X\r\}\\
    &\Leftrightarrow\ex x\in X:u\in\l\{x\r\}\times Y&&\textrm{Substitution}\\
    &\Leftrightarrow\ex x\in X,\ex y\in Y:u=\tpl{x,y}.&&\textrm{Definition of }\l\{x\r\}\times Y\qedin
\end{alignat}$
