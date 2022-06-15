---
aliases: [partiell differenzierbar, pdb., stetig partiell differenzierbar, stetig pdb.]
---

# Partielle Differenzierbarkeit
## Definition #card
Die [[Funktion]] $f: D \subseteq \mathbb{R}^{n}\to \mathbb{R}$ ($D$ [[offene Mengen|offen]]) heißt in $x_0$ **partiell [[Differenzierbarkeit|differenzierbar]]** (**pdb**) nach $x_i$, genau dann wenn folgender [[Grenzwert]] existiert:
$$f_{x_i}(x_{0}):= \frac{\partial f}{\partial x_i} := \lim_{t \to 0} \frac{f(x_0+t_{e_{i})}-f(x_0)}{t}\in \mathbb{R}$$
(Steigung entlang der $i$-ten Achse von $x_0$ aus)
In diesem Fall heißt $f_{x_i}(x_0)$ die partielle Ableitung von $f$ in $x_0$ nach $x_i$.

### Stetige Differenzierbarkeit
$f$ heißt **$m$-mal pdb.** wenn in jedem $x_0$ alle $m$-fachen partiellen Ableitungen von f existieren. Wenn zusätzlich alle Funktionen
$$
\forall k \leq m \forall k \in \{1,...,n\}

\frac{\partial^{k}f}{\partial x_{i_{1}} \partial x_{i_{2}} \; ... \; \partial x_{i_{k}}}: D \to \mathbb{R}
$$
[[Stetigkeit|stetig]] sind, dann heißt $f$ **$m$-mal stetig pdb.**

### Höhere Ableitungen
Bei höheren Ableitungen schreibt man auch
$$
\frac{\partial^{3}t}{\partial x \partial y \partial z} = \frac{\partial t}{\partial x} \left(\frac{\partial t}{\partial y} \left(\frac{\partial t}{\partial z}\right)\right)= f_{zyx}
$$
Man beachte die unterschiedliche Darstellung der Reihenfolge der Ableitungen.
^c-9iuIW1Xdom

## Konzept #card
Man fasst (vorübergehend) alle bis auf eine Variable $x_i$ als Konstante auf und leitet nach dieser Variable $x_i$ ab. Man erhält die partielle Ableitung $f_{x_i}(x_0)$ von $f$ nach $x_i$.
^c-6PVuA8qTPJ

## Regeln
Die Rechenregeln fürs [[Differenzierbarkeit|Ableiten]] gelten auch für partielle Ableitungen. An Abschnittsgrenzen muss man den Differenzialquotienten manuell untersuchen.

### Satz von Schwarz
Ist $f \in C^m(D)$, so sind alle partiellen Ableitungen von $f$ bis zur Ordnung $m$ unabhängig von der Reihenfolge der Ableitungen.
$$
f_{xyz} = f_{zyx} = f_{yxz} = \; ...
$$

## Verfahren #card
- Bei potentiell nicht-pdb. Funktionen auf eine Abschnittsgrenze prüfen an dem gegebenen Punkt. Gegebenenfalls obige Definition nutzten, statt Regeln anzuwenden.
    - Obigen Grenzwert wenn möglich bestimmen
    - Existiert der Grenzwert nicht, so ist $f$ in $x_0$ nicht pdb.
- Ableiten nach der gegebenen Variable
- Koordinatenwerte einsetzen
^c-Ne0wD4X16d

## Beispiele
### In allen Punkten partiell differenzierbar
![[Pasted image 20220517100206.png|500]]

### Stellenweise nicht partiell differenzierbar
![[Pasted image 20220517101348.png|500]]

### Auf Intervallen definierte Funktion
![[Pasted image 20220517110933.png|500]]

---
**Tags**: 