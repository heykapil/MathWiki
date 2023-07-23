<div class="topSpace"></div>

Date Created: 21/02/2022 19:26:38
Tags: #Type/Proposition #Topic/Category_Theory/Later

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $\tpl{X,\leq}$ be a preordered set. Then the preorder category $\cat{C}\tpl{X,\leq}$ it includes is a category.

```

<i>Proof.</i> We first need to check that the composition is closed; that is, if $f\in\Hom\l(x,y\r)$ and $g\in\Hom\l(y,z\r)$ for $x,y,z\in X$, then $g\circ f\in\Hom\l(x,z\r)$. This statement is vacuously true if $x\not\leq y$ or $y\not\leq z$, so assume otherwise and thus $f=\tpl{x,y}$ and $g=\tpl{y,z}$. Since $\leq$ is transitive on $X$, we see that $x\leq z$ from which it follows that $\Hom\l(x,z\r)=\l\{\tpl{x,z}\r\}$. Observe then that $g\circ f\coloneqq\tpl{x,z}\in\Hom\l(x,z\r)$. Furthermore, for all $x\in X$, the morphism $\id_x$ is indeed in $\Hom\l(x,x\r)$ since $\leq$ is reflexive.

We now verify the axioms of a category.
* ($\axicat[1]$): Take $x,y,z,w\in X$ and consider morphisms $f\in\Hom\l(x,y\r)$, $g\in\Hom\l(y,z\r)$, and $h\in\Hom\l(z,w\r)$. It follows that $g\circ f\in\Hom\l(x,z\r)$ and $h\circ g\in\Hom\l(y,w\r)$, and, similarly, that$$\begin{equation}
        h\circ\l(g\circ f\r)\in\Hom\l(x,w\r)\ \ \ \ \textrm{and}\ \ \ \ \l(h\circ g\r)\circ f\in\Hom\l(x,w\r).
    \end{equation}$$
Since $\Hom\l(x,w\r)=\l\{\tpl{x,w}\r\}$ is a singleton, the two morphisms must coincide.

* ($\axicat[2]$): Take $x,y\in X$ and a morphism $f\in\Hom\l(x,y\r)$, so $f=\tpl{x,y}$. Since $\id_x\coloneqq\tpl{x,x}$ and $\id_y\coloneqq\tpl{y,y}$, we see that
$$\begin{equation}
    f\circ\id_x=\tpl{x,y}\circ\tpl{x,x}=\tpl{x,y}\ \ \ \ \textrm{and}\ \ \ \ \id_y\circ f=\tpl{y,y}\circ\tpl{x,y}=\tpl{x,y}
\end{equation}$$
by definition of the composition. Since $\Hom\l(x,y\r)=\l\{\tpl{x,y}\r\}$ is a singleton, both must coincide with $\tpl{x,y}=f$.<span style="float:right;">$\blacksquare$</span> 
