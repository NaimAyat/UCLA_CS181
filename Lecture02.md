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
* Note: concatenating the empty string with a word simply returns the word
* Note: strings must be finite
* Assume we have string w = rst
  * Substring ≡ s is a substring of w
  * Prefix ≡ r is a prefix of w, rs is a prefix of w, rst is a prefix of w (but not a proper prefix)
  * Suffix ≡ t is a suffix of w, st is a suffix of w, rst is a suffix of w (but not a proper suffix)
  * Proper substring/prefix/suffix: not the entire string
* ε is a prefix/suffix/substring of every string over any alphabet ∑
  * ε is a prefix/suffix/substring of itself, but is not a proper prefix/suffix/substring of itself
* *Run*: the entirety of a consecutive sequence of the same character
  * Example: 11100001111 has three runs
* Language ≡ any set of strings (words) over ∑
  * Example: {all even length strings}
## Finite State Machines
* Deterministic finite automaton (DFA)
  * Accepting state: double circle
  * String read one at a time, no going back. For example, a string of length 5 needs 5 movements
* If the move is not defined, we say the machine blocks
* Example: 
  * ∑ ≡ {a,b}
  * L ≡ {w| in every prefix of w, the number of "a"s and the number of "b"s differ at most by 2}
    
    ![DFA](images/april4-2.PNG)
