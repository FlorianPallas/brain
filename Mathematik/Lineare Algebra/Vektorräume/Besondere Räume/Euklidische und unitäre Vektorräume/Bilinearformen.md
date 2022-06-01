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
	- ist ausgeartet, falls [[Radikal]] $\operatorname{rad}(s)\neq \{0\}$  
	- ist positiv definit, falls für alle $v \in V \backslash\{0\}$ gilt, dass: $s(v, v)>0$
	- Hinweis: Ausgeartet und positiv definit schließen sich gegenseitig aus.
- ist schiefsymmetrisch, falls $s(x, y)=-s(y, x) \; \forall x, y \in V$
- ist alternierend, falls $s(x, x)=0 \; \forall x \in V$. 
	- Eine alternierende Bilinearform ist stets schiefsymmetrisch
- Die Menge der Bilinearformen auf $V$ ist ein Untervektorraum des $\mathbb{K}$-Vektorraums $\operatorname{Abb}(V \times V, \mathbb{K})$ ([[Dualraum]]).
## Beispiele
- [[Standardskalarprodukt]] (symmetrisch)
- [[Determinante]] in $\mathbb{K}^2$
- $V=\mathrm{C}([a, b])$ als $\mathbb{R}$-Vektorraum mit $s(f, g)=\int_{a}^{b} f(x) g(x) \mathrm{d} x$ für $f, g \in \mathrm{C}([a, b])$
- $V=\mathbb{K}^{n}, A \in \mathbb{K}^{n \times n}, s_{A}: \mathbb{K}^{n} \times \mathbb{K}^{n} \rightarrow \mathbb{K},(x, y) \mapsto x^{\top} \cdot A \cdot y$
	- [[Standardskalarprodukt]] erhält man für $A=E$.
## Fundamentalmatrix
Jede endlichdimensionale Bilinearform kann als [[Fundamentalmatrix]] codiert werden.
^c-E8RTHsatJp
---
**Tags**: 