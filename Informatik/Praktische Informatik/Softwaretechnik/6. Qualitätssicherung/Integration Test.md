---
aliases: []
---

# Integration Test #card
## Definition
- Voraussetzung: Jede involvierte Komponente wurde bereits für sich überprüft 
- Schrittweise Integration: Integriere eine weitere Komponente in die bereits im Zusammenspiel geprüfte Komponentenmenge und prüfe erneut bis das System komplett integriert ist.
	- getestet wird das Zusammenspiel der Komponenten
	- Stummel und Attrappen werden mit den Implementierungen ersetzt
## Strategiegruppen
![[Pasted image 20220706160642.png]]
### Unmittelbar
Vorteile:
- keine Testtreiber und keine Platzhalter benötigt 
Nachteile:
- Alle Systemkomponenten müssen fertig und überprüft sein
- Defekt schwer zu lokalisieren
- Testüberdeckung schwierig sicherzustellen
Fazit:
- Für größere Systeme nicht geeignet
### Inkrementell
Vorteile:
- Testen fertiger Komponenten und Fertigstellung unfertiger Komponenten parallelisierbar
- Testfälle leichter konstruierbar
- Testüberdeckung prüfbar
Nachteile:
- Evtl. viele [[Testhelfer]] notwendig
### Vorgehensorientiert
Integrationsreihenfolge leitet sich aus der Systemarchitektur ab
### Testzielorientiert
- Testfälle werden ausgehend von den Testzielen (z.B. „so schnell wie möglich fertige Komponenten integrieren") erstellt
- Jeweils benötigte Komponenten werden „zusammenmontiert"
## Konkrete Strategien
### Big bang
- Alle Komponenten werden gleichzeitig integriert
- Integrationstest kaum systematisierbar
- Konstruktion von Testfällen schwierig
- Defektsuche schwierig
„Nichts geht bis alles geht."
### Funktionsorientiert
- Spezifikation funktionaler Testfälle (funktionale Anforderungen)
- Schrittweise Integration und Test der Komponenten, die durch die Testfälle betroffen sind
### nach Verfügbarkeit
- Integration von Komponenten sofort nach Abschluss inrer Überprüfung
- Schrittweise Integration und Test
- Reihenfolge durch Implementierungsfertigstellungsreihenfolge festgelegt ( $\rightarrow$ schlechte Planbarkeit)
### Top-Down
- Integration von höchster logischer Ebene her (z.B. Benutzeroberfläche)
- Frühe Verfügbarkeit eines Simulationsmodells, anhand dessen Defekte in der Produktdefinition identifizierbar sind
- Späte Prüfbarkeit des Zusammenspiels mit Hardware und Basissoftware
- Integrierte Systemkomponenten setzen Dienste niedrigerer logischer Ebenen voraus $\rightarrow$ z.T. aufwendige, schwierig zu erstellende Testhelfer
### Bottom-Up
- Integration von niedrigster logischer Ebene her (Komponenten, die selbst nicht von anderen Komponenten abhängen)
- Testtreiber erforderlich
- leichteres Herstellen von Testbedingungen
- leichtere Interpretation von Testergebnissen
$\rightarrow$ (die Vorteile von top-down sind hier natürlich entsprechend die Nachteile und umgekehrt)
### Outside-In
- Versuch, die Nachteile von top-down und bottom-up zu mindern
- Beginnt gleichzeitig auf höchster und niedrigster logischer Ebene mit der Integration
- Schrittweise Integration in beide Richtungen aufeinander zu
### Inside-Out
- Beginnt auf mittlerer Ebene mit der Integration
- Schrittweise Integration in beide Richtungen auseinander
- Vereinigt eher die Nachteile von topdown und bottom-up
$\rightarrow$ höchstens sinnvoll in Verbindung mit hardest-first!
### Hardest-First
- Zuerst werden die kritischen (also kompliziert zu testenden oder potentiell fehlerhaften) Komponenten integriert
- Bei jedem Integrationsschritt werden die kritischen Komponenten indirekt mitgeprüft $\rightarrow$ letztlich die am Besten getesteten Komponenten
^c-jlavMrHeI7
---
**Tags**: