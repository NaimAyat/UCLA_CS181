# Lecture 11: May 14, 2018
## This Week
* Pumping lemma for context-free languages
* Prove the set of all pushdown automata are equivalent to the set of all context-free grammars
* Deterministic pushdown automata
## Examples of Context-Free Languages
* {ww<sup>R</sup>} is context-free
* L = {ww} is not
  * L<sup>even</sup> = { xy | x ≠ y and |x| = |y| }
  * L<sup>c</sup> = L<sup>even</sup> ∪ { odd-length strings }
* Prove L<sup>c</sup> is a context-free language CFL. 
  1. Construct a simple DFA for odd-length strings (finite state languages are a subset of CFLs)
## Pumping Lemma for CFLs
* L CFL →	∃ p > 0 such that for all s ∈ L
  * |s| ≥ p
  * s = uvxyz for all i ≥ 0 uv<sup>i</sup>xy<sup>i</sup>z ∈ L
