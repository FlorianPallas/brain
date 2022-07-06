---
aliases: []
---

# Testwerkzeuge #card
## Arten
### Manuel
#### Printf-Debuging
Sich wichtige (Variablen-)Werte auf der Konsole ausgeben lassen
#### Interaktiver-Debugger
Variablen an Haltepunkten oder durch einen Ablauf verfolgen
Nachteil: Mühsam und unpraktisch
### Automatisiert
#### Zusicherungen (engl. assertions)
Boolesche Funktionen, um Vor-, Nachbedingungen oder Invarianten zu definieren
- Praxis: 
	- Öffentliche Methoden lieber mit Exceptions absichern, damit Klientprogramme darauf reagieren können. 
	- In private Methoden sollten Eingabeparameter, Nachbedingungen und Invarianten mit Zusicherungen überprüft werden, da eine Verletzung dieser einen unerwarteten Defekt darstellt.
#### Automatisch Ablaufende Testfälle, die sich selbst überprüfen
- Überprüfen Ergebnis ihrer Ausführung selbst
- Rückgabe: boolescher Wert (erfolgreich oder fehlgeschlagen)
- Optional: Auslösen einer Ausnahme bei Fehlschlag
- Können zu großen Testmengen zusammengesetzt werden.
- Können beliebig oft ausgeführt werden (täglich, stündlich, bei jede Änderung).
- Können als [[Regressionstest]] benutzt werden.
- Beispiel: [[JUnit]]
#### Prüfprogramme
- Checkstyle
- SpotBugs
^c-thnnjpybMK
---
**Tags**: 