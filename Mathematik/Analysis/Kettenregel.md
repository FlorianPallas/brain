---
aliases: []
---

# Kettenregel
## Definition #card
Wenn die Funktionen $f$, $g$
$$
D\subseteq \mathbb{R}^{n}\to E \subseteq \mathbb{R}^{m}\to \mathbb{R}^{p}
$$
[[Totale Differenzierbarkeit|db.]] sind, dann ist auch $g \circ f: D \to \mathbb{R}$ db. mit $x \mapsto g(f(x))$ .

Eine Funktion $f: D\subseteq \mathbb{R}^{n}\to \mathbb{R}^m$ heißt differenzierbar in $u \in D$, wenn alle Koordinatenfunktionen $f_{1}, ... , f_{m}$ db. in $u$ sind. Dann schreibt man
$$
f'(x):=\begin{pmatrix}
grad f_{1}(x) \\ \vdots \\ grad f_{m}(x)
\end{pmatrix} =
\left(\begin{array}{}
\frac{\partial f_1}{\partial x_1}(x) & \cdots & \frac{\partial f_1}{\partial x_n}(x) \\
\vdots & \ddots & \vdots \\
\frac{\partial f_m}{\partial x_1}(x) & \cdots & \frac{\partial f_m}{\partial x_n}(x)
\end{array}\right)
\in \mathbb{R}^{m \times n}
$$
([[Jacobimatrix]]) und
$$(g \circ f)'(x) = g'(f(x)) \cdot f'(x)$$

### Bemerkung
Mit $r=n=p=1$ folgt die Kettenregel im reellen.
^c-FGYs5KawoZ

## Beispiele
![[Pasted image 20220525081857.png]]

---
**Tags**: 