# Lecture 7: April 23, 2018
## Proof NFAs and DFAs Recognize the Same Set of Languages
* Given a DFA N, constuct a DFA M such that L(M) = L(N). Note: N = (Q, Σ, δ, q<sub>0</sub>, F), M = (𝒫(Q), Σ, δ, _, F) where 𝒫(Q) = all subsets of Q of N
  1. Remove ε-moves from N
  2. Transitive closure
  3. q ∈ Q
  4. E: Q → 𝒫(Q)
## Node and Mesh Analysis
