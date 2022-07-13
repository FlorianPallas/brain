---
aliases: []
---

# Drehung #card
## Drehung in $\mathbb{R}^2$
Die Drehung ist gegeben durch folgende Drehmatrix:
$$
D_{\varphi}:=\left(\begin{array}{cc}
\cos \varphi & -\sin \varphi \\
\sin \varphi & \cos \varphi
\end{array}\right) \in \mathbb{R}^{2 \times 2}
$$
Die Matrix beschreibt eine Drehung $L_{\left.D_{\varphi}\right)}: \mathbb{R}^{2} \rightarrow \mathbb{R}^{2}, x \mapsto D_{\varphi} \cdot x$ um den Winkel $\varphi$ mit Zentrum im Ursprung. Die Drehung ist eine lineare [[Isometrie]]
![[Pasted image 20220713151719.png]]
## Drehung im $\mathbb{R}^3$
Die Drehung ist gegeben durch folgende Drehmatrix:
$$
D_{\varphi}:=\left(\begin{array}{cc}
\cos \varphi & -\sin \varphi  & 0\\
\sin \varphi & \cos \varphi & 0 \\
0 & 0 & 1
\end{array}\right) \in \mathbb{R}^{2 \times 2}
$$
Die Matrix beschreibt eine Drehung $L_{\left.D_{\varphi}\right)}: \mathbb{R}^{3} \rightarrow \mathbb{R}^{3}, x \mapsto D_{\varphi} \cdot x$ um den Winkel $\varphi$ mit Zentrum im Ursprung. Die **Drehachse** ist die $x_3$-Achse und die **Drehebene** ist die $x_1x_2$-Ebene. Durch geeignete Basiswahl kann jede Drehung im $\mathbb{R}^3$ mit der Matrix dargestellt werden.
## Allgemeine Drehungen
- Die Vektoren entlang der Drehachse (**Fixpunktvektoren**) sind [[Eigenvektor|Eigenvektoren]] mit einem [[Eigenwerte|Eigenwert]] von $1.$
- Die Drehmatrix ist [[orthogonale Gruppe|orthogonal]]
- Die Drehmatrix ist eine [[Isometrie]]
- Für reine Drehungen gilt: $\det(D) = 1$
## Prüfen einer Drehmatrix
1. Vektor $v$ [[Orthogonalität|orthogonal]] zur Drehachse wählen
2. $v'= D \cdot v$
3. $\varphi = \arccos \left( \dfrac{\lt v, v' \gt}{\mid \mid v \mid \mid \cdot \mid \mid v' \mid \mid} \right)$ 
^c-X3GPd92FFl
---
**Tags**: 