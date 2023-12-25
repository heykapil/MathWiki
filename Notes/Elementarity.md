---
mathLink-blocks:
    Tarski-Vaught-test: Tarski-Vaught Test
---

<div class="topSpace"></div>

Date Created: 21/12/2023 14:38:27
Tags: #Type/Definition #Topic/Model_Theory

Types: <i>Not Applicable</i>
Examples: <i>Not Applicable</i>
Constructions: <i>Not Applicable</i>
Generalizations: <i>Not Applicable</i>

Properties: <i>Not Applicable</i>
Sufficiencies: [[Lowenheim-Skolem Theorem]]
Equivalences: <i>Not Applicable</i>
Justifications: <i>Not Applicable</i>

``` ad-Definition
title: Definition.

Two $\sigma$-structures $\mc{A}$ and $\mc{B}$ are <b>elementarily equivalent</b>, written $\mc{A}\elemequiv\mc{B}$, if $\Th\mc{A}=\Th\mc{B}$.
* We say that $\mc{A}$ <b>elementarily embeds</b> in $\mc{B}$, written $\mc{A}\into_e\mc{B}$, if there is a homomorphism $h:\mc{A}\to\mc{B}$ such that for all $\sigma$-formulas $\phi(\vec{v})$ and $\vec{a}\in A^{|\vec{v}|}$, we have $\mc{A}\models\phi(\vec{a})$ iff $\mc{B}\models\phi(h(\vec{a}))$. Such a homomorphism $h$ is said to be an <b>elementary embedding</b>, written $h:\mc{A}\into_e\mc{B}$.
* A substructure $\mc{A}\substructeq\mc{B}$ is said to be <b>elementary</b>, written $\mc{A}\elemembed\mc{B}$, if $\iota:\mc{A}\into_e\mc{B}$. In this case, we also say that $\mc{B}$ is an <b>elementary extension</b> of $\mc{A}$.

```

<b>Remark.</b> It follows by induction on the complexity of a $\sigma$-sentence that isomorphic structures are elementarily equivalent. If $\mc{A}\substructeq\mc{B}$ is a $\sigma$-substructure, then they agree on quantifier-free formulas, but for a general $\sigma$-formula $\phi(\vec{v})$, the best that we can say is that $\mc{B}\models\phi(\vec{a})$ implies $\mc{A}\models\phi(\vec{a})$ whenever $\phi$ is universal, and that $\mc{A}\models\phi(\vec{a})$ implies $\mc{B}\models\phi(\vec{a})$ whenever $\phi$ is existential. This motivates the notion of an <i>elementary</i> substructure, for which a useful criterion is the <i>Tarski-Vaught Test</i>, stating that $\mc{A}\elemembed\mc{B}$ iff for every $\sigma$-formula $\phi(\vec{x},y)$ and every $\vec{a}\in A^{|\vec{x}|}$, we have $\mc{B}\models\ex y\phi(\vec{a},y)$ iff there exists $a'\in A$ such that $\mc{B}\models\phi(\vec{a},a')$. That is, $\mc{A}\elemembed\mc{B}$ iff any $\sigma$-formula $\ex y\phi(\vec{a},y)$ can always be witnessed by some $a'\in A$. ^Tarski-Vaught-test
* Indeed, the forwards direction is trivial. For the backwards, let $\phi(\vec{x})$ be a $\sigma$-formula and take $\vec{a}\in A^{|\vec{x}|}$. We show that $\mc{A}\models\phi(\vec{a})$ iff $\mc{B}\models\phi(\vec{a})$ by induction on the complexity of $\phi$, for which the only non-trivial case is when $\phi(\vec{x})=\ex y\psi(\vec{x},y)$. But $\mc{B}\models\phi(\vec{a})$ iff $\mc{B}\models\ex y\psi(\vec{a},y)$, so the Tarski-Vaught condition furnishes a witness $a'\in A$ such that $\mc{B}\models\psi(\vec{a},a')$. That $\mc{A}\models\psi(\vec{a},a')$ holds by induction, so $\mc{A}\models\phi(\vec{a})$ as desired. The converse is trivial.

This test also gives us simple examples of $\sigma$-structures $\mc{A}\substructeq\mc{B}$ such that $\mc{A}\elemequiv\mc{B}$ that are <i>not</i> elementary. Indeed, let $\sigma\coloneqq\tpl{<}$ and consider the isomorphic $\sigma$-structures $\mc{A}\coloneqq\tpl{\N_{>0},<}$ and $\mc{B}\coloneqq\tpl{\N,<}$. Clearly $\mc{A}\elemequiv\mc{B}$, but the $\sigma$-formula $\phi(y)\coloneqq\lnot\ex z(z<y)$ is only witnessed by $0\not\in A$ in $\mc{B}$. In general, the failure of a $\sigma$-substructure to be elementary is the lack of those witnesses, called <i>Skolem witnesses</i>, which are used in the <i>Downward Löwenheim-Skolem Theorem</i> to build elementary substructures.<span style="float:right;">$\blacklozenge$</span>