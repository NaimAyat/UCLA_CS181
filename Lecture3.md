# Lecture 3: April 9, 2018
## Today
* Differential equations
* 1st and 2nd order circuits
* Impulse response and evaluation integral
## Deterministic Finite Automaton
* M = (Q, Σ, δ, q<sub>0</sub>, F) where:
  * Q = finite set (states)
  * Σ = finite set (alphabet)
  * q<sub>0</sub> ∈ Q = initial state
  * F ⊆ Q = the accepting state(s)
  * δ: Qx Σ → Q
    * δ(q, a) = q'. In state q on input a, go to state q'. Each move consumes one input symbol a.
## Language Concatenation
* Σ* indicates "all strings over Σ"
* Σ<sup>+</sup> "sequences of strings of length one or more over Σ (cannot just be empty string)"
* L<sub>1</sub> • L<sub>2</sub> = { xy | x ∈ L, & y ∈ L<sub>2</sub> }
  * L<sup>0</sup> = {ε}
  * L<sup>1</sup> = L
  * L<sup>n</sup> = L•L<sup>n-1</sup> n≥1 