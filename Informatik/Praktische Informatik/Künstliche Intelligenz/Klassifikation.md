## Typen

### Generativ

Klassen anhand von ungelabelten Daten finden.
Sehr schwer zu lernen.

### Diskriminativ

Daten zu vordefinierte und gelabelte Klassen zuweisen.
Einfacher als Generation.

### Lineare Klassifikation

![[Pasted image 20250303170234.png]]
$$f(x) = w^T x + b$$

- 2D -> Linie, $w$ orthogonal zur Linie, $b$ ist $y$-Achsen Abschnitt ("bias")
- 3D -> Ebene
- $n$D -> Hyperebene

### Margin

Abstand zwischen Grenze und nächstem Datenpunkt
Großer Margin -> Hohes Vertrauen in Vorhersage
Kleiner Margin -> Vorhersage eventuell ungenau

### Loss Funktionen

### 0-1 Loss

Anzahl falsch klassifizierter Punkte ist minimal
NP-schwer zu optimieren

### MSE

- Mit [[Gradient Descent]] optimieren
- Labels sind 0 oder 1, nicht kontinuierlich -> nicht robust gegen Ausreißer

### Sigmoid Funktion

$$\sigma(a) = \frac{1}{1 + exp(-a)}$$
Werte sind glatt verteilt zwischen 0 und 1.
-> MSE Loss, indem wir auf $f(x_i)$ die Sigmoid Funktion anwenden, damit Gradient Descent funktioniert.
