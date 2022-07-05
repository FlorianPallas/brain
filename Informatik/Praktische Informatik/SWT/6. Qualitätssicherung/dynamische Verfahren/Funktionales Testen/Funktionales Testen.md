---
aliases: []
---

# Funktionales Testen #card
## Ziel
Testen der spezifizierten Funktionalität
- Testfälle aus der Spezifikation ableiten
- Interne Struktur des Testlings nicht berücksichtigt weil für den Tester unbekannt
- Testfälle enthalten
	- Eingabedaten
	- Erwartete Ausgabedaten / Reaktion (soll)
- Vorteile:
	- Testfälle unabhängig von der Implementierung erstellbar (vorher oder gleichzeitig)
	- Vermeidet „Kurzsichtigkeit“ bei der Auswahl
- Nachteil:
	- mögl. kritische Pfade nicht bekannt und nicht getestet, da es oft nicht jede Kombination von Eingabedaten getestet werden kann
## Verfahren zur Testfallbestimmung
### Funktionale Äquivalenzklassenbildung
#### Annahme
Ein Programm/Modul reagiert bei der Verarbeitung eines Wertes aus einem bestimmten Bereich genau so wie bei der Verarbeitung jedes anderen Wertes aus diesem Bereich. Achtung: Der Wert muss nicht im Definitionsbereich der Eingabeparameter liegen! 
#### Ansatz
Zerlege Wertebereich der Eingabeparameter und Definitionsbereich der Ausgabeparameter in Äquivalenzklassen (ÄK).
- Bildung der Äquivalenzklassen (Ansatzidee)
	- Partitionierung ausgehend von einer großen ÄK
	- Aufteilung entlang Definitionsbereichsgrenzen
	- Aufteilung entlang anzunehmenden(!) Verarbeitungsmethodengrenzen
- Auswahl der Repräsentanten
	- Sei m die Anzahl der ÄK der Eingabeparameter und $n$ die Anzahl der ÄK der Ausgabeparameter.
	- Dann entstehen $\leq m \cdot n$ verschiedene ÄK aus denen jeweils 1 beliebiger Repräsentant zum Testen verwendet wird
#### Beispiel
![[Pasted image 20220705152314.png]]
![[Pasted image 20220705152325.png]]
![[Pasted image 20220705152333.png]]
### Grenzwertanalyse
Weiterentwicklung der funktionalen Äquivalenzklassenbildung
- Beobachtungen:
	- Off-by-one: Knapp daneben ist auch vorbei
	- Testfälle, die die Grenzen der Äquivalenzklassen und deren unmittelbare Umgebung abdecken sind besonders effektiv
$\Rightarrow$ Verwende nicht irgendein Element aus der ÄK, sondern solche auf und um den Rand (Annäherung von beiden Seiten)
Beispiel bei Monaten: 0 und 1, 12 und $13 .$
- Spezielle Kandidaten: 0, 1, MAX_INT, NaN, ...
### Zufallstest
- Testen der Funktion mit zufälligen Testfällen
- Beobachtung: Tester neigen dazu, Testfälle zu erzeugen, die auch bei der Implementierung als nahe liegend erachtet wurden (eine Art Betriebsblindheit)
- Vorteil: nichtdeterministisches Verfahren behandelt alle Testfälle gleich
- Sinnvoll als Ergänzung zu anderen Verfahren
- Sinnvoll wenn man viele Testfälle erzeugen möchte (z.B. für Sortierverfahren) und die Überprüfung der Korrektheit automatisch erfolgen kann.
- Sinnvoll als unterlagertes Kriterium (z.B. beim Verfahren der funktionalen ÄK-Bildung)
### Test von Zustandsautomaten
- Hat eine Komponente einen internen Zustand, können Testfälle aus den Zustandsübergängen abgeleitet werden
- Ziel: mindestens einmaliges Durchlaufen aller Übergänge
- Achtung:
	- Überdeckung aller Übergänge garantiert noch keinen vollständigen Test (vgl. Zweigüberdeckung)
	- Zum Nachvollziehen der Testsequenzen ist ggf. eine Instrumentierung der Komponente notwendig
^c-TVa49BLZ16
---
**Tags**: 