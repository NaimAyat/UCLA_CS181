# Lecture 1: April 2, 2018
## Logistics
* Midterm and final rooms TBD
* Office: Boelter 3531C after class (MW 6:15pm - TBD)
* Homework due Mondays 3:00pm in Box A1 "CS 181", Boelter 2432 
### Today
* Preliminaries
* Motivations
* Informal intro to automata theory
* Math foundations
## Course Overview
* In order from least to greatest expressive power and greatest to least predictability:
  * Deterministic finite automaton (DFA)
  * Deterministic pushdown automaton (DPDA)
  * Pushdown automaton (PDA)
  * Turing Machine (TM)
## Terminology
* ∪
* ∩
* s̅ ("s bar" with respect to some universal set)
* S-T (set difference)
* 2<sup>S</sup> or 𝒫(S) (power set)
* Cardinality, finite, infinite
  * Infinite: countable or uncountable?
* Relationships: =, ≠, ⊆, ⊂, ⊄
* Ordered pairs
* Cartesian product: x
  * R x S x T ≠ R x (S x T) ≠ (R x S) x T
* Graphs: (V, E)
  * Verticies, edges
  * Undirected, directed
  * Labeled directed
  * Cyclic, acyclic
  * Rooted trees: (V, E, r) where r ∈ V
* Transitive closure: generalization of a path. Given a directed graph, find out if a vertex j is reachable from another vertex i for all vertex pairs (i, j) in the given graph. Asking "what is the transitive closure of node A?" is equivalent to asking "what is the set of nodes that can be reached by node A?"
* What is a computer?
  * Input, output
  * Memory state
    * Well-defined initial state
  * Execution
  * Deterministic
  * Program, set of instructions
