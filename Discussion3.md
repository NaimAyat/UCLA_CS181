# Discussion 3: June 8, 2018
* Recursive language: Turing machine always halts and accepts or halts and rejects on all input
* Recursively enumerable, not recursive language: Turing machine always halts and accepts, but if it rejects it may not halt
* If a language is inherently ambiguous, it must have a nondeterministic CFG and cannot have a DCFG
## Final Topics
* Ambiguous grammars
  * Grammar for which there exists a string that can have more than one leftmost derivation or parse tree
* Unambiguous grammars
  * Every valid string has a unique leftmost derivation or parse tree
* Ambiguous languages
* Unambiguous languages
* Recursively enumerable language
  * Halts on all strings that are part of the language, but may loop infinitely on strings that are not
* Recursive language
  * Halts on all strings that are part of the language and all strings that are not. Subset of recursively enumerable.
* Pumping lemma for CFGs and FSLs
* Construct a PDA
  * Describe the language modeled by a PDA
* Write CFGs for FSLs
* Can you have an:
  * ambiguous deterministic grammar? No. You can not come up with two parse trees for something if you have more than one choice.
  * ambiguous nondeterministic grammar? Yes. You can have two parse trees that are both correct.
  * unambiguous deterministic grammar? Yes. One parse tree, one choice.
  * unambiguous nondeterministic grammar? Yes. One parse tree, two choices; one doesn't work.
* Can you have an:
  * ambiguous deterministic language? No. There is a DPDA, meaning there must be an unambiguous grammar.
  * ambiguous nondeterministic language? Yes. There is no DPDA, meaning there can be an ambiguous grammar.
  * unambiguous deterministic language? Yes. There is a DPDA, meaning there must be an unambiguous grammar.
  * unambiguous nondeterministic language? Yes. 
* If you have an inherently ambiguous language, it must have an ambiguous grammar
* Ambiguity: # of parse trees you can have; Determinism: number of choices you have
## FSM
* Recognizes FSLs
## PDA
* Recognizes CFGs
