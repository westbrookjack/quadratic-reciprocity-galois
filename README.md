# A Proof of Quadratic Reciprocity by Galois Theory

This note presents a modern proof of **quadratic reciprocity** using Galois theory and basic algebraic number theory.  
It was written by **Jack Westbrook**, with guidance and discussion from **Prof. Ana Caraiani** (Imperial College London).

📄 **PDF:** [`Quadratic_Reciprocity_by_Galois_Theory.pdf`](Quadratic_Reciprocity_by_Galois_Theory.pdf)

---

## Overview

Quadratic reciprocity is one of the central results in number theory, describing a remarkable symmetry in quadratic residues between distinct primes:

\[
\left(\frac{q}{p}\right)
= (-1)^{\frac{p-1}{2}\frac{q-1}{2}}
\left(\frac{p}{q}\right).
\]

This exposition derives the result **purely through Galois-theoretic reasoning**, by studying the relationship between the Galois groups of cyclotomic and quadratic extensions.

---

## Main Idea

Let \( p \) be an odd prime and \( \zeta_p \) a primitive \( p \)-th root of unity.  
The key ingredients of the proof are:

1. **Cyclotomic and quadratic fields.**  
   The Galois group \( \mathrm{Gal}(\mathbb{Q}(\zeta_p)/\mathbb{Q}) \cong (\mathbb{Z}/p\mathbb{Z})^\times \) has a unique index-2 subgroup corresponding to the quadratic subfield \( \mathbb{Q}(\sqrt{p̂}) \), where \( p̂ = (-1)^{\frac{p-1}{2}}p \).

2. **Frobenius elements and splitting behavior.**  
   The Frobenius automorphism \( \mathrm{Frob}_q \) acts as \( \zeta_p \mapsto \zeta_p^q \).  
   Tracking how \( \mathrm{Frob}_q \) restricts to the quadratic subfield yields a commutative diagram linking  
   \[
   \mathrm{Gal}(\mathbb{Q}(\zeta_p)/\mathbb{Q}) \longrightarrow \mathrm{Gal}(\mathbb{Q}(\sqrt{p̂})/\mathbb{Q})
   \]
   with the Legendre symbols \( \left(\frac{q}{p}\right) \) and \( \left(\frac{p̂}{q}\right) \).

3. **Commutativity implies reciprocity.**  
   Comparing these maps produces
   \[
   \left(\frac{q}{p}\right) = \left(\frac{p̂}{q}\right)
   = (-1)^{\frac{p-1}{2}\frac{q-1}{2}}\left(\frac{p}{q}\right),
   \]
   which is the law of quadratic reciprocity.

The argument concludes by computing the Frobenius at 2 to obtain the supplementary laws:
\[
\left(\frac{2}{p}\right) =
\begin{cases}
1, & p \equiv \pm1 \pmod{8},\\
-1, & p \equiv \pm3 \pmod{8},
\end{cases}
\quad
\left(\frac{-1}{p}\right) = (-1)^{\frac{p-1}{2}}.
\]

---

## References

- J. S. Milne, *Algebraic Number Theory* — Course Notes.  
  [https://www.jmilne.org/math/CourseNotes/ANT.pdf](https://www.jmilne.org/math/CourseNotes/ANT.pdf)

---

*Written October 2025.*
