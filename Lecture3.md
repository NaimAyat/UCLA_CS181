# Lecture 3: April 9, 2018
## Today
* Differential equations
* 1st and 2nd order circuits
* Impulse response and evaluation integral
## Language Concatenation
* Σ* indicates "all strings over Σ"
* Σ<sup>+</sup> "sequences of strings of length one or more over Σ (cannot just be empty string)"
* L<sub>1</sub> • L<sub>2</sub> = { xy | x ∈ L, & y ∈ L<sub>2</sub> }
  * L<sup>0</sup> = {ε}
  * L<sup>1</sup> = L
  * L<sup>n</sup> = L•L<sup>n-1</sup> n≥1 
## Deterministic Finite Automaton
* M = (Q, Σ, δ, q<sub>0</sub>, F) where:
  * Q = finite set (states)
  * Σ = finite set (alphabet)
  * q<sub>0</sub> ∈ Q = initial state
  * F ⊆ Q = the accepting state(s)
  * δ: Qx Σ → Q
    * δ(q, a) = q'. In state q on input a, go to state q'. Each move consumes one input symbol a.
* M = (Q, Σ, δ, q<sub>0</sub>, F) 
  * L(M)
  * If L is a finite state language (FSL), is ~L (Σ* - L) always an FSL? 
  * ~M = (Q, Σ, δ, q<sub>0</sub>, (Q-F))
## Closure PRoperties
* L<sub>1</sub> • L<sub>2</sub>
* L<sub>1</sub> ∪ L<sub>2</sub>
* L<sub>1</sub>* and L<sub>1</sub><sup>+</sup> (Kleene star and Kleene plus)
* L<sub>1</sub> ∩ L<sub>2</sub>
* L<sub>1</sub><sup>R</sup>
* Homomorphism: any function h: Σ → Σ*
  * Ex: for the language L = { w | x y; x = a<sup>n</sup>; y = b<sup>n</sup>; n ≥ 0} 
    * h(a) = ε, h(b) = ε
      * h(aaabbb) = εεεεεε = ε
    * h(a) = a, h(b) = a
      * h(L) = {a<sup>2n</sup>}
