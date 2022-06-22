---
aliases: []
---

# (2,3)-Tree #card
## Eigenschaften
![[Pasted image 20220620164557.png]]
![[Pasted image 20220620164449.png]]
## Operationen
Das Einfügen und das Löschen eines Eintrags benötigt $O(\log n),$ da das Problem bei beiden Operationen jeweils um eine Schicht nach Oben geschoben wird.
### Einfügen
![[Pasted image 20220620164417.png]]
### Löschen
![[Pasted image 20220620164311.png]]
## Implementierung
### Repräsentation
![[Pasted image 20220622141829.png]]
### Initialisierung
![[Pasted image 20220622141630.png]]
### Suche
![[Pasted image 20220622141745.png]]
### Einfügen
![[Pasted image 20220622142442.png]]
![[Pasted image 20220622143712.png]]
![[Pasted image 20220622143842.png]]
### Löschen
![[Pasted image 20220622151002.png]]
![[Pasted image 20220622151013.png]]
Hinweis: Das Löschen des Kinds $b$ von $a$ beinhaltet das Aktualisieren des Keys von $a.$
![[Pasted image 20220622152035.png]]
![[Pasted image 20220622152120.png]]
^c-2KxvFonrN8
---
**Tags**: 