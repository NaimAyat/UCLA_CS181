# Lecture 9: April 30, 2018
## Sentential Form
* G = (V, Σ, R, S)
  * S → α → ...
  * (Σ ∪ V)*
* We say that G "generates" or "derives" as S → α → ...
## Pumping Lemma Examples
### Example 1
* Σ = {0, 1}
* Show { ww | w ∈ Σ* }. Choose: s = 0<sup>p</sup>1<sup>p</sup>0<sup>p</sup>1<sup>p</sup>
### Example 2
* Let the number of "a"s in r be a(r) and so on
* L = { r#s#t | r, s, t ∈ (a + b)* }, a(s) < a(r) < a(t)
* Σ = { a, b, # } 
* Choose s = a<sup>p</sup>#a<sup>p-1</sup>#a<sup>p+1</sup>
* s = xyz, |xy| ≤ p, |y| ≥ 1, xy<sup>i</sup>z ∈ L
 
