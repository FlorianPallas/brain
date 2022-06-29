---
aliases: []
---

# Gram-Schmidt-Verfahren #card
## Idee
![[Pasted image 20220629165237.png]]
## Definition
Ein Verfahren welches eine beliebige [[Basis]] $A = (a_{1}, \dots, a_{n})$ eines [[Vektoraum|Vektorraums]] $V$ zunächst in eine [[Orthogonalbasis]] $B$ und im zweiten Schritt in eine [[Orthonormalbasis]] $C$ umwandelt.

Die paarweise zueinander [[Orthogonalität|orthogonalen]] Basisvektoren von $B$ erhält man durch folgenden Vorschrift:
$$
b_{j} := a_{j} - \sum_{k=1}^{j-1} \frac{<a_{j}, b_{k}>}{<b_{k}, b_{k}>} b_{k}
$$
Die normalisierte Basis $C$ kann schließlich durch [[Normierung|Normieren]] der Basisvektoren aus $B$ bestimmt werden.

## Folgerungssatz
Satz 3.6. Ist $V$ endlich-dimensional, so lässt sich jede [[Orthogonalität|orthogonale]] Teilmenge von $V \backslash\{0\}$ zu einer [[Orthogonalbasis]] von $V$ ergänzen. Es gibt eine [[Orthonormalbasis]] $B=\left(b_{1}, b_{2}, \ldots, b_{n}\right)$ von $V$, und jedes $v \in V$ lässt sich bezüglich $B$ schreiben als
$$
v=\left\langle v, b_{1}\right\rangle b_{1}+\left\langle v, b_{2}\right\rangle b_{2}+\cdots+\left\langle v, b_{n}\right\rangle b_{n} .
$$
(Fourierformel)
Für den Basisisomorphismus $D_{B}: V \rightarrow \mathbb{K}^{n}$ gilt folglich
$$
D_{B}(v)=\left(\begin{array}{c}
\left\langle v, b_{1}\right\rangle \\
\left\langle v, b_{2}\right\rangle \\
\vdots \\
\left\langle v, b_{n}\right\rangle
\end{array}\right) .
$$

^c-7EGgzIeYdt

---
**Tags**: 