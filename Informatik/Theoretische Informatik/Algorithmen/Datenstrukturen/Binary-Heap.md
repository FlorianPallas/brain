---
aliases: [Min-Heap]
---

# Binary-Heap #card
## Zweck
Wird verwendet um eine [[Priority-Queue]] zu realisieren. Im Folgenden wird der Aufbau für ein Min-Heap beschrieben.
## Eigenschaften
![[Pasted image 20220621095441.png]]
![[Pasted image 20220621095531.png]]
## Realisierung als Array
![[Pasted image 20220621095140.png]]
## Pseudocode
![[Pasted image 20220621095227.png]]
![[Pasted image 20220621095250.png]]
## Initialer Aufbau
![[Pasted image 20220621095756.png]]
![[Pasted image 20220621100011.png]]
## decPrio
Diese Funktionalität unterstützen nur wenige Implementierungen, da wenn die Priorität eines Elements geändert wird das Neuordnen $O(\log n)$ benötigt, was genauso aufwendig ist, wie wenn das alte Element gelöscht wird und mit neuer Priorität hinzugefügt wird.
Für [[Dijkstra]] bietet es sich an decPrio mittels Lazy Evaluation umzusetzen.
![[Pasted image 20220621101739.png]]
## Anmerkungen 
- Prioritäten können Elemente einer beliebigen geordneten Menge sein; $z$.B. Strings, da das einzige, was wir mit den Prioritäten machen ist das Vergleichen
- Laufzeit: $\Theta(\log n)$ Vergleiche pro Operation
^c-dRFUKKZNQy
---
**Tags**: 