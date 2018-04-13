# Discussion 2: April 13, 2018
## Closure of Regular Languages
* Union
* Intersect
* Kleene closure
* Concatenation
* Complement
### Methods of Proof
1. Construct a DFA or NFA algorithm
2. Define language in terms of closed operations
### Transitive Closure
* δ* vs δ
  * δ(Q, a) is a function from one state and one symbol to one state (function from (q,a) to q where a∈Σ)
  * δ* is a function from one state and any string in Σ* to one state. It is recursive and uses d.
    * Difference between δ and δ*: δ* accepts strings and ɛ rather than just individual symbols
    * Inductive: δ* exists for one state. For any other symbol of a string you can always get to the next symbol and a valid state
    * Inductive in other words: Prove that δ(q,a) will always yield q. Prove that Σ* can always be split into ax, where x is a smaller string.
