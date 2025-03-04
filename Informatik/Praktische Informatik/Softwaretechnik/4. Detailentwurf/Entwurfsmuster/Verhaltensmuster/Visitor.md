---
aliases: []
---

# Visitor #card
## Zweck
- Kapsle eine auf den Elementen einer Objektstruktur auszuführende Operation als ein Objekt.
- Das Visitor-Muster ermöglicht es, eine neue Operation zu definieren, ohne die Klassen der von ihr bearbeiteten Elemente zu verändern.
## Struktur
![[Pasted image 20220621183040.png]]
## Anwendbarkeit
- Wenn eine Objektstruktur viele Klassen von Objekten mit unterschiedlichen Schnittstellen enthält und Operationen auf diesen Objekten ausgeführt werden sollen, die von ihren konkreten Klassen abhängen.
- Wenn mehrere unterschiedliche und nicht miteinander verwandte Operationen auf den Objekten einer Objektstruktur ausgeführt werden müssen und diese Klassen nicht mit diesen Operation „verschmutzt” werden sollen.
- Wenn sich die Klassen, die eine Objektstruktur definieren, praktisch nie ändern, aber häufig neue Operationen für die Struktur definiert werden.
## Beispiel 
![[Pasted image 20220621183302.png]]
![[Pasted image 20220621183319.png]]
![[Pasted image 20220621183353.png]]
^c-f5SszNxgFl
---
**Tags**: 