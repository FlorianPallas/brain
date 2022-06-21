---
aliases: []
---

# Command #card
## Zweck
Kapsle einen Command als ein Objekt. Dies ermöglicht es, Clients mit verschiedenen Anfragen zu parametrisieren, Operationen in eine Warteschlange zu stellen, ein Logbuch zu führen und Operationen rückgängig zu machen.
## Struktur
![[Pasted image 20220621181325.png]]
## Anwendbarkeit
- Wenn Objekte mit einer auszuführenden Aktion parametrisiert werden sollen (wie bei den MenüEintrag-Objekten).
- Wenn Anfragen zu unterschiedlichen Zeiten spezifiziert, aufgereiht und ausgeführt werden sollen.
- Wenn ein Rückgängigmachen von Operation (Undo) unterstützt werden soll.
- Wenn das Mitprotokollieren von Änderungen unterstützt werden soll (um System nach Absturz wiederherzustellen).
- Wenn ein System mittels komplexer Operationen strukturiert werden soll, die aus primitiven Operationen aufgebaut werden (Makrobefehle).
## Beispiel
![[Pasted image 20220621181716.png]]
![[Pasted image 20220621181704.png]]
^c-HqyfpAYFQh
---
**Tags**: 