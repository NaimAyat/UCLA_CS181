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
