---
aliases: []
---

# komplexe Fundamentalmatrix #card
## Definition
Ist $V$ endlich-dimensionaler [[unitärer Vektorraum]] und sei $B=\left(b_{1}, b_{2}, \ldots, b_{n}\right)$ eine geordnete Basis von so heißt die Matrix
$$
G:=\left(\begin{array}{ccc}
\langle b_{1}, b_{1} \rangle & \cdots & \langle b_{1}, b_{n}\rangle \\
\vdots & \ddots & \vdots \\
\langle b_{n}, b_{1}\rangle & \cdots & \langle b_{n}, b_{n}\rangle
\end{array}\right) \in \mathbb{C}^{n \times n}
$$
Fundamentalmatrix des [[unitäres Skalarprodukt]] bezüglich $B$. Mit der Fundamentalmatrix lässt sich das [[unitäres Skalarprodukt]] folgendermaßen auswerten:
$$ \langle v, w \rangle =\left(D_{B}(v)\right)^{\top} \cdot F_{B}(s) \cdot \overline{D_{B}(w)}$$
## Eigenschaften
- $G$ ist hermitesch 
- $G$ ist positiv definit
- Folglich ist $G$ invertierbar (siehe [[Matrix]]) 
^c-dIuyCwUFDX
---
**Tags**: 