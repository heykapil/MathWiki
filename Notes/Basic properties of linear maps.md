<div class="topSpace"></div>

Date Created: 27/12/2022 17:35:44
Tags: #Type/Proposition #Topic/Linear_Algebra

Proved by: <i>Not Applicable</i>
References: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

Specializations: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

``` ad-Proposition
title: Proposition.

Let $V_1$ and $V_2$ be $K$-vector spaces and consider a linear map $T:V_1\to V_2$. Let $W_1\subseteq V_1$ and $W_2\subseteq V_2$ be linear subspaces. Then the following properties hold.
* (Image preserve subspaces): $\im_T\l(W_1\r)\subseteq V_2$ is a subspace.
* (Preimage preserve subspace): $\preim_T\l(W_2\r)\subseteq V_1$ is a subspace.
* (Inverse preserve linearity): If $T$ is invertible, then $T^{-1}:V_2\to V_1$ is a linear map.

```

<b>Remark.</b> In particular, $\im T\subseteq V_2$ and $\ker T\subseteq V_1$ are subspaces.<span style="float:right;">$\blacklozenge$</span>

---

<i>Proof.</i>
* Since $T\l(0\r)=0$, we see that $0\in W_1$. Take $\alpha\in K$ and $w_2,w_2'\in\im_T\l(W_2\r)$, so there exist $w_1,w_1'\in W_1$ such that $T\l(w_1\r)=w_2$ and $T\l(w_1'\r)=w_2'$. Observe then that
$$\begin{equation}
    \alpha w_2+w_2'=\alpha\l(T\l(w_1\r)\r)+T\l(w_1'\r)=T\l(\alpha w_1\r)+T\l(w_1'\r)=T\l(\alpha w_1+w_1'\r),
\end{equation}$$
so $\alpha w_2+w_2'\in\im_T\l(W_1\r)$.

* Similarly, we see that $0\in\preim_T\l(W_2\r)$. Take $\alpha\in K$ and $w_1,w_1'\in\preim_T\l(W_2\r)$, so there exist $w_2,w_2'\in W_2$ such that $T\l(w_1\r)=w_2$ and $T\l(w_1'\r)=w_2'$. Observe then that
    $$\begin{equation}
        T\l(\alpha w_1+w_1'\r)=T\l(\alpha w_1\r)+T\l(w_1'\r)=\alpha T\l(w_1\r)+T\l(w_1'\r)=\alpha w_2+w_2'\in W_2,
    \end{equation}$$
so $\alpha w_1+w_1'\in\preim_T\l(W_2\r)$.
* (Inverse preserve linearity): Take $\alpha\in K$ and $v_2,v_2'\in V_2$, and set $v_1\coloneqq T^{-1}\l(v_2\r)$ and $v_1'\coloneqq T^{-1}\l(v_2'\r)$. Observe then that
$$\begin{equation}
    T^{-1}\l(\alpha v_2+v_2'\r)=T^{-1}\l(\alpha T\l(v_1\r)+T\l(v_1'\r)\r)=T^{-1}\l(T\l(\alpha v_1+v_1'\r)\r)=\alpha v_1+v_1'=\alpha T^{-1}\l(v_2\r)+T^{-1}\l(v_2'\r).\qedin
\end{equation}$$
