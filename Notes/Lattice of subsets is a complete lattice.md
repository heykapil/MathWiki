<div class="topSpace"></div>

Date Created: 25/01/2022 18:38:44
Tags: #Type/Proposition #Topic/Set_Theory/Later

Proved by: [[Set ordered by inclusion is a poset]]
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $X$ be a set. Then the pair $\tpl{\pow\l(X\r),\subseteq}$ is a complete lattice.

```

<i>Proof.</i> Observe that $\tpl{\pow\l(X\r),\subseteq}$ is a poset, so it suffices to prove that every subset of $\pow\l(X\r)$ has both a join and a meet. To this end, take $\mc{Y}\subseteq\pow\l(X\r)$. We first prove the case for then $\mc{Y}=\em$. In this case, every $W\in\pow\l(X\r)$ is vacuously an upper and lower bound of $\mc{Y}$.
* For the join of $\em$, we need to find an upper bound that is a subset of every subset of $X$; simply take $\em$ itself.
* For the meet of $\em$, observe that every lower bound is a subset of $X$, so $X$ is the greatest such lower bound.

Assume now that $\mc{Y}\neq\em$.
* Recall that $\fa Y\in\mc{Y}:Y\subseteq\bigcup\mc{Y}$, so $\bigcup\mc{Y}$ is an upper bound of $\mc{Y}$. Furthermore, we have $\bigcup\mc{Y}\subseteq U$ for every $U\in\pow\l(X\r)$ such that $\fa Y\in\mc{Y}:Y\subseteq U$. To see this, take $W\in\bigcup\mc{Y}$, so there exists $Y\in\mc{Y}$ such that $W\in Y$. But $Y\subseteq U$, so $W\in U$ too.
* Recall that $\fa Y\in\mc{Y}:\bigcap\mc{Y}\subseteq Y$, so $\bigcap\mc{Y}$ is a lower bound of $\mc{Y}$. Furthermore, we have $U\subseteq\bigcap\mc{Y}$ for every $U\in\pow\l(X\r)$ such that $\fa Y\in\mc{Y}:U\subseteq Y$. To see this, take $W\in U$, so $W\in Y$ for all $Y\in\mc{Y}$ and thus $W\in\bigcap\mc{Y}$ by definition of the intersection.

Overall, we have
$$\begin{equation}
    \bigvee\mc{Y}=
        \begin{dcases}
            \em & \textrm{if }\mc{Y}=\em\\\ \\
            \bigcup\mc{Y} & \textrm{else}
        \end{dcases}\ \ \ \ \ \ \ \ \textrm{and}\ \ \ \ \ \ \ \ \bigwedge\mc{Y}=
        \begin{dcases}
            X & \textrm{if }\mc{Y}=\em\\\ \\
            \bigcap\mc{Y} & \textrm{else.}
        \end{dcases}\qedin
\end{equation}$$
