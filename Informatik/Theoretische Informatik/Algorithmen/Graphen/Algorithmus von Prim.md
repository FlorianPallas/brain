---
aliases: []
---

# Algorithmus von Prim #card
## Idee
- zeige, dass gewisse Kanten in jedem MST enthalten sind
- finde iterativ solche Kanten und wähle sie aus
- nach $n-1$ Schritten bilden die $n-1$ gewählten Kanten den MST
## Funktionsweise
1. Wähle einen beliebigen Knoten als Startknoten und markiere ihn als abgearbeitet.
2. Betrachte den Schnitt zwischen den abgearbeiteten und den nicht-abgearbeiteten Knoten und wähle die minimale Schnittkante.
3. Wiederhole 2. solange bis alle Knoten abgearbeitet sind.
## Effiziente Umsetzung
Das Auffinden der minimalen Schnittkante kann naiv in $O(m)$ erledigt werden. Effizienter ist es eine [[Priority-Queue]] einzusetzen. 
Dabei enthält die [[Priority-Queue]] die noch nicht-abgearbeiteten Knoten und die Priorität ist das minimale Kantengewicht zu abgearbeiteten Knoten (Hinweis: Viele Kanten werden vermutlich keine solche Kante haben. Bei ihnen wird die Priorität auf $\infty$ gesetzt).
Pro Schritt wird das Minimum der [[Priority-Queue]] abgearbeitet, die minimale Kante in den Spannbaum mit aufgenommen und es wird ggf. die Priorität der Nachbarn verringert.
## Laufzeit
- Naive Umsetzung: $\Theta(n \cdot m)$
- Effiziente Umsetzung (mit [[Binary-Heap]] als [[Priority-Queue]]): $\Theta((n+m)\cdot \log n)$
	- Es werden $n$ Knoten betrachtet und $n$ mal popMin() mit je $\Theta(\log n)$ aufgerufen
	- Es werden $m$ Kanten betrachtet und $m$ mal decPrio() mit je $\Theta(\log n)$ aufgerufen
- Effiziente Umsetzung (mit [[Fibonacci-Heap]] als [[Priority-Queue]]): $\Theta(n \cdot \log n + m)$
	- Es werden $n$ Knoten betrachtet und $n$ mal popMin() mit je $\Theta(\log n)$ aufgerufen
	- Es werden $m$ Kanten betrachtet und $m$ mal decPrio() mit je $\Theta(\log n)$ aufgerufen
## Algorithmus Klasse
Gehört zu den [[Greedy-Algorithmus|Greedy-Algorithmen]], da er in jedem Schritt die minimale Kante wählt, die den bisherigen Teilbaum vergrößert. Er geht dabei ähnlich wie [[Dijkstra]] vor, nur die Prioritäten werden leicht anders aktualisiert.
^c-4FjxAwrnC7
---
**Tags**: 