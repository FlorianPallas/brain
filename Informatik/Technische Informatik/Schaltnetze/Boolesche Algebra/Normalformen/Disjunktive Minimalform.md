---
aliases: [DMF]
---

# Disjunktive Minimalform #card
## Definition
Ein Ausdruck in disjunktiver Minimalform (Abk.: DMF) ist eine Disjunktion von Konjunktionen
$$
y\left(x_{1}, \ldots, x_{n}\right)=\left(L_{11} \cdots \cdots L_{1 k}\right) \vee \ldots \vee\left(L_{m 1} \cdots \cdots L_{m j}\right)
$$
mit den Literalen $L_{v w} \in\left\{x_{1}, \ldots, x_{n}, \bar{x}_{1}, \ldots, \bar{x}_{n}\right\}$, welche die gesamten Realisierungskosten
$$
Y_{y}=\Psi_{O D E R}(m)+\Psi_{U N D}(k)+\cdots+\Psi_{U N D}(j)
$$
minimiert.
## Beispiele
- $y_{1}=\bar{a} b \vee a \bar{b}$ ist in disjunktiver Minimalform,
- $y_{2}=\bar{a} b \vee a b$ jedoch nicht, da $y_{2}$ auch kürzer durch $y_{2}=b$ ausgedrückt werden kann.
^c-Rh1ZF54K18
---
**Tags**: 