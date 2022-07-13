---
aliases: [riccati DGL, riccatischen DGL]
---

# riccatische DGL #card
## Definition
Eine [[Differentialgleichung|DGL]] der Form
$$
y'(x) = a(x) \cdot y(x) + b(x) \cdot 
(y(x))^{2} + c(x)
$$
heißt **riccatische DGL**. Die Form ist ähnlich zur [[bernoullische DGL|bernoullischen DGL]], erlaubt allerdings einen Störterm $c(x)$

## Verfahren
1. Eine Lösung $z$ der DGL raten (z.B. Monome $1,x,x^{2},\cdots, x^{-1}$ oder $e^{x}, \cdots$)
2. Transformiere die DGL mit dem Ansatz $g(x) := y(x) - z(x)$ in eine [[bernoullische DGL]] für $g$.
3. Lösen dieser bernoulli DGL und Rücksubstituieren nach $y$ liefer die Lösungen der originalen DGL.
^c-EAOHSWiErn

---
**Tags**: #todo 