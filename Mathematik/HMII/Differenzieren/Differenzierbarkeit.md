---
aliases: [differenzierbar, Ableitung, Differenzenquotient, Differenzenquotienten]
---

# Differenzierbarkeit
## Definition
Eine [[Funktion]] $f: I \to \mathbb{R}$ heißt **in $x_{0}$ differenzierbar**, genau dann wenn der [[Mathematik/HMII/Konvergenz/Grenzwert]] des **Differenzenquotienten**
$$
\lim\limits_{x \to x_{0}} \frac{f(x) - f(x_{0})}{x - x_{0}}
$$
existiert. Äquivalent ist: Es existiert
$$
\lim\limits_{h \to 0} \frac{f(x_{0}+h) - f(x_{0})}{h}
$$
In diesem Fall heißt der obige Grenzwert die **Ableitung** von $f$ in $x_{0}$ und wird mit $f'(x_{0})$ bezeichnet.

Ist $f$ in jedem $x \in I$ differenzierbar, so heißt **$f$ auf $D$ differenzierbar** und die Ableitung $f'(x)$ ist gegeben durch $x \mapsto f'(x)$.

### Bemerkungen
Eine Verkettung von differenzierbaren Funktionen ist im Allgemeinen wieder differenzierbar.

Ist eine Funktion differenzierbar, so ist sie ebenso stetig. Die Umkehrung gilt im Allgemeinen nicht. #relation 

## Regeln
Es gelten die bekannten Ableitungsregeln.

## Ableitung der Umkehrfunktion
Sei $f$ auf $I$ stetig, streng monoton und in $x_{0}$ differenzierbar mit $f'(x_{0}) \neq 0$, dann ist die Umkehrfunktion $f^{-1}$ differenzierbar in $y_{0} := f(x_{0})$. Es gilt
$$
(f^{-1})'(y_{0}) = \frac{1}{f'(x_{0})} = \frac{1}{f'(f^{-1}(y_{0}))}
$$

---
# Differenzierbarkeit im $\mathbb{R}^{n}$
## Definition
Eine vektorwertige Funktion $f: D \subseteq \mathbb{R}^{n}\to \mathbb{R}^m$, geschrieben $f(x) = (f_1(x),f_2(x),\dots,f_m(x))$ heißt partiell differenzierbar in $u$, wenn alle $\frac{\partial f_i}{\partial x_j}(u)$ existieren. Es existiert die [[Jacobi-Matrix]] $J_f$.

Eine Funktion $f: D\subseteq \mathbb{R}^{n}\to \mathbb{R}^m$ heißt [[Totale Differenzierbarkeit|differenzierbar]] in $u \in D$, wenn alle Koordinatenfunktionen $f_i$ in $u$ db. sind. Dann gilt: $f'(u) := J_f(u)$.

## Beispiele
![[Pasted image 20220531105938.png|400]]

---
**Tags**: #todo 