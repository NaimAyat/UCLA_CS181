# Lecture 6: April 18, 2018
## Applications
* DFA and NFA to DFA
  * Token scanner for compiler
* Localization of software
  * Code-driven to data/table-driven
* Nodes in models (eg. UML)
* Representaion of patterns
  * Code to data
  * Executable representation
## Pumping Lemma
If A is a FSL over Σ, then ∃ an integer p ≥ 1 such that for all strings s in A, |s| ≥ p, ∃ x,y,z such that s=xyz and:

  1. ∀i xy<sup>i</sup>z ∈ A
  2. |y| > 0
  3. |xy| ≤ 0
