---
aliases: []
---

# Decorator #card
## Zweck
- Fügt dynamisch neue Funktionalität zu einem Objekt hinzu
- Kann alternativ zu Vererbung verwendet werden
## Struktur
![[Pasted image 20220616173644.png]]
Der Umweg über das gemeinsame Interface ist aus zweierlei Gründen notwendig
1. Es ermöglicht alle Variationen mit einem Interface anzusprechen
2. Es ermöglicht eine unendliche Verschachtelung von Konkreten Decorators ineinander, da der Decorator eine Instanzvariable mit Referenz auf eine Komponente speichert, die ebenfalls eine Konkreter Decorator sein kann. Idealerweise nimmt der Konstruktor der Konkreten Decorators eine Komponente entgegen.
## Beispiel
![[Pasted image 20220616174447.png]]
![[Pasted image 20220616174549.png]]
![[Pasted image 20220616174643.png]]
^c-BezFhvh2pt
---
**Tags**: 