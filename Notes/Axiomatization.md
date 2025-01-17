<div class="topSpace"></div>

Date Created: 05/02/2024 14:01:55
References: #Ref/Anu23 #Ref/Mar02
Tags: #Type/Definition #Topic/Logic/Model_Theory

Types: <i>Not Applicable</i>
Examples: [[Dense Linear Orders]]
Constructions: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

Properties: <i>Not Applicable</i>
Sufficiencies: <i>Not Applicable</i>
Equivalences: <i>Not Applicable</i>
Justifications: [[Completeness Theorem]], [[Compactness Theorem]]

``` ad-Definition
title: Definition (Axiomatization).

Let $\mc{L}$ be a language in $\FOL$ and let $T$ be an $\mc{L}$-theory. An <b>axiomatization</b> of $T$ is a collection $T_0$ of $\mc{L}$-sentences such that $T=\Cn T_0\coloneqq\l\{\phi\in\Sent\mc{L}\st T_0\proves\phi\r\}$, in which case we say that $T$ is <b>axiomatizable</b> by $T_0$.
* Given a collection $\mc{S}\subseteq\Sent\mc{L}$ of $\mc{L}$-sentences, we say that $T$ is <b>$\mc{S}$-axiomatizable</b> if $T$ is axiomatizable by sentences in $\mc{S}$.

```

<b>Remark.</b> Using the Completeness Theorem, we see that $T$ is axiomatizable by a subset $T_0\subset T$ occurs iff $\mc{A}\models T_0$ implies $\mc{A}\models T$ for every $\mc{L}$-structure $\mc{A}$. Indeed, if $T=\Cn(T_0)$ and $\mc{A}\models T_0$, then $T_0\proves\phi$ for any $\phi\in T$. By Soundness, we see that $T_0\models\phi$ for any $\phi\in T$, so $A\models T$. Conversely, suppose that $\phi\in T$ but $T\not\proves\phi$. Then $T_0\not\models\phi$ by Completeness, so there is some model $\mc{A}\models T_0$ such that $A\not\models\phi$. But $\mc{A}\models T$, a contradiction, so $T\subseteq\Cn(T_0)$. That $\Cn(T_0)\subseteq T$ is clear.
* A priori, a finite axiomatization $F$ of $T$ need not lie in $T$, but it is a consequence of the Compactness Theorem that such a witness $F_0\subseteq T$ can always be found. Indeed, write $F=\l\{\phi_1,\dots,\phi_n\r\}$ for some $\mc{L}$-sentences $\phi_i$, so $\mc{A}\models T$ iff $\mc{A}\models\phi_i$ for each $i$. In particular, we see that $T\models\phi_i$ for each $i$, so Compactness furnishes finite subtheories $T_i\subseteq T$ such that $T_i\models\phi_i$ for each $i$. The finite subtheory $F_0\coloneqq\bigcup_{i=1}^nT_i$ of $T$ is as desired.<span style="float:right;">$\blacklozenge$</span>
