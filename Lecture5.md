# Lecture 5: April 16, 2018
## Today
* Tellegen's Theorem
* Node analysis
## Families of Languages
### Regular Sets (Languages Recognized by DFAs)
#### Closure Properties
* Let S, T be regular sets. Then:
  * S ∪ T is a regular set
  * S • T is a regular set
  * S* is a regular set
  * S ∩ T is a regular set
  * S<sup>R</sup> is a regular set (reverse)
  * h(S) is a regular set (homomorphism)
* Σ = { a, b }; L = { w | number of "a"s is twice the number of "b"s } 
  * Not finite state language (FSL)
* L<sub>1</sub> ∪ L<sub>2</sub> = L<sub>3</sub>
  * Given L<sub>2</sub> is FSL and L<sub>3</sub> is not, we know L<sub>1</sub> is FSL
  * Given L<sub>1</sub> is not FSL and L<sub>2</sub> is FSL, we don't know anything about L<sub>3</sub>
* L<sub>1</sub> ⊆ L<sub>2</sub> ⊆ L<sub>3</sub>
  * Knowing L<sub>1</sub> is/isn't FSL doesn't tell us anything about the others
  * Knowing L<sub>3</sub>  is/isn't FSL tells us the others are the same
### Known Non-FSLs
* { a<sup>n</sup>b<sup>n</sup> }
* { a<sup>n</sup>ba<sup>n</sup> }
* { x#y | x,y ∈ {a,b}* and |x|=|y| }
* { ww | w ∈ Σ* }
* {w | number of "a"s = number of "b"s }
### NFA
* At every nondeterministic fork, N chooses one branch
* Graph search
* Graph unrolling
* All possible computations in parallel
