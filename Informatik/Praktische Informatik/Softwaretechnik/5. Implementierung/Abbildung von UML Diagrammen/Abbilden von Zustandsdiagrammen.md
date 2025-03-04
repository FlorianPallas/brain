---
aliases: []
---

# Abbilden von [[Zustandsdiagramm|Zustandsdiagrammen]] #card
## Implizite Speicherung des Zustands
- Der Zustand des Objektes kann aus den Attributwerten eines Exemplars „berechnet“ werden 
- Keine dedizierten Instanzvariablen nötig, der Zustand muss aber jedes Mal neu berechnet werden
- Zustandsübergangsfunktion ist implizit
### Beispiel
![[Pasted image 20220622170028.png]]
## Explizite Speicherung des Zustands
- Der Zustand eines Objektes wird in dedizierten Instanzvariablen gespeichert und kann daher einfach gelesen und neu gesetzt werden
- Die Zustandsübergangsfunktion muss ebenfalls explizit angegeben werden
### Beispiel
![[Pasted image 20220622170152.png]]
## Vergleich
- Die implizite Speicherung spart Speicherplatz, die explizite (potentiell) Rechenzeit.
- Die implizite Speicherung ist potentiell komplizierter (trickreicher), die explizite umfangreicher.
- Die explizite Speicherung ist immer offensichtlich und wird daher bei Änderungen wahrscheinlicher berücksichtigt.
- Die implizite Speicherung ist nicht immer möglich, die explizite schon.
## Alternativen
### Eingebettete Speicherung des Zustands
Jede Methode „kennt" den kompletten Automaten.
- Sie führt ihre Aufgabe kontextsensitiv (= dem aktuellen Zustand entsprechend) durch und Nimmt die Zustandsübergänge selbst vor
- Implementiert als eine große Fallunterscheidung pro Methode (switch- oder if-Anweisungen)
- Vorteil: kompakter, schneller
### Ausgelagerte Speicherung des Zustands
- Die Methode läuft im aktuellen Zustand, der ein Objekt ist.
- Der Code zur Reaktion und Änderung der Zustände befindet sich in dedizierten (ggf. automatisch erzeugten) Klassen
- Die Äste der Fallunterscheidung sind auf gleichnamige Methoden verteilt (a la Strategie-Muster)
- Vorteil: flexibler, bei komplexen Automaten übersichtlicher
### Ausgelagerte explizite
^c-W4wTclpsQu
---
**Tags**: #todo 