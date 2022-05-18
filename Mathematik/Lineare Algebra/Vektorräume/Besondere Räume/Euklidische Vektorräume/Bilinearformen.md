---
aliases: [Bilinearform, Fundamentalmatrix]
---

# Bilinearformen #card
## Definition
Eine Abbildung $s: V \times V \rightarrow \mathbb{K}$ heißt Bilinearform, falls für beliebige $x, y, z \in V$ und $\alpha \in \mathbb{K}$ gilt
$$
\begin{aligned}
s(x+y, z) &=s(x, z)+s(y, z) \\
s(x, y+z) &=s(x, y)+s(x, z), \\
s(\alpha x, y) &=\alpha s(x, y), \\
s(x, \alpha y) &=\alpha s(x, y) .
\end{aligned}
$$
(Linear im 1. und im 2. Argument)
## Eigenschaften
- ist symmetrisch, falls $s(x, y)=s(y, x) \; \forall x, y \in V$
- ist schiefsymmetrisch, falls $s(x, y)=-s(y, x) \; \forall x, y \in V$
- ist alternierend, falls $s(x, x)=0 \; \forall x \in V$. 
	- Eine alternierende Bilinearform ist stets schiefsymmetrisch
- Die Menge der Bilinearformen auf $V$ ist ein Untervektorraum des $\mathbb{K}$-Vektorraums $\operatorname{Abb}(V \times V, \mathbb{K})$ ([[Dualraum]]).
## Beispiele
- [[Standardskalarprodukt]]
- [[Determinante]] in $\mathbb{K}^2$
- $V=\mathrm{C}([a, b])$ als $\mathbb{R}$-Vektorraum mit $s(f, g)=\int_{a}^{b} f(x) g(x) \mathrm{d} x$ für $f, g \in \mathrm{C}([a, b])$
- $V=\mathbb{K}^{n}, A \in \mathbb{K}^{n \times n}, s_{A}: \mathbb{K}^{n} \times \mathbb{K}^{n} \rightarrow \mathbb{K},(x, y) \mapsto x^{\top} \cdot A \cdot y$
	- [[Standardskalarprodukt]] erhält man für $A=E$.
## Fundamentalmatrix
Ist $V$ endlich-dimensional, $B=\left(b_{1}, b_{2}, \ldots, b_{n}\right)$ eine geordnete Basis von $V$ und $s: V \times V \rightarrow \mathbb{K}$ eine Bilinearform, so heißt die Matrix
$$
F_{B}(s):=\left(\begin{array}{ccc}
s\left(b_{1}, b_{1}\right) & \cdots & s\left(b_{1}, b_{n}\right) \\
\vdots & \ddots & \vdots \\
s\left(b_{n}, b_{1}\right) & \cdots & s\left(b_{n}, b_{n}\right)
\end{array}\right)
$$
Fundamentalmatrix von s bezüglich $B$. Mit der Fundamentalmatrix lässt sich die Bilinearform folgendermaßen auswerten:
$$s(v, w)=\left(D_{B}(v)\right)^{\top} \cdot F_{B}(s) \cdot D_{B}(w)$$
### Eigenschaften der Fundamentalmatrix
- s ist symmetrisch genau dann, wenn $F_{B}(s)$ eine symmetrische Matrix ist.
- s ist schiefsymmetrisch genau dann, wenn $F_{B}(s)$ eine schiefsymmetrische Matrix ist (das heißt $F_{B}(s)^{\top}=-F_{B}(s)$ ).

^c-E8RTHsatJp
---
**Tags**: 