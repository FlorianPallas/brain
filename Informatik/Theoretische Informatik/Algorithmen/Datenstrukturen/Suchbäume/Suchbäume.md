---
aliases: []
---

# Suchbäume #card
## Motivation
Eine dynamisch sortierte Folge zu speichern. 
- In einem [[Sortieren|sortierten]] [[Array]] ist das Ändern eines Eintrags teuer, da der geänderte Eintrag vermutlich verschoben werden muss. Dies benötigt $\Theta(n).$ Das Finden eines Eintrags ist mit [[Binäre Suche]] in $\Theta(\log n)$ möglich.
- In einer [[Liste]] ist das Auffinden eines Eintrags mit $\Theta(n)$ teuer. Das Verschieben eines geänderten Eintrags benötigt ebenso $\Theta(n).$
Ein Suchbaum unterstützt in $\Theta(\log n)$ das Auffinden eines Elements und das Verschieben eines geänderten Eintrags in $\Theta(\log n)$
## Theoretisches Konstrukt
[[Binary-Tree]]
## Implementierungen
- Halbwegs binär und perfekt balanciert: [[(2,3)-Tree]]
- Binär und halbwegs balanciert: [[Red-Black-Tree]]
^c-vA1gPUIb6W
---
**Tags**: 