# Lecture 4: April 11, 2018
## Last Time
* Alphabet Σ = nonempty, finite set of symbols (except ε)
* Words = concatenation of symbols
* Language = set of words
* Family of languages = set of languages
* To get from alphabet to words, use concatenation operator •
* To get from words to lanuages, form sets {}
* How do we specify which languages are in a family of languages?
  * Set of all languages that can be recognized by a DFA = finite state languages (FSL)
## Regular Sets
* Basis: 
  * {}
  * {ε}
  * {a<sub>i</sub>} ∀ 1≤n≤i
* Inductive / Recursive: 
   * If r and s are regular sets, then so are
     * r • s
     * r ∪ s
     * r*
* Anything that's accepted by a DFA is a regular set; regular sets are equivalent to finite state languages
### Regular Expressions

