---
aliases: []
---

# Winkel #card
## Definition
Es seien $x, y \in V \backslash\{0\}$ und $V$ ein [[Euklidischer Vektorraum]]. Der von $x$ und $y$ eingeschlossene Winkel ist die eindeutig bestimmte Zahl $\angle(x, y) \in[0, \pi]$ mit
$$
\cos (\angle(x, y))=\frac{\langle x, y\rangle}{\|x\| \cdot\|y\|}
$$
## Bemerkungen
Für alle $x, y \in V \backslash\{0\}$ und $\lambda, \mu \in \mathbb{R} \backslash\{0\}$ gilt:
- $\angle(x, y)=\angle(y, x)$,
- $\angle(\lambda x, \mu y)=\left\{\begin{array}{cc}\angle(x, y), & \lambda \mu>0, \\ \pi-\angle(x, y), & \lambda \mu<0\end{array}\right.$
-  $\angle(x, y)=0$ genau dann wenn $y=\alpha x$ für ein $\alpha>0$,
- $\angle(x, y)=\pi$ genau dann wenn $y=\alpha x$ für ein $\alpha<0$.
## Hinweis
- Da das [[unitäres Skalarprodukt]] im Allgemeinen nicht reell ist, mach die Definition von Winkeln (außer $0, \frac{\pi}{2}$ und $\pi$) in einem [[unitärer Vektorraum]] keinen Sinn.
^c-vervERlguZ
---
**Tags**: 