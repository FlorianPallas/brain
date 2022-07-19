---
aliases: []
---

# Refactoring #card
## Definition
Refactoring ist der Prozess, ein Softwaresystem so zu verändern, dass das externe Verhalten unverändert bleibt, der Code aber eine bessere Struktur erhält.
## Beispiele
- Umbenennen einer Variablen (und aller Zugriffe)
- Teilen einer Methode in zwei Methoden
- Verschieben einer Klasse in ein anderes Package
## Gründe für das Refactoring
- Lesbarkeit / Übersichtlichkeit / Verständlichkeit
	- Reduktion vom Komplexität, z.B. Aufteilen von Methoden Bewusste Benennung von Variablen, Methoden
- Wiederverwendung / Entfernen von Redundanz
	- Methoden aufteilen, um Teile wiederzuverwenden
	- Kopierte Quelltextfragmente in eine Methode extrahieren
- Testbarkeit
- Erweiterbarkeit
## Anwendung: Extract Method
- Turn a fragment into a method whose name explains the purpose of the method.
- Methode ist zu lang.
- Methode braucht Kommentare für Struktur/Verständnis.
- Kopiertes Codefragment in vielen Methoden benutzt.
- Starke Verzweigung innerhalb der Methode
![[Pasted image 20220719154731.png]]
## Weitere Refactorings
![[Pasted image 20220719154824.png]]
## Automatisiertes Refactoring
Viele Entwicklungsumgebungen (z.B. Eclipse, IntelliJ) automatisieren Refactorings

^c-dyisZSegXm
---
**Tags**: 