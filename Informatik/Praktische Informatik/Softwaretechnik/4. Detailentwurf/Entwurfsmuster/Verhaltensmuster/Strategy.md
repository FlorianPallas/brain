---
aliases: []
---

# Strategy #card
## Zweck
Definiere eine Familie von Algorithmen, kapsele sie und mache sie austauschbar. Das Strategiemuster ermöglicht es, den Algorithmus unabhängig von nutzenden Clients zu variieren.
## Motivation
Manchmal müssen Algorithmen, abhängig von der notwendigen Performanz, der Menge oder des Typs der Daten, variiert werden.
## Struktur
![[Pasted image 20220621180445.png]]
## Anwendbarkeit
- Wenn sich viele verwandte Klassen nur in ihrem Verhalten unterscheiden. Strategieobjekte bieten die Möglichkeit, eine Klasse mit einer von mehreren möglichen Verhaltensweisen zu konfigurieren.
- Wenn unterschiedliche Varianten eines Algorithmus benötigt werden.
- Wenn ein Algorithmus Datenstrukturen verwendet, die Clients nicht bekannt sein sollen.
- Wenn eine Klasse unterschiedliche Verhaltensweisen definiert und diese als mehrfache Fallunterscheidungen in ihren Operationen erscheinen. Mit Strategie kann man diese Fallunterscheidungen vermeiden („switch-less programming").
## Beispiele
![[Pasted image 20220621180508.png]]
![[Pasted image 20220621180524.png]]

^c-Nb2PNNmyVC
---
**Tags**: 