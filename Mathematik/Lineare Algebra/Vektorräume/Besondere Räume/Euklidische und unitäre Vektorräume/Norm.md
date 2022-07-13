---
aliases: [normiert]
---

# Norm #card
## Definition
Es sei $V$ ein [[Vektorraum]] über dem Körper $\mathbb{K}=\mathbb{R}$ oder $\mathbb{K}=\mathbb{C}$. Eine [[Abbildung]] $\|\cdot\|: V \rightarrow \mathbb{R}$ heißt Norm, wenn für alle $v, w \in V$ und alle $\lambda \in \mathbb{K}$ gilt:
- Definitheit: $\|v\|>0$ falls $v \neq 0$, und $\|v\|=0$ falls $v=0$,
- Homogenität: $\|\lambda v\|=|\lambda| \cdot\|v\|$,
- Dreiecksungleichung: $\|v+w\| \leq\|v\|+\|w\|$.
## Norm im [[Euklidischer Vektorraum|euklidischen Vektorraum]]
$\|\cdot\|: V \rightarrow \mathbb{R}, \quad v \mapsto\|v\|:=\sqrt{\langle v, v\rangle}$
## Norm im [[unitärer Vektorraum]]
$\|\cdot\|: V \rightarrow \mathbb{R}, \quad v \mapsto\|v\|:=\sqrt{\langle v, v\rangle}$
Somit ist die Norm identisch mit der Norm im [[Euklidischer Vektorraum|euklidischen Vektorraum]].
## Parallelogrammungleichung Satz
Es sei $(V,\|\cdot\|)$ ein normierter $\mathbb{R}$-Vektorraum.
(a) Gehört $\|\cdot\|$ zu einem [[(euklidische) Skalarprodukt]] $\langle\cdot, \cdot\rangle$ auf $V$, so ist die Parallelogrammgleichung erfüllt, das heißt es gilt für alle $x, y \in V$
$$
\|x+y\|^{2}+\|x-y\|^{2}=2\|x\|^{2}+2\|y\|^{2} .
$$
(b) Gilt umgekehrt für $\|\cdot\|$ die Parallelogrammgleichung, so gibt es ein [[(euklidische) Skalarprodukt]] $\langle\cdot, \cdot\rangle$ auf $V$ mit $\|v\|=\sqrt{\langle v, v\rangle}$ für alle $v \in V$.
### Hinweis:
Die Parallelogrammungleichung gilt auch in $\mathbb{C}$ für Aussage a). Aber Aussage b) ist in $\mathbb{C}$ nicht erfüllt.
## Maximalnorm:
Sei $V=\mathbb{R}^{n}$ versehen mit der sogenannten Maximumsnorm, die definiert ist durch
$$
\|x\|_{\max }=\max \left\{\left|x_{i}\right|: i \in\{1,2, \ldots, n\}\right\} \quad \text { für } x=\left(\begin{array}{c}
x_{1} \\
x_{2} \\
\vdots \\
x_{n}
\end{array}\right)
$$
Diese erfüllt nicht die Parallelogrammgleichung und ist somit ein Beispiel für eine Norm, die nicht von einem [[(euklidische) Skalarprodukt]] induziert wird.
^c-ndp2Ju0ptx
---
**Tags**:  