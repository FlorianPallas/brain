---
aliases: []
---

# Strukturerhaltende Transformation #card
## Definition
Wir sprechen von einer strukturerhaltenden Transformation einer Quellsprache (z.B. Java) in die [[Zwischensprache]], wenn
- (ausschließlich) die Befehle, die die Ausführungsreihenfolge beeinflussen, durch Befehlsfolgen der Zwischensprache ersetzt werden, wobei die Ausführungsreihenfolge der anderen Befehle bei gleicher Parametrisierung gleich bleibt mit der in der Quellsprache!
- alle anderen Befehle unverändert übernommen werden
- Transformationen, bei denen Anweisungsfolgen oder bedingte Sprünge repliziert werden, vermieden werden (kein Ausrollen von Schleifen, keine Optimierungen.)
## Beispiel
![[Pasted image 20220705141136.png]]
^c-yNcrRQGm5N
---
**Tags**: 