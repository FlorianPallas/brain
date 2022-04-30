---
cards-deck: Lineare Algebra
#todo
---

# Determinante

## Definition
Im $\mathbb{K}^n$ stellt die Determinante das Volumen des Objekts (mit Vorzeichen) dar.

multilinear, schiefsymmetrisch, normiert, parallel Epiped
Die Determinante ist eine [[Invariante]]. Ihr Wert bleibt also bei einem Basiswechsel erhalten.


## Regeln
Aus den Eigenschaften der Determinante können folgende Rechenregeln abgeleitet werden:
- $det(A \cdot B) = det(A) \cdot det(B)$
- Aber: $det(A+B) \neq det(A) + det(B)$
- $\forall k \in \mathbb{Z}: det(A^k) = det(A)^k$
- $det(\lambda \cdot A) = \lambda^n \cdot det(A)$
- $det()=1$
- $det(A^T) = det(A)$

$det(\begin{pmatrix} * & * & * \\ \lambda a_{1} & ... & \lambda a_{n} \\ * & * & * \end{pmatrix}) = \lambda \cdot det(\begin{pmatrix} * & * & * \\ a_{1} & ... & a_{n} \\ * & * & * \end{pmatrix})$

Addition von Vielfachen einer Spalte oder Zeil verändern die Determinante nicht. Beim Tausch einzelner angrenzenden Zeilen oder Spalten ändert sich allerdings das Vorzeichen der Determinante.

$det(\begin{pmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{pmatrix}) = -det(\begin{pmatrix} 4 & 5 & 6 \\ 1 & 2 & 3 \\ 7 & 8 & 9 \end{pmatrix})$


## Berechnung

### $2 \times 2$ Matrix

### Laplace
[[Laplace Verfahren]]

### Dreiecksmatrix

### $3 \times 3$ Matrix
