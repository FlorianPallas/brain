---
aliases: []
---

# Minimale Spannbäume #card
## Problemstellung
Sei $G=(V, E)$ ein Graph mit Kantengewichten $w: E \rightarrow \mathbb{Z}$. Finde einen Spannbaum $T=\left(V, E_{T}\right)$, sodass die Summe der Gewichte in $E_{T}$ minimal ist.
## Allgemeine Bemerkung
Satz: Für jeden [[Graph|Schnitt]] gilt, dass die minimale Schnittkante in jedem MST enthalten ist.
## Algorithmen
Es gibt zwei [[Greedy-Algorithmus|Greedy-Algorithmen]] die das Problem lösen. Beide gehen ähnlich vor, indem sie in jedem Schritt die minimale Kante wählen, die
- [[Algorithmus von Prim]] unter allen Kanten, die den bisherigen Teilbaum vergrößern
- [[Kruskal]] unter allen Kanten, die keinen Kreis mit schon gewählten Kanten bilden
^c-0e3FZfRS2u
---
**Tags**: 