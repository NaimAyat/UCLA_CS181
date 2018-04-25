# Lecture 8: April 25, 2018
## Today
1. Uses of pumping lemma
2. Context free grammars and languages
3. GNFA conversion to regular expressions
## Pumping Lemma
* For any FSL, L:
  * ∃ p such that 
  * ∀ w ∈ L and |w| ≥ p
  * ∃ xyz = w such that: ∀ i ≥ 0, xy<sup>i</sup>z ∈ L; |xy| ≤ p; |y| ≥ 1
### Example
* Let L = { w ∈ Σ<sup>+</sup> | w contains balanced parentheses }, Σ = { (, ) }
  * Proof of irregularity: let w = (<sup>p</sup>)<sup>p</sup>
    * Cases for xyz:
       1. |xy| = p
         * x and y must consist completely of ( characters, while z must consist entirely of z characters
         * Hence, w' = (<sup>|x|</sup>ε)<sup>|z|</sup> for i = 0 should be in L, which is a contradiction
       2. |xy| < p