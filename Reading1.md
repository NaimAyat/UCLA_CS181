# Introduction to the Theory of Computation - Sipser (3rd Edition)
## 0.2 Mathematical Notations and Terminology
* Set with one member: singleton set
* Set with two members: unordered pair
* To describe a set containing elements according to some rule, write {n| rule about n}. For example, {n| n = m<sup>2</sup> for some m ∈ N} refers to the set of perfect squares
* Complement of a set A is denoted with a bar, A̅
### Sequences and Tuples
* A sequence of objects is a list of objects in some order, written within parentheses
* Repetition and order matters in sequences, not sets
* Finite sequences are called tuples
* Sequences with k elements are called k-tuple
* 2-tuples are called ordered pairs
* The *power set* of A is the set of all subsets of A, including the null set and itself
* The cartesian product or cross product of A and B, A x B, is the set of all ordered pairs wherin the first element is a member of A and the second element is a member of B.
* Predicate/property: function whose range is {true, false}
* A property whose domain is a set of k-tuples A x ... x A is called a relation, a k-ary relation, or a k-ary relation on A. A common case is a 2-ary relation, called a binary relation
* A special type of binary relation, called an equivalence relation, captures the notion of two objects being equal in some feature. A binary relation R is an equivalence relation if R satisfies three conditions:
  1. R is reflexive if for every x, xRx;
  2. R is symmetric if for every x and y, xRy implies yRx; and
  3. R is transitive if for every x, y, and z, xRy and yRz implies xRz.
### Graphs
* Simple path is a path that doesnt repeat any nodes
* Graph is connected if every two nodes have a path between them
* Path is a cycle if it starts and ends at the same node
* Simple cycle contains at least three nodes and repeats only the first and last nodes
* A directed graph has arrows instead of lines, as shown in the following figure. The number of arrows pointing from a particular node is the outdegree of that node, and the number of arrows pointing to a particular node is the indegree.
* A path in which all the arrows point in the same direction as its steps is called a directed path. A directed graph is strongly connected if a directed path connects every two nodes
### Strings and Languages
* We define an alphabet to be any nonempty finite set. The members of the alphabet are the *symbols* of the alphabet
* We generally use capital Greek letters Σ and Γ to designate alphabets and a typewriter font for symbols from an alphabet
  * Example alphabet: Γ = {0, 1, x, y, z}
* A string over an alphabet is a finite sequence of symbols from that alphabet, usually written next to one another and not separated by commas. If Σ = {0,1}, then 01001 is a string over Σ
* If w is a string over Σ, the length of w, written |w|, is the number of symbols that it contains
* The string of length zero is called the empty string and is written ε
* Reverse of a string w is denoted as w<sup>r</sup>
## 0.4 Types of Proof
### Proof by Construction
* Demonstrate how to construct the object
### Proof by Contradiction
* Assume that the theorem is false and then show that this assumption leads to an obviously false consequence, called a contradiction
### Proof by Induction
* Has basis and induction step
* Goal is to prove P(1) is true for every K in some property P
* Basis proves that P(1) is true
* Induction step proves that for each i ≥ 1, if P(i) is true, then so is P(i + 1)
## 1.1 Finite Automata
* Finite automata and their probabilistic counterpart Markov chains are useful tools when we are attempting to recognize patterns in data. These devices are used in speech processing and in optical character recognition.
* A finite automaton is a 5-tuple (Q, Σ, δ, q<sub>0</sub>, F), where
   1. Q is a finite set called the states,
   2. Σ is a finite set called the alphabet,
   3. δ : Q × Σ→Q is the transition function,
   4. q<sub>0</sub> ∈ Q is the start state, and
   5. F ⊆ Q is the set of accept states.
* The transition function, δ, defines the rules for moving. If the finite automaton has an arrow from a state x to a state y labeled with the input symbol 1, thatmeans that if the automaton is in state x when it reads a 1, it then moves to state y. We can indicate the same thing with the transition function by saying that δ(x, 1) = y
* If A is the set of strings machine M accepts, A is the language of machine M, written as L(M) = A. We say that M recognizes A or M accepts A
* A machine may accept several strings, but it always recognizes only one language. If the machine accepts no strings, it still recognizes one language— namely, the empty language ∅
### Formal Definition of Computation
* Let M = (Q, Σ, δ, q<sub>0</sub>, F) be a finite automaton and let w = w<sub>1</sub>w<sub>2</sub> ... w<sub>n</sub> be a string where each w<sub>i</sub> is a member of the alphabet Σ. Then M accepts w if a sequence of states r<sub>0</sub>, r<sub>1</sub>, ... , r<sub>n</sub> in Q exists with three conditions:
  1. r<sub>0</sub> = q<sub>0</sub>,
  2. δ(r<sub>i</sub>, w<sub>i</sub>+1) = ri+1, for i = 0, ... , n − 1, and
  3. r<sub>n</sub> ∈ F.
* We say that M recognizes language A if A = {w| M accepts w}
* A language is called a *regular language* if some finite automaton recognizes it
### The Regular Operations
* Let A and B be languages. We define the regular operations union, concatenation, and star as follows:
  * Union: A ∪ B = {x| x ∈ A or x ∈ B}.
  * Concatenation: A ◦ B = {xy| x ∈ A and y ∈ B}.
  * Star: A* = {x<sub>1</sub>2<sub>i</sub> ... x<sub>k</sub>| k ≥ 0 and each x<sub>i</sub> ∈ A}.
