## Übersicht
[Altklausuren](https://i11www.iti.kit.edu/teaching/winter2022/tgi/index)

- [x] Nerode Relation
- [x] Kodierungen
- [x] Automaten
	- [x] Moore Automat
	- [x] Mealy Automat
	- [x] Kellerautomaten
- [x] TMs
- [x] Mächtigkeit
- [x] Entscheidbarkeit
- [x] NP Vollständigkeit
- [x] Approximationsalgorithmen
- [x] Reguläre Sprachen
	- [x] Pumping Lemma
- [x] Kontextfreie Grammatiken
	- [x] Chomsky Hierarchie
	- [x] Chomsky Normalform
	- [x] CYK Algorithmus
	- [x] Ableitungsbäume

Cheat Sheet
DIN-A4 Handschriftlich Beidseitig

## NP-Vollständigkeit
### Beweis
1. Zeige dass das Problem in $NP$ liegt
	- Eine Lösung kann in polynomieller Zeit geraten und verifiziert werden
	- Orakel TM & DTM
2. Reduziere ein passendes bekannt $NP$-vollständiges Problem auf das jetzige Problem
	- Konstruiere eine Instanz des bekannten Problems aus dem jetzigen Problem
	- z.B. $COLOR \propto FREQUENCY ALLOCATION$: Knoten sind Transmitter, Kanten interfierende Transmitter, Mögliche Färbungen sind alle mögliche Frequenzen, Färbung ist gewählte Frequenz
	- Beachte und definiere dabei die nötigen Eingaben des Problems!
3. Zeige dass eine Instanz des bekannten Problem genau dann lösbar ist, wenn die transformierte Instanz das jetzige Problem löst
	- Zeige Hin- und Rückrichtung!
4. Mit $NP$-Vollständigkeit des bekannten Problems auf die Behauptung Folgern