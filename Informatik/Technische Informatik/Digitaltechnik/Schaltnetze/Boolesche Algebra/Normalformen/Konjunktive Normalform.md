---
aliases: [KNF]
---

# Konjunktive Normalform #card
## Definition
Es sei eine [[Boolesche Funktionen|Booleschen Funktion]] $y\left(x_{1}, \ldots, x_{n}\right)$ gegeben. Ein Boolescher Ausdruck heißt konjunktive Normalform (Abk.: KNF), wenn er aus einer konjunktiven Verknüpfung von [[Maxterm|Maxtermen]] $D_{i}$ besteht:
$$
y=D_{0} \wedge D_{1} \wedge \cdots \wedge D_{k} \quad, k \leq 2^{n}-1
$$
Es darf dabei keine zwei Disjunktionen $D_{i}, D_{j}$ mit $i \neq j$ geben, die zueinander äquivalent sind.
## Beispiel
- $y=(a \vee b \vee c) \wedge(a \vee \bar{b} \vee c) \wedge(\bar{a} \vee \bar{b} \vee c)$
## Eigenschaft
- Die konjunktive Normalform ist bis auf Vertauschung der Konjunktionen eindeutig.
^c-4W7Y9CY7yf
---
**Tags**: 