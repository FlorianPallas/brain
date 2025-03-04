---
aliases: []
---

# Programmierrichtlinien #card
## Motivation
- Konsistenter Stil erleichtert die Lesbarkeit,
- Beschleunigt Einarbeitung bei Personalwechsel und Wiedereinarbeitung,
- Zeitersparnis bei Fehlerfindung, Erweiterung und Pflege des Programms,
"Ein sauberer Stil ist Ehrensache"
- Muss konsistent angewandt werden: Einhaltung der Standards sollte bei Durchsichten und Inspektionen beachtet werden
- Aber: Nicht übertreiben! Alle Regeln mit Augenmaß anwenden.
## Problem
Es gibt keine allgemein anerkannten einheitlichen Programmierrichtlinien. Wichtig ist daher zunächst die Projekt-/Firmen-interne Einigung auf einen Standard!
## Guidelines aus Elements of Programming
- Write clearly - don't be too clever.
- Don't sacrifice clarity for efficiency.
- Don't patch bad code - rewrite it.
- Don't comment bad code - rewrite it.
- Make it right before you make it faster.
- Make it clear before you make it faster.
- Keep it right when you make it faster.
- Let your compiler do the simple optimizations
## Inhalte
### Formatierung
Einhalten der Konventionen
Bei Java: 4 Zeichen normale Einrückung und 8 Zeichen für Sonderzwecke
### Bezeichner
Aussagekräftig und Einhalten der Konventionen
- Bei Java:
	- Camle-Case-Notation für Variablen, Funktionen und Klassennamen
	- Upper-Case-Notation für Konstanten
	- Lower-Case-Notation für packages
### Funktionen
Nicht zu groß, Teilschritte in eigene Funktionen
### Kommentare
Merke: Lesbarer kommentarfreier Code ist besser als kommentierter, aber unlesbarer Code.
![[Pasted image 20220622133703.png]]
![[Pasted image 20220622133710.png]]
Es empfiehlt sich Dokumentationswerkzeuge wie u.a. JavaDoc zu verwenden.
^c-g4y9E28fSh
---
**Tags**: 