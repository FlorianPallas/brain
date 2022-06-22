---
aliases: []
---

# Facade #card
## Zweck
Biete eine einheitliche Schnittstelle zu einer Menge von Schnittstellen eines Subsystems. Somit ist eine Facade quasi ein [[Adapter]] für viele Klassen.
Die Facade-Klasse definiert eine abstrakte Schnittstelle, welche die Benutzung des Subsystems vereinfacht.
## Anwendbarkeit
- Wenn eine einfache Schnittstelle zu einem komplexen Subsystem angeboten werden soll. Eine Fassade kann eine einfache voreingestellte Sicht auf das Subsystem bieten, die den meisten Clients genügt.
- Wenn es viele Abhängigkeiten zwischen den Clients und den Implementierungsklassen einer Abstraktion gibt. Die Einführung einer Facade entkoppelt die Subsysteme von Clients und anderen Subsystemen.
- Wenn Subsysteme in [[Layered Architecture|Schichten]] aufgeteilt werden sollen. Man verwendet eine Facade, um einen Eintrittspunkt zu jeder Subsystemschicht zu definieren.
## Beispiel
![[Pasted image 20220616172557.png]]
^c-fABSVVYqfT
---
**Tags**: 