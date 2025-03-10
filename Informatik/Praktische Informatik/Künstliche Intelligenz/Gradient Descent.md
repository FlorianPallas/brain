## Vorgehen

- Beginne mit (zufälligem) Punkt
- Folge dem Gradienten -> Zeigt immer in Richtung des steilsten Anstiegs
  ![[Pasted image 20250304152500.png]]
  Lernrate / Schrittweite $\eta$

## Wahl der Lernrate

Zu Große Lernrate -> Oszillation, Divergenz
Zu Kleine Lernrate -> Langsame Konvergenz

## Abbruchkriterium

Änderung als Kriterium: Änderungs Threshold
Budget als Kriterium: Zeitschritt überschreitet kritischen Wert

## Stochastisch (SGD) vs Batch (BGD)

Batch -> Gut nah am Optimum
Stochastisch -> Gut weit weg vom Optimum, Weniger Berechnungen (Keine Dopplungen)
Mini Batches -> Mischung aus SGD und BGD, sehr effizient, weit verbreitet
