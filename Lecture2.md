# Lecture 2: April 4, 2018
## Today's Lecture
* Review of elements
* Power and energy
* Typical signals
* What is a computer?
  * Input
  * Output
  * Programs
  * Storage
  * Deterministic
  * Execution
  * Problems
  * Classes of problems
* What can computers do and not do?
* Math foundations: sets, Cartesian product
* Graphs, rooted trees
## Strings
* Alphabet ≡ any finite set of symbols, except ε for the empty string
  * Example: binary alphabet is {0,1}
  * Subset of C alphabet: {for, if, while, int, ...}
    * Note that elements like "for" are treated as one symbol, so for<sup>R</sup> is still "for"
  * Alphabets can contain ordered pairs: {(0,1), a, b, 1, 3, 4}
    * Note that (0,1) is treated as a single symbol here
* String ≡ word ≡ sequence of zero or more symbols from an alphabet ∑
  * Word w over alphabet ∑ ≡ concatenation of symbols from ∑: w = a<sub>1</sub> • a<sub>2</sub> • ... • a<sub>i</sub> for some i ≥ 0 each a<sub>j</sub>∈∑ 1≤j≤i.
* Concatenating the empty string with a word simply returns the word
