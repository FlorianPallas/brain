---
aliases: []
---

# Binäre Suche #card
## Theorem
Sei $M$ eine geordnete Menge $($z.B. $\mathbb{Z})$. Sei $A$ ein sortiertes Array der Länge $n$ mit Werten aus $M$ und sei $x \in M$. Die binäre Suche findet den Index $i$ mit $A[i-1]<x \leq A[i]$ in $\Theta(\log n)$ Zeit (Konvention: $A[-1]=-\infty, A[n]=\infty$ ).
## Folgerungen
- für $a, b \in M$ können wir in $\Theta(\log n)$ herausfinden, wie viele Elemente $A$ aus $[a, b]$ enthält.
- $A$ enthält $k$ Elemente aus $[a, b] \rightarrow$ wir können sie in $\Theta(\log n+k)$ aufzählen
## Implementierung


^c-zQIynvvOaO
---
**Tags**: #todo 