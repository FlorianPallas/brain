---
aliases: []
---

# Isometrienormalform #card
## Euklidische Normalform
(Euklidische Normalform). Sei $(V,\langle\cdot, \cdot\rangle)$ ein euklidischer Vektorraum mit $\operatorname{dim} V=n$, und $f \in \operatorname{End}(V)$ eine lineare [[Isometrie]]. Dann gibt es eine Orthonormalbasis $B$ von $V$, sodass für die Abbildungsmatrix $D_{B B}(f)$ von $f$ bezüglich $B$
$$
D_{B B}(f)=\left(\begin{array}{ccccc}
I_{r} & & & & 0 \\
& -I_{S} & & & \\
& & D_{\omega_{1}} & & \\
& & & \ddots & \\
0 & & & & D_{\omega_{\ell}}
\end{array}\right)
$$
gilt. Dabei sind $\omega_{i} \in(0, \pi)$ und $D_{\omega_{i}} \in \mathrm{SO}(2)$ für $i \in\{1,2, \ldots, \ell\}$ Drehmatrizen wie in Lemma 3. Die Parameter $r, s, \ell, \omega_{1}, \ldots \omega_{\ell}$ sind durch $f$ eindeutig bestimmt, und es gilt $r+s+2 \ell=n$
## Unitäre Normalform
(Unitäre Normalform). Sei $(V,\langle\cdot, \cdot\rangle)$ ein unitärer Vektorraum mit $\operatorname{dim} V=n$, und $f \in \operatorname{End}(V)$ eine lineare Isometrie. Dann gibt es eine Orthonormalbasis $B$ von $V$, die aus Eigenvektoren von $f$ besteht. Insbesondere gilt für die Abbildungsmatrix $D_{B B}(f)$ von $f$ bezüglich $B$
$$
D_{B B}(f)=\left(\begin{array}{ccc}
\lambda_{1} & & 0 \\
& \ddots & \\
0 & & \lambda_{n}
\end{array}\right)
$$
mit $\lambda_{i} \in \mathbb{C},\left|\lambda_{i}\right|=1$ für $i \in\{1,2, \ldots, n\}$.
## Herleitende Eigenschaften
### Lemma 1
Sei $(V,\langle\cdot, \cdot\rangle)$ ein euklidischer oder unitärer Vektorraum, und $f \in \operatorname{End}(V)$ eine lineare Isometrie.
(a) Für jeden Eigenwert $\lambda$ von $f$ gilt $|\lambda|=1$.
(b) Sind $\lambda$ und $\mu$ Eigenwerte von $f$ mit $\lambda \neq \mu, v \in E_{\lambda}$ und $w \in E_{\mu}$, so gilt
$$
\langle v, w\rangle=0 .
$$
### Lemma 2
Es sei $(V,\langle\cdot, \cdot\rangle)$ ein euklidischer oder unitärer Vektorraum und $f \in \operatorname{End}(V)$ eine lineare Isometrie. Weiter sei $U \subset V$ ein endlich-dimensionaler $f$-invarianter Untervektorraum. Dann ist das orthogonale Komplement $U^{\perp}$ ein $f$-invariantes Komplement von $U$, das heißt
$$
f\left(U^{\perp}\right) \subset U^{\perp} \quad \text { und } \quad V=U \oplus U^{\perp} .
$$
### Lemma 3 - Basiswechsel zur unitären Normalform
Zu jeder unitären Matrix $A \in \mathrm{U}(n)$ gibt es eine unitäre Matrix $S \in \mathrm{U}(n)$ und komplexe Zahlen $\lambda_{1}, \lambda_{2}, \ldots, \lambda_{n} \in \mathbb{C}$ mit $\left|\lambda_{i}\right|=1$ für $i \in\{1,2, \ldots, n\}$ sodass
$$
\bar{S}^{\top} \cdot A \cdot S=\left(\begin{array}{ccc}
\lambda_{1} & & 0 \\
& \ddots & \\
0 & & \lambda_{n}
\end{array}\right)
$$
### Lemma 4 - Drehkästchen
Sei $(V,\langle\cdot, \cdot\rangle)$ ein euklidischer Vektorraum mit $\operatorname{dim} V=n, u n d ~ f \in \operatorname{End}(V)$ eine lineare Isometrie. Besitzt das charakteristische Polynom $\chi_{f}$ von $f$ eine nichtreelle Nullstelle $\lambda \in \mathbb{C} \backslash \mathbb{R}$, so gilt:
(a) $\lambda=\cos (\omega)+\mathrm{i} \sin (\omega)$ für ein $\omega \in(0,2 \pi) \backslash\{\pi\}$.
(b) Es existiert ein $f$-invarianter Untervektorraum $U$ von $V$ mit $\operatorname{dim} U=2 .$
(c) Es gibt eine Orthonormalbasis $C$ von U sodass
$$
D_{C C}(f \mid u)=\left(\begin{array}{cc}
\cos (\omega) & -\sin (\omega) \\
\sin (\omega) & \cos (\omega)
\end{array}\right)=D_{\omega} \in \operatorname{SO}(2)
$$
### Lemma 5 - Basiswechsel zur euklidischen Normalform
Zu jeder orthogonalen Matrix $A \in \mathrm{O}(n)$ gibt es eine orthogonale Matrix $S \in \mathrm{O}(n), r, s, \ell \in\{1,2, \ldots, n\}$ mit $r+s+2 \ell=n$, sowie $\omega_{1}, \omega_{2}, \ldots \omega_{\ell} \in(0, \pi)$ sodass
$$
\widetilde{A} = S^T \cdot A \cdot S=\left(\begin{array}{ccccc}
I_{r} & & & & 0 \\
& -I_{S} & & & \\
& & D_{\omega_{1}} & & \\
& & & \ddots & \\
0 & & & & D_{\omega_{\ell}}
\end{array}\right)
$$
## Bestimmung der Kästchen
### naheliegende (aber aufwändigere) Variante
Die Kästchen ergeben sich aus den Eigenwerten. Hierzu können einfach alle Eigenwerte der Matrix bestimmt werden.
#### Fixpunktvektoren
Die Vektoren die sich bei dem Anwenden der Drehmatrix nicht verändern sind die sogenannten Fixpunktvektoren. Diese gehören zu dem [[Eigenwerte|Eigenwert]] $1$.
#### Spiegelachsen
Die Vektoren an denen entlang gespiegelt werden gehören zu dem [[Eigenwerte|Eigenwert]] $-1$
#### Drehkästchen
Zu einem Drehkästchen gehören zwei [[Eigenwerte]] $\lambda$ und $\bar{\lambda}$. Die Sinus und Kosinus Anteile werden über folgende Formel berechnet: $\lambda = \cos \varphi + i \sin \varphi$ 

### Transpositions-Trick Variante
Ist $A \in \mathrm{O}(n)$, so ist die Matrix $B:=A+A^{\top}$ diagonalisierbar mit reellen Eigenwerten vom Betrag $\leq 2$. Da nach Lemma 1 gilt $\mid \lambda \mid =1$ und es gilt:
$$
B \cdot v = (A + A^T)(v)=(A + A^{-1})(v)=A \cdot v + A^{-1} \cdot v= \lambda \cdot v + \frac{1}{\lambda} \cdot v = (\lambda + \frac{1}{\lambda})(v)
$$
#### Fixpunktvektoren
Ist $+2$ Eigenwert von $\mathrm{B}$ mit Vielfachheit $r$, so ist $+1$ Eigenwert von A mit derselben Vielfachheit $r$.
#### Spiegelachsen
Ist -2 Eigenwert von $\mathrm{B}$ mit Vielfachheit s, so ist $-1$ Eigenwert von $A$ mit derselben Vielfachheit s.
#### Drehkästchen
Ist $\lambda \in(-2,2)$ Eigenwert von $B$ mit Vielfachheit $2 \ell$, so hat die Normalform von $A$ genau $\ell$ Drehkästchen $D_{\omega} \in \mathrm{SO}(2)$, wobei $\omega \in(0, \pi)$ eindeutig bestimmt ist durch die Gleichung $2 \cos \omega=\lambda$. Es gilt außerdem: $\sin^2 \varphi = \sqrt{1- \cos^2 \varphi}$

## Bestimmung der Basis
### naheliegende (aber aufwändigere) Variante
1. Bestimmen der Kästchen
2. Mittels dem [[Gram-Schmidt-Verfahren]] je eine [[Orthonormalbasis]] der [[Eigenraum|Eigenräume]] $E_A(1)$ und $E_A(-1)$ bestimmen
3. Berechnen der [[Eigenraum|Eigenräume]] der übrigen [[Eigenwerte|Eigenwert]]-Paare von $A$
	1. Bestimme eine Orthonormalbasis $\left(z_{1}, z_{2}, \ldots, z_{j}\right)$ des Eigenraums zum Eigenwert $\lambda$ in $\mathbb{C}^{n}$.
	2. Für $i=1,2, \ldots, j$ setze
$$
\begin{aligned}
&x_{i}=\frac{1}{\mathrm{i} \sqrt{2}}\left(z_{i}-\overline{z_{i}}\right) \in \mathbb{R}^{n} \\
&y_{i}=\frac{1}{\sqrt{2}}\left(z_{i}+\overline{z_{i}}\right) \in \mathbb{R}^{n}
\end{aligned}
$$
		Nach Lemma 4 Drehkästchen ist $B_{i}:=\left(x_{i}, y_{i}\right)$ eine Orthonormalbasis eines Untervektorraums $U_{i}$ von $\mathbb{R}^{n}$, auf dem $A$ durch eine Drehmatrix $D_{\omega_{i}}$ dargestellt wird. Gilt $\omega_{i} \in(\pi, 2 \pi)$, so wähle $B_{i}:=\left(y_{i}, x_{i}\right)$.
### Transpositions-Trick
Die [[Eigenvektor|Eigenvektoren]] von der Abbildungsmatrix $A$ sind auch Eigenvektoren der Matrix $B$ (siehe obigen Abschnitt zum Transpositions-Trick). Die Matrix B enthält üblicherweise viel mehr Nulleinträge und ist symmetrisch
1. Bestimmen der Kästchen
2. Mittels dem [[Gram-Schmidt-Verfahren]] je eine [[Orthonormalbasis]] der [[Eigenraum|Eigenräume]] $E_B(1)$ und $E_B(-1)$ bestimmen
3. Berechnen der [[Eigenraum|Eigenräume]] der übrigen [[Eigenwerte]] von $B$
4. Es gibt folgende zwei Möglichkeiten
	- Berechnen der Determinante der Basiswechselmatrix. Diese ist die [[Summenraum|direkte Summe]] der [[Eigenvektor|Eigenvektoren]]. Ist die Determinante $-1$ so muss eine ungerade Anzahl an [[Eigenvektor|Eigenvektoren]] zu Drehkästchen getauscht werden. oder 
	- Zum Überprüfen ob $b_j$ und $b_{j+1}$ in der richtigen Reihenfolge sind muss gelten $S^T \cdot A \cdot b_j = \widetilde{A} \cdot e_j.$ Dies kann leicht nachgerechnet werden.

^c-rj3e9uYPKG
---
**Tags**: 