---
aliases: []
---

# Fundamentalmatrix #card
## Definition
Ist $V$ endlich-dimensional, $B=\left(b_{1}, b_{2}, \ldots, b_{n}\right)$ eine geordnete Basis von $V$ und $s: V \times V \rightarrow \mathbb{K}$ eine [[Bilinearformen|Bilinearform]], so heißt die Matrix
$$
F_{B}(s):=\left(\begin{array}{ccc}
s\left(b_{1}, b_{1}\right) & \cdots & s\left(b_{1}, b_{n}\right) \\
\vdots & \ddots & \vdots \\
s\left(b_{n}, b_{1}\right) & \cdots & s\left(b_{n}, b_{n}\right)
\end{array}\right)
$$
Fundamentalmatrix von s bezüglich $B$. Mit der Fundamentalmatrix lässt sich die [[Bilinearformen|Bilinearform]] folgendermaßen auswerten:
$$s(v, w)=\left(D_{B}(v)\right)^{\top} \cdot F_{B}(s) \cdot D_{B}(w)$$
## Eigenschaften
- s ist symmetrisch genau dann, wenn $F_{B}(s)$ eine symmetrische Matrix ist.
- s ist schiefsymmetrisch genau dann, wenn $F_{B}(s)$ eine schiefsymmetrische Matrix ist (das heißt $F_{B}(s)^{\top}=-F_{B}(s)$ ).
## Basiswechsel der Fundamentalmatrix
Ist $V$ ein endlich-dimensionaler Vektorraum über einem Körper $\mathbb{K}$, und sind $B, C$ Basen von $V$, so gilt für jede Bilinearform $s: V \times V \rightarrow \mathbb{K}$
$$
F_{B}(s)=\left(D_{C B}\left(\mathrm{id}_{V}\right)\right)^{\top} \cdot F_{C}(s) \cdot D_{C B}\left(\mathrm{id}_{V}\right)
$$
## [[Diagonalisierbarkeit]]
Falls die [[Bilinearformen|Bilinearform]] symmetrisch ist und paarweise verschiedene [[Eigenwerte]] $\lambda_i$ besitzt, so ist die Fundamentalmatrix diagonalisierbar. Achtung: Auf der Diagonalen stehen im Allgemeinen nicht die [[Eigenwerte]], sondern $\lambda_i \cdot v_i^T \cdot v_i$.
^c-SdsAaiP17l
---
**Tags**: 