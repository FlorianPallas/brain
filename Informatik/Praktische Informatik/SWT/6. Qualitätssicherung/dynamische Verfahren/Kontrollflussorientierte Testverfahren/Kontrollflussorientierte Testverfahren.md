---
aliases: []
---

# Kontrollflussorientierte Testverfahren #card
## Idee
1. [[Strukturerhaltende Transformation]] des Programms in eine [[Zwischensprache]]. 
2. Aufteilen des Programms in [[Grundblock|Grundblöcke]]
3. [[Kontrollflussgraph]] aufstellen
4. [[Kontrollflussgraph]] analysieren
## Verfahren
### Anweisungsüberdeckung
Die Teststrategie Anweisungsüberdeckung $\mathrm{C}_{\text {Anweisung }}$ (engl. statement coverage) verlangt die Ausführung aller Grundblöcke des Programms P.
- C steht für Coverage
- Metrik, auch $\mathrm{C}_{0}$ genannt
$$
\mathrm{C}_{\text {Anweisung }}=\frac{\text { Anzahl durchlaufener Anweisungen }}{\text { Anzahl aller Anweisungen }}
$$
- Nicht ausreichendes Testkriterium
- Nicht ausführbare Programmteile können gefunden werden.
- Fehlende Programmteile werden nicht entdeckt.
- Auch Anweisungserfassung genannt (ein Testvollständigkeitskriterium)
### Zweigüberdeckung
Die Zweigüberdeckung $C_{Z w e i g}$ (engl. branch coverage) verlangt das Traversieren aller Zweige im KFG.
- Metrik, auch $\mathrm{C}_{1}$ genannt
$$
\mathrm{C}_{\text {Zweig }}=\frac{\text { Anzahl traversierter Zweige }}{\text { Anzahl aller Zweige }}
$$
- Zweige, die nicht ausgeführt werden, können entdeckt werden
- Weder Kombination von Zweigen (Pfade) noch komplexe Bedingungen berücksichtigt
- Schleifen werden nicht ausreichend getestet
- Fehlende Zweige nicht testbar, nicht entdeckt.
Auch Zweigerfassung genannt.
### Boundary-Interior Test
"Boundary-Interior Test" (Grenz- und Innen-Test) testet Schleifen ausführlicher als Zweigüberdeckung (und subsummiert sie)
- Konstruiere einen Satz Testfälle, die den Schleifenrumpf einmal queren,
- Einen zweiten Satz, die den Schleifenrumpf mindestens zweimal queren
- Verzweigungen innerhalb des Schleifenrumpfes mit Zweigüberdeckung berücksichtigen, d.h. beim einmaligen Queren alle Zweige abdecken, beim mehrmaligen Queren in der letzten Querung alle Zweige abdecken (andere egal).
- Eine Schleife mit einer bedingten Anweisung braucht also Testfälle für $2 \cdot 2$ Pfade.
### Pfadüberdeckung
Die Pfadüberdeckung (engl. path coverage) fordert die Ausführung aller unterschiedlichen, vollständigen Pfade im Programm.
- Pfadanzahl wächst bei Schleifen dramatisch an.
- Manche Pfade können nicht ausführbar sein, durch sich gegenseitig ausschließende Bedingungen
- Mächtigste KFO Teststrategie
- Nicht praktikabel, da es oft schon für kleine Programme mit Schleifen nicht zu realisieren ist.
### Vergleich der drei
![[Pasted image 20220705144032.png]]
### Bedingungsüberdeckung
- Zweigüberdeckung nicht ausreichend bei zusammengesetzten oder hierarchischen Bedingungen
- Drei Ausprägungen der Bedingungsüberdeckungen (BÜ) (engl. condition coverage):
	- Einfache BÜ: Jede atomare Bedingung einmal wahr und falsch sein
	- Mehrfache BÜ: Jede Kombination von Bedingungen einmal wahr und falsch (exponential viele)
	- Minimal-mehrfache BÜ: Jedes Atom der Bedingung, jeder atomare Teilausdruck und der Gesamtausdruck müssen mindestens einmal TRUE und einmal FALSE geworden sein (linear viele)
### Zusammenhang
![[Pasted image 20220630152055.png]]
^c-Dy9f4rxBzl
---
**Tags**: 