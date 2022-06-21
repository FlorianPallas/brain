---
aliases: []
---

# Template Method #card
## Zweck
- Definiere das Skelett eines Algorithmus in einer Operation und delegiere einzelne Schritte an Unterklassen.
- Die Verwendung einer Template Method ermöglicht es Unterklassen, bestimmte Schritte eines Algorithmus zu überschreiben, ohne seine Struktur zu verändern.
Somit ist die Template Method eine feingranularere Variante des [[Strategy]] Patterns.
## Struktur
![[Pasted image 20220621180926.png]]
## Anwendbarkeit
- Um die invarianten Teile eines Algorithmus genau einmal festzulegen und es dann Unterklassen zu überlassen, das variierende Verhalten zu implementieren.
- Wenn gemeinsames Verhalten aus Unterklassen herausfaktorisiert und in einer allgemeinen Klasse platziert werden soll, um die Verdopplung von Code zu vermeiden.
- Um die Erweiterungen durch Unterklassen zu kontrollieren. Eine Template Method lässt sich so definieren, dass sie „Einschubmethoden” (engl. hooks) an bestimmten Stellen aufruft und damit Erweiterungen nur an diesen Stellen zulässt.
- Häufig bei Framework-Architekturen genutzt.
## Beispiel
![[Pasted image 20220621180940.png]]
beziehungsweise noch modularer
![[Pasted image 20220621181154.png]]
^c-88MTooIhJ1
---
**Tags**: 