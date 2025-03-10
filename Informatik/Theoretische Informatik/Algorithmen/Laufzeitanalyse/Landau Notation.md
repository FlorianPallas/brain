---
aliases: [Laufzeit]
---

# Landau Notation

## Motivation

Die Landau Notation wird verwendet, um die Laufzeit von Algorithmen in Klassen einteilen zu können. Es werden grobe Laufzeitklassen gebildet, da es zu aufwändig und unpraktikabel ist einen Algorithmus ins Detail zu analysieren.

## Definitionen

### Original Definition

![[Pasted image 20220420162108.png]]

### Grenzwert Definition

![[Pasted image 20220420162729.png]]

## Ordnung auf Funktionen

![[Pasted image 20220420162332.png]]
![[Pasted image 20220420163015.png]]
Merke: Alle Logarithmen wachsen langsamer als [[Polynom|Polynome]] mit positiven reellen Exponenten

## Rechenregeln

![[Pasted image 20220420162416.png]]
![[Pasted image 20220420162430.png]]
![[Pasted image 20220420162446.png]]

- $\sum_{i} c^{i}$ wird asymptotisch vom größten Summanden dominiert, also: $\sum_{i=a}^{b} c^{i} \in \Theta\left(c^{a}+c^{b}\right),$ falls $c \neq 1$. Die Indizes $a$ bis $b$ dürfen von $n$ abhängen.
- $\log (n !) \in \Theta(n \log n)$

## Rechentipps

- Abschätzungen sind in der Ungleichung erlaubt, sofern diese die Ungleichung einschränken.
- Oft bietet sich an den Logarithmus zu ziehen
- Manchmal bietet sich Substitution an

## Anmerkungen

- $\Theta$ ist eine [[Äquivalenzrelation]]
- $\Theta (n \log n)$ wird als quasi-linear bezeichnet

## Beispiel: Ist $10+n^{2} \in o\left(2^{n}\right)?$

$\lim _{n \rightarrow \infty} 10+n^{2}=\infty \wedge \lim _{n \rightarrow \infty} 2^{n}=\infty \Rightarrow$ I'Hopital anwenden

$$

\lim _{n \rightarrow \infty} \left|\frac{10+n^{2}}{2^{n}}\right| \stackrel{\text { l'Hospital }}{=} \lim _{n \rightarrow \infty}\left|\frac{2 \cdot n}{\log (2) \cdot 2^{n}}\right| \stackrel{\text { l'Hospital }}{=} \lim _{n \rightarrow \infty}\left|\frac{2}{\log ^{2}(2) \cdot 2^{n}}\right| =0


$$
