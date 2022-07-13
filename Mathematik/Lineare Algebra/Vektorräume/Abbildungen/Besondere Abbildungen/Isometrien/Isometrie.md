---
aliases: []
---

# Isometrie #card
## Definition
Seien $(V,\|\cdot\|)$ und $(W, \mid \mid \mid \cdot \mid \mid \mid)$ [[Norm|normierte]] [[Vektoraum|Vektorräume]]. Eine [[Abbildung]] (muss nicht linear sein) $f: V \rightarrow W$ heißt Isometrie, falls für alle $x, y \in V$ gilt
$$
\mid \mid \mid f(x)-f(y) \mid \mid \mid =\|x-y\| .
$$
Die Menge aller bijektiven Isometrien von $V$ nach $V$ wird bezeichnet mit Is $(V,\|\cdot\|)$ oder auch kürzer mit Is $(V)$.
## Eigenschaften
- Jede Isometrie ist injektiv.
- Die Umkehrabbildung einer bijektiven Isometrie ist ebenfalls eine Isometrie.
- Die Verkettung zweier Isometrien ist wieder eine Isometrie.
## Hinweise
- Die Menge Is $(V)$ ist eine Untergruppe der Gruppe aller bijektiven Selbstabbildungen von $V$ nach $V$.
- Eine Isometrie ist nicht notwendigerweise eine lineare Abbildung wie man am Beispiel einer Translation $\tau_{v}: V \rightarrow V, \quad x \mapsto x+v$ um einen festen Vektor $v \neq 0$ erkennen kann.
## Kriterien für euklidische und unitäre Vektorräume
Es seien $(V,\langle\cdot, \cdot\rangle)$ und $(W, \ll \cdot \cdot \gg)$ Vektorräume mit [[Standardskalarprodukt]] über demselben Körper $(\mathbb{R}$ oder $\mathbb{C}$ ), und $f: V \rightarrow W$ eine [[Lineare Abbildung]]. Dann sind folgende Aussagen äquivalent:
- $f$ ist eine Isometrie.
- $\ll f(x), f(y) \gg=\langle x, y\rangle$ für alle $x, y \in V$.
- $\ll f(x), f(x) \gg=\langle x, x\rangle$ für alle $x \in V$.
- $\ll f(x), f(x) \gg=1 \quad$ für alle Einheitsvektoren $x \in V$.
## Weitere Sätze
### Orthonormal
Es seien $(V,\langle\cdot, \cdot\rangle)$ und $(W, \ll \cdot, \gg)$ Vektorräume mit Skalarprodukt über demselben Körper $(\mathbb{R}$ oder $\mathbb{C}$ ), und $f: V \rightarrow W$ eine lineare Abbildung. Dann ist $f$ eine Isometrie genau dann, wenn jede orthonormierte Teilmenge von $V$ injektiv auf eine orthonormierte Teilmenge von $W$ abgebildet wird.
Ist zusätzlich $V$ endlich-dimensional, so ist $f$ eine Isometrie genau dann, wenn eine Orthonormalbasis von $V$ injektiv auf eine orthonormierte Teilmenge von $W$ abgebildet wird.
### Abbildungsmatrizen
Sei $\mathbb{K}=\mathbb{R}$ beziehungsweise $\mathbb{K}=\mathbb{C}, \mathbb{K}^{n}$ der Standardvektorraum versehen mit dem [[(euklidische) Skalarprodukt]] beziehungsweise [[unitäres Skalarprodukt]] und $f \in \operatorname{End}\left(\mathbb{K}^{n}\right)$. Dann ist $f$ eine Isometrie genau dann, wenn $f=L_{A}: \mathbb{K}^{n} \rightarrow \mathbb{K}^{n}, x \mapsto A \cdot x$ gilt für eine Matrix $A \in \mathrm{O}(n)$ ([[orthogonale Gruppe]]) beziehungsweise $A \in \mathrm{U}(n)$ ([[unitäre Gruppe]]).
### Orthonormalbasis
Ist $(V,\langle\cdot, \cdot\rangle)$ ein endlich-dimensionaler euklidischer oder unitärer Vektorraum, $B=\left(b_{1}, b_{2}, \ldots, b_{n}\right)$ eine Orthonormalbasis von $V$ und $f \in \operatorname{End}(V)$, so sind folgende Aussagen äquivalent:
- $f$ ist eine Isometrie.
- $f(B)=\left(f\left(b_{1}\right), f\left(b_{2}\right), \ldots, f\left(b_{n}\right)\right)$ ist eine Orthonormalbasis von $V$.
- $D_{B B}(f)$ ist eine orthogonale beziehungsweise eine unitäre Matrix.
^c-taDcw9CIoX
---
**Tags**: 