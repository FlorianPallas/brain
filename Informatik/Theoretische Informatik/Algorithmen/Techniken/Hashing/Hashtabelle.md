---
aliases: []
---

# Hashtabelle #card
## Motivation
Mit Hashing kann eine Map (key-value pairs) mit wenig vergleichsweise wenig Speicherverbrauch aufgestellt werden, die Einfügen, Bearbeiten und Löschen durchschnittlich in $\Theta(1)$ unterstützt.
## Funktionsweise
![[Pasted image 20220518142120.png]]
Die Wahrscheinlichkeit, dass der Hashwert zweier Keys gleich ist, ist erstaunlich hoch. Siehe [[Geburtstagsparadoxon]]. Folglich wird Chaining angewandt um mit den Kollisionen umzugehen.
![[Pasted image 20220518144223.png]]
## Wahl der Größe der Tabelle
Idee: siehe [[Unbeschränktes Array|unbeschränktes Array]]
![[Pasted image 20220518145659.png]]
Hinweis: $m$ gibt die Größe der Hashtabelle an und $n$ die Menge an Elementen die hinzugefügt werden.
## Laufzeit mit der [[Simple Uniform Hashing Assumption]]
![[Pasted image 20220518145139.png]]
![[Pasted image 20220518145211.png]]
Folglich gilt:
Gegeben die [[Simple Uniform Hashing Assumption]], dann kann eine Hashtabelle die Operationen Einfügen, Suchen und Löschen in erwartet konstanter Zeit ausführen, wenn die Anzahl Buckets $m$ linear ist in der Anzahl (key, value)-Paare $n$.
## Generelle Laufzeit
Mit [[Universelles Hashing|Universellem Hashing]] kann die obige Laufzeit garantiert werden. Dabei wird eine Hashfunktion gewählt und diese verwendet, bis die Tabelle ihre Kapazität vergrößert.
^c-4UH8dMs6nA
---
**Tags**: 