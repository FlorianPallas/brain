---
aliases: []
---

# Kruskal #card
## Idee
Wähle in jedem Schritt die minimale Kante unter allen Kanten, die keinen Kreis mit schon gewählten Kanten bilden und füge sie dem Spannbaum hinzu.
## Umsetzung
1. Sortiere die Kanten aufsteigend nach Kantengewicht
2. Betrachte die Kanten der Reihe nach. Es können zwei Fälle eintreten:
	1. Die Kante schließt einen Kreis -> Kante überspringen
	2. Die Kante schließt keinen Kreis -> Kante in den Spannbaum aufnehmen
^c-Sge0XgLKl1
---
**Tags**: 