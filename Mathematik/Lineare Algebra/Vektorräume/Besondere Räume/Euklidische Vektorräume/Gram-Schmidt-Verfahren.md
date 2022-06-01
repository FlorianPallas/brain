---
aliases: []
---

# Gram-Schmidt-Verfahren #card
## Definition
Ein Verfahren welches eine beliebige [[Basis]] $A = (a_{1}, \dots, a_{n})$ eines [[Vektoraum|Vektorraums]] $V$ zunächst in eine [[Orthogonalbasis]] $B$ und im zweiten Schritt in eine [[Orthonormalbasis]] $C$ umwandelt.

Die paarweise orthogonalen Basisvektoren von $B$ erhält man durch folgenden Vorschrift:
$$
b_{j} := a_{j} - \sum_{k=1}^{j-1} \frac{<a_{j}, b_{k}>}{<b_{k}, b_{k}>} b_{k}
$$

Die normalisierte Basis $C$ kann schließlich durch [[Normierung|Normieren]] der Basisvektoren aus $B$ bestimmt werden.


---
**Tags**: #todo 