---
aliases: []
---

# Liste #card
Eine Liste ist eine [[Verzeigerte Datenstruktur]].
## Kluge Implementierung
![[Pasted image 20220504144847.png]]
- jeder Knoten der Datenstruktur speichert
	- eine der Zahlen der Folge value
	- Zeiger zum nächsten Knoten next
	- Zeiger zum vorherigen Knoten prev
- Einstiegspunkt: head 
## Operationen
- Einfügen oder Löschen vor oder nach einem Knoten hat eine [[Landau Notation|Laufzeit]] von $\Theta(1)$.
- Splice (Einfügen einer Teilliste nach einem gegebenen Knoten) hat eine [[Landau Notation|Laufzeit]] von $\Theta(1)$ 
## Vorteile
- Einfügen, Löschen und Verschieben
- Konkatinieren von zwei Listen
- Verschieben ganzer Bereiche
- Löschen ganzer Bereiche
## Nachteile
- Kein wahlfreier Zugriff (random access)
- Man muss die relevanten Knoten immer schon in der Hand haben
- In der Praxis: schlechtere konstante Faktoren (Speicheroverhead, Cache-Effekte)
## Auf Listen basierende Datenstrukturen
- [[Stack]]
- [[Queue]]
- [[Deque]]
^c-BeOl5ZysGo
---
**Tags**: