---
aliases: []
---

# Richtungsableitung
## Definition #card
Fuer eine [[Funktion]] $f: D \subseteq \mathbb{R}^{n}\to \mathbb{R}$, einen Punkt $u \in D$ und eine [[Richtung]] $v \in \mathbb{R}^{n}$ mit $||v||=1$, heißt
$$
\frac{\partial f}{\partial v} (u) :=
\lim_{t\to0} \frac{f(u+t\cdot v) - f(u)}{t}
$$
die Richtungsableitung von $f$ in $u$ nach $v$ (wenn der [[Mathematik/Analysis/HMII/Konvergenz/Grenzwert]] existiert).

Ist $f$ [[Totale Differenzierbarkeit|db.]] in $u$, dann existieren alle Richtungsableitungen $\frac{\partial f}{\partial v} (u)$ und es ist
$$
\frac{\partial f}{\partial v} (u) = grad f(u) \cdot v
$$

### Bemerkung
Die Richtungsableitung entlang eines Einheitsvektors entspricht dabei der [[Partielle Differenzierbarkeit|partiellen Ableitung]]. Es gilt
$$\frac{\partial f}{\partial e_{i}}= \frac{\partial f}{\partial x_i}$$
^c-LHEA1Dzdhv

## Beispiele
![[Pasted image 20220524100216.png]]

![[Pasted image 20220525081816.png]]
---
**Tags**: 