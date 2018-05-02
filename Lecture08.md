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
          * Hence, w' = (<sup>|x|</sup>ε)<sup>|z|</sup> for i = 0 should be in L; we have reached a contradiction
       2. |xy| < p
          * x and y must contain completely ( characters, while z must contain both ( and ) characters
          * Hence, w = (<sup>|x+y|</sup>(<sup>n</sup>)<sup>p</sup> for some n. Therefore, w' = p - |x| - |y|. We have reached a contradiction
## Contex-Free Grammars
* G = ( V, Σ, R, S )
  * V = finite set of variables
  * Σ = alphabet, a.k.a. "terminals"
  * R = finite set of rewriting rules
  * S ∈ V = start variable
* Ambigious grammar: more than one parse tree to generate the same string (or more than one left-most derivation, or more than one right-most derivation)
### Example
* Balanced parentheses grammar: 
  * V = {S}
  * Σ = { (, ) }
  * R = 
    ```
    { S → SS
      S → (S)
      S → ()  }
    ```
* Left-most derivation of (())()():
  * S → SS → SSS → (S)SS → (())SS → (())()S → (())()()
## Parse Tree vs. Derivation Tree
* "Parse tree" implies starting at the string and working up to start symbol
* "Derivation tree" implies starting at start symbol and working down to string
