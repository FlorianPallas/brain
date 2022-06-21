---
aliases: []
---

# Null-Object #card
## Zweck
Stelle einen Stellvertreter zur Verfügung, der die gleiche Schnittstelle bietet, aber nichts tut. Das Null-Objekt kapselt die Implementierungs-Entscheidungen (wie genau es „nichts tut") und versteckt diese Details vor seinen Mitarbeitern.
## Motivation
Es wird verhindert, dass der Code mit Tests gegen Null-Werte verschmutzt wird.
## Struktur
![[Pasted image 20220621182001.png]]
## Anwendbarkeit
- Wenn ein Objekt Mitarbeiter benötigt und einer oder mehrere von innen nichts tun sollen.
- Wenn Clients sich nicht um den Unterschied zwischen einem echten Mitarbeiter und einem der nichts tut kümmern sollen.
- Wenn das „tue nichts"-Verhalten von verschiedenen Clients wiederverwendet werden soll.
^c-0QHLZAmvk0
---
**Tags**: 