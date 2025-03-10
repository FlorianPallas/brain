---
aliases:
  - Neurale Netzwerke
---

Neurale Netzwerke, meist Feed Forward Neural Networks, werden als azyklischer Graph dargestellt. Dieser zeigt die Verbindungen (Kanten) zwischen Neuronen (Knoten). Dabei werden Neuronen in Schichten (input, hidden, output) aufgeteilt.

Im Vergleich zu Algorithmen basierend auf [[Regression]], sind Neurale Netzwerke deutlich flexibler. Um nicht-lineare Zusammenhänge mit Regression zu erkennen, müssen wir dem Algorithmus die Funktion vorgeben. Ein Neurales Netzwerk erkennt den Zusammenhang ohne vorherige Annahmen.

## Layers

- $N$ Inputs, $M$ Outputs
- "Fully Connected": Alle Inputs mit Outputs verbunden
- Jeder Layer ist eine Gewichtsmatrix $\theta = M \times N$
- Berechnung: $y = \phi(\theta x + b)$

Warum mehrere Layer?
Erfahrung zeigt, dass zwar alle Probleme mit einem hidden Layer approximiert werden können, allerdings Neurale Netze mit mehreren Layers mit weniger Neuronen auskommen.

## Initialisierung

Zu Beginn müssen wir Standardgewichte hinterlegen. Das passiert meistens mittels Zufall.

Warum Initialisieren?
Wenn alle Gewichte gleich wären, hätten wir keinen wirklichen Gradienten. Zufällige Werte sorgen für eine bessere Umgebung.

## Aktivierungsfunktion

Die Aktivierungsfunktion entscheidet wann ein Neurone aktiviert wird. Dabei können wir verschiedene Funktionen nutzen.

![[Pasted image 20250304154851.png]]

Eine gute Aktivierungsfunktion muss folgende Eigenschaften erfüllen:
Immer guter Gradient: Schnelle Konvergenz
Outputs um 0 zentriert: Leichte Initialisierung
Günstige Funktion: Schnellere Berechnung

Fazit:

- ReLU sehr gut
- Leaky ReLU, ELU gut
- tanh maybe
- sigmoid niemals, außer für Klassifikation

## Training

Neurale Netzwerke werden mittels [[Back Propagation]] trainiert. Allerdings sind die Werte hier mehrdimensional, was es schwert macht das zu visualisieren. Der Ansatz bleibt gleich:

- Gradient berechnen
- In andere Richtung bewegen
- -> Loss minimieren

## Komplexität

Forward Propagation:

- Eine Multiplikation und Addition pro Gewicht
  Back Propagation:
- Zwei Multiplikationen und Additionen pro Gewicht
  Fazit:
- Kosten sind linear zu Gewichten
- Kosten sind linear zu Schichten
- Kosten sind quadratisch zu Neuronen pro Schicht
