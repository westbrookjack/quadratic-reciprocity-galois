# A Proof of Quadratic Reciprocity by Galois Theory

This note presents a modern proof of **quadratic reciprocity** using Galois theory and basic algebraic number theory.  
Written by **Jack Westbrook**, with guidance and discussion from **Prof. Ana Caraiani** (Imperial College London).

📄 **PDF:** [`Quadratic_Reciprocity_by_Galois_Theory.pdf`](Quadratic_Reciprocity_by_Galois_Theory.pdf)

---

## Overview

Quadratic reciprocity is one of the central results in number theory, describing a symmetry in quadratic residues between distinct primes:

$$
\left(\frac{q}{p}\right)
= (-1)^{\frac{p-1}{2}\frac{q-1}{2}}
\left(\frac{p}{q}\right).
$$

This exposition derives the result **purely through Galois-theoretic reasoning**, by studying the relationship between the Galois groups of cyclotomic and quadratic extensions.

---

## Main Idea

Let $p$ be an odd prime and $\zeta_p$ a primitive $p$-th root of unity.  
Key ingredients:

1. **Cyclotomic and quadratic fields.**  
   The Galois group $\mathrm{Gal}(\Bbb Q(\zeta_p)/\Bbb Q)\cong(\Bbb Z/p\Bbb Z)^\times$ has a unique index-2 subgroup corresponding to the quadratic subfield $\Bbb Q(\sqrt{\hat p})$, where $\hat p=(-1)^{(p-1)/2}p$.

2. **Frobenius elements and splitting.**  
   The Frobenius $\mathrm{Frob}_q$ acts by $\zeta_p\mapsto\zeta_p^{\,q}$.  
   Restricting $\mathrm{Frob}_q$ to the quadratic subfield links
   $\mathrm{Gal}(\Bbb Q(\zeta_p)/\Bbb Q)\to\mathrm{Gal}(\Bbb Q(\sqrt{\hat p})/\Bbb Q)$
   with the Legendre symbols $\big(\frac{q}{p}\big)$ and $\big(\frac{\hat p}{q}\big)$.

3. **Commutativity implies reciprocity.**  
   Comparing these maps yields
   $\big(\frac{q}{p}\big)=\big(\frac{\hat p}{q}\big)=(-1)^{\frac{p-1}{2}\frac{q-1}{2}}\big(\frac{p}{q}\big)$.

The supplementary laws follow by computing Frobenius at $2$:

$$
\left(\frac{2}{p}\right)=
\begin{array}{ll}
1,& p\equiv\pm1\pmod8,\\
-1,& p\equiv\pm3\pmod8,
\end{array}
\qquad
\left(\frac{-1}{p}\right)=(-1)^{\frac{p-1}{2}}.
$$



---

## Reference
- J. S. Milne, *Algebraic Number Theory* (course notes), https://www.jmilne.org/math/CourseNotes/ANT.pdf

*Written October 2025.*
