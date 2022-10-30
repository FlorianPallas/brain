---
aliases: []
---

# Normalbereich #card
## Definition
Eine [[Teilmenge]] $B \subseteq \mathbb{R}^{2}$ heißt **Normalbereich bezüglich der $x$-Achse**, wenn es ein Intervall $I=[a,b]$ und [[Stetigkeit|stetige]] Funktionen $f,g: I \to \mathbb{R}$ mit
$$
B=\{(x,y) \in \mathbb{R}^{2}: x \in I \land f(x)\leq y \leq g(x)\}
$$
Analog für **bezüglich der $y$-Achse** ($x$ wird durch $y$ getauscht).

$n$-dimensionale Normalbereiche können durch ihre Vorgänger-Normalbereiche (also $n-1$) und die Bedingung an eine weitere [[Komponente]] definiert werden.

## Integration
Aus dem [[Satz von Fubini]] folgt für Normalbereiche $B = \{(x,y) \in \mathbb{R}^{2}: x \in [a,b] \land f(x) \leq y \leq g(x)$ und $f: B \to \mathbb{R}$ [[Integrierbarkeit|integrierbar]]
$$
\int\limits_{B} f(x,y) d(x,y) = \int\limits_{a}^{b} \int\limits_{f(x)}^{g(x)} f(x,y) d(y,x)
$$

## Beispiele



---
**Tags**: #todo 