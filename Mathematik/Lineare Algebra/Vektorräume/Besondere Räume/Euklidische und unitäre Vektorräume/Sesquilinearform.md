---
aliases: [hermitesche Sesquilinearform]
---

# Sesquilinearform #card
## Definition
Eine Abbildung $s: V \times V \rightarrow \mathbb{C}$ heißt Sesquilinearform, falls für alle $x, y, z \in V$ und alle $\alpha \in \mathbb{C}$ gilt
$$
\begin{aligned}
s(x+y, z) &=s(x, z)+s(y, z), \\
s(x, y+z) &=s(x, y)+s(x, z), \\
s(\alpha x, y) &=\alpha s(x, y), \\
s(x, \alpha y) &=\bar{\alpha} s(x, y) .
\end{aligned}
$$
## Hinweis
- Ist im ersten Argument linear
- Heißt hermitesch, falls $\forall x,y \in V: s(x,y) = \overline{s(y,x)}$ 
- Heißt positiv definit, falls $\forall x\neq0 \in V: s(x,x)\gt0$
^c-kKsZerKZS3
---
**Tags**: 