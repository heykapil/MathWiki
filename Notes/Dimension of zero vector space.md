<br />
<br />

Date Created: 06/04/2022 22:04:49
Tags: #Proposition #Closed

Proved by: [[Linearly independent subset cannot contain the zero vector]]
Generalizations: _Not Applicable_

Counterexamples: _Not Applicable_

``` ad-Proposition
title: Proposition.

_Let $K$ be a field and consider the zero vector space $\l\{0\r\}$ over $K$. Then $\dim\l\{0\r\}=0$._

```

_Proof_. It suffices to find a basis for $\l\{0\r\}$, but since $\l\{0\r\}$ contains only the zero vector $0$ and any linearly independent set cannot contain $0$, we see that there are no non-empty bases for $\l\{0\r\}$. The only option then is the empty set $\em$, which we observe is trivially linearly independent and has cardinality $\l|\em\r|=0$. To see that $\span\l(\em\r)=\l\{0\r\}$, observe that
$$\begin{align}
    \span\l(\em\r)&=\bigcup\l\{U\subseteq\l\{0\r\}\mid\em\subseteq U\land U\textrm{ is a linear subspace of }\l\{0\r\}\r\} && \textrm{Definition of linear span} \\
    &=\bigcup\l\{U\subseteq\l\{0\r\}\mid U\textrm{ is a linear subspace of }\l\{0\r\}\r\} && \em\subseteq U\textrm{ vacuously} \\
    &=\bigcup\l\{\l\{0\r\}\r\} && \textrm{The only subspaces of $\l\{0\r\}$ are trivial subspaces} \\
    &=\l\{0\r\}. && \textrm{Definition of union}\qedin
\end{align}$$