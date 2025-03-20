# Agenten
Agenten werden hauptsächlich an ihrer Rationalität und Autonomie klassifiziert.

## Autonom
- nimmt seine Umgebung wahr: Input
- agiert mit der Umgebung: Aktionen
- -> Kreislauf (Aktion, Reaktion)

## Rational
- wählt Handlungen die seinen erwarteten Nutzen maximieren
- Kostenfunktion kontrolliert Verhalten

## Planung vs Reflex
Reflex
- Agieren aufgrund der momentanen Wahrnehmung
- Bedenken nicht die Konsequenzen des Handelns
Planend
- Entscheiden aus Handlungsfolgen
- Brauchen ein Ziel und Modell für Auswirkungen ihrer Handlungen

## Umgebungseigenschaften
- Vollständig / teilweise beobachtbar
	- Eventuell Erinnerung (Speicher) notwendig
	- z.B. Pacman vs. FPS Labyrinth
- Diskret / kontinuierlich
	- Der Agent kann eventuell nicht alle Zustände aufzählen
	- z.B. Pacman vs. Bootrennen
- Deterministisch / Stochastisch
	- Zustandsübergänge sind unsicher
	- z.B. Pacman vs Blackjack
- Einzelagen / Multiagent
	- Agent muss sich ggf. zufällig verhalten
	- z.B. Pacman vs. Schach

# Suchproblem
Agenten für Suchprobleme stellen die einfachste Form von Planung dar. Da Suchprobleme in die Kategorien: vollständig beobachtbar, diskret, deterministisch, Einzelagent fallen.

Suchprobleme bestehen aus:
- Zustandsraum
- Nachfolgerfunktion
	- Mit Aktionen und Kosten
- Startzustand und Zielbedingung 

Suchprobleme werden gelöst durch die Abfolge von Aktionen (Plan), die den Startzustand in den Zielzustand überführen.

## State Space Graph
Suchprobleme können als Graph dargestellt werden. Wobei ein Lösung eine Verbindung zwischen Start- und Zielknoten darstellt.

## Suchbaum
Suchprobleme können in Baumform dargestellt werden, wobei die Wurzel der Startzustand ist, und Verzweigungen durch die möglichen Aktionen erzeugt werden, welche zu entsprechenden Knoten als neue Zustände führen. Dabei können "Duplikate" von Knoten existieren, da Zustände auf verschiedenen Wegen erreicht werden können.

Probleme die in einem endliche State Space Graph dargestellt werden können, können im Suchbaum unendlich werden!

## Fringe
Prioritätenliste, welche für die Abarbeitung von möglichen Aktionen genutzt wird.

# Suchverfahren
## Eigenschaften
- Ein Suchalgorithmus ist vollständig, wenn er garantiert eine Lösung findet.
- Ein Suchalgorithmus ist optimal, wenn er garantiert die beste Lösung findet.

# Uninformierte Suchverfahren
Suchverfahren die ohne Informationen über den Zustandsraum agieren.
[[Baumsuche]]
[[DFS]]
[[BFS]]
[[UCS]]

# Heuristische Suchverfahren
Suchverfahren die mittels einer [[Heuristik]] Entscheidungen treffen.
[[A*]]

# Baumsuche
Die generelle Baumsuche initialisiert den Fringe mit dem Startknoten und exploriert einen Fringe Knoten nach einer vorgegebenen Strategie. Ist dieser ein Zielknoten, terminiert der Algorithmus mit dem entsprechenden Pfad. Wenn nicht, werden alle Nachbarknoten dem Fringe hinzugefügt, und der Algorithmus wählt den nächsten Knoten.

- Zuerst den tiefsten, neusten Knoten wählen: Depth-First Search (DFS)
	- Umsetzung mit LIFO Queue
	- Nicht optimal, bei Zyklen unvollständig
	- Kein Spezialfall von A*, keine FIFO Queue
- Zuerst den flachsten Knoten wählen: Breadth-First Search (BFS)
	- Umsetzung mit FIFO Queue
	- Nicht optimal, bei Zyklen unvollständig
	- Spezialfall von A*, wenn h=0, und alle Kanten gleiche Kosten haben
- Zuerst den billigsten Knoten wählen: Uniform-Cost Search (UCS)
	- Umsetzung mit Priority Queue, Priorität: akkumulierte Kosten des Pfades vom Start zum Knoten (Rückwärtskosten)
	- optimal (vgl. A*), vollständig mit endliche, positive Kosten
	- Spezialfall von A*, wenn h =0
	- Ähnlich zu [[Dijkstra]]

# Heuristik
Eine Funktion, die schätzt, wie nahe ein Zustand am Ziel ist
z.B. Manhatten Distance, Euklidic Distance

## Unzulässig / Pessimistisch
- Führen zu suboptimalen Ergebnissen, da sie gute Pläne ausschließen
- Werte auch über den tatsächlichen Kosten

## Zulässig / Optimistisch
- Verhindern schlechte Pläne, unterschätze aber die tatsächlichen Kosten
- Werte stets zwischen 0 und den tatsächlichen Kosten liegen
- Meistens Vereinfachungen eines Problems (z.B. Luftlinie)

## Konsistenz
- Auf Graphen relevant
- Jeder Pfad zwischen Knoten muss kleiner gleich den tatsächlichen Kosten sein
- Impliziert Zulässigkeit
- Meiste Heuristiken sind konsistent, vor allem bei Vereinfachungen

## Beispiele
- Manhattan Distance: $|x_1 - x_2| + |y_1 - y_2|$
- Euclidean Distance: $\sqrt{(x_2-x_1)^2+(y_2-y_1)^2}$

# Greedy Search
Sortiere Fringe nach Zielnähe via [[Heuristik]] (Vorwärtskosten).

# A*
Sortiere nach der Summe von Vorwärts- und Rückwärtskosten (vgl. UCS, Greedy Search). Die Heuristik summiert daher die akkumulierten Kosten des Knotens vom Startknoten, und das Ergebnisse der Heuristik zum Zielknoten.

## Baumsuche
Mit **zulässiger** [[Heuristik]] dehnt A* seine Kontur Richtung Ziel aus, exploriert diese Knoten also früher, schließt andere aber nicht aus. So ist die optimalen Lösung garantiert.

## Graphsuche
Für Graphen muss die Heuristik zusätzlich **konsistent** sein.

## Anwendungen
- Videospiele
- Routenplanung
- Scheduling

# Graph Suche
- Niemals einen Zustand zweimal explorieren
