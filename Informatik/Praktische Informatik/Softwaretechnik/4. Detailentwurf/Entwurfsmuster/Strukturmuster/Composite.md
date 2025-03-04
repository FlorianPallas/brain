---
aliases: []
---

# Composite #card
## Zweck
Füge Objekte zu Baumstrukturen zusammen, um Bestands-Hierarchien zu repräsentieren. Das Muster ermöglicht es Clients, sowohl einzelne Objekte als auch Aggregate einheitlich zu behandeln.
## Motivation
- Bestands-Hierarchien treten überall dort auf, wo komplexe Objekte modelliert werden, wie beispielsweise Dateisysteme, graphische Anwendungen, Textverarbeitung, CAD, CIM,...
- Bei diesen Anwendungen werden einfache Objekte zu Gruppen zusammengefasst, welche wiederum zu größeren Gruppen zusammengefügt werden können.
- Häufig soll dabei die Behandlung von Objekten und Aggregaten durch das Programm einheitlich sein. Das Composite isoliert die gemeinsamen Eigenschaften von Objekt und Aggregat und bildet daraus eine Oberklasse.
## Struktur
![[Pasted image 20220616175430.png]]
## Beispiele
![[Pasted image 20220616175535.png]]
![[Pasted image 20220616175517.png]]
^c-W3SYWLiGyK
---
**Tags**: 