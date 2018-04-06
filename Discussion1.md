# Discussion 1: April 6, 2018
## Logistics
* Office Thurs 10am-12pm @ Boelter 2432
## Notation
* Σ represents an alphabet
* L = language
* M = DFA
* L(M) describes language accepted by machine
* L = {w| predicate over w} ∈ Σ*
* Σ* zero or more elements of the set
* Σ<sup>+</sup> one or more elements of the set
## DFA
* Example for Σ = {0,1}; L = {w| all strings that end in 01} 

  ![DFA 1](images/disc1-1.PNG)
* Example for Σ = {0,1}; L = {w| no two consecutive 0s and ends with a 1}

  ![DFA 2](images/disc1-2.PNG)
## Transition Functions
* Denoted by δ(current state, input), returns next state
* [Example](https://qph.fs.quoracdn.net/main-qimg-20ed869770b369d15eb8365220016858)
  * δ(q<sub>1</sub>, 1) = q<sub>2</sub>
  
