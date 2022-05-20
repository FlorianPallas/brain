---
aliases: []
---

# Würfelkalkül #card
## Definition
Ein [[Produktterm]] $K$ lässt sich im so genannten Würfelkalkül beschreiben. Ein Würfel
$$
C:=\left(c_{1}, \ldots, c_{n}\right) \in\{0,1,-\}^{n}
$$
wird durch den [[Produktterm]] $K$ wie folgt bestimmt:
$$
c_{i}:= \begin{cases}0, & \text { falls das Literal } \bar{x}_{i} \text { in } K \text { vorkommt } \\ 1, & \text { falls das Literal } x_{i} \text { in } K \text { vorkommt } \\ -, & \text { falls die Variable } x_{i} \text { in } K \text { nicht vorkommt (sog. ,don't care") }\end{cases}
$$
## Beispiel
- Es seien die Variablen $x_{1}, \ldots, x_{6}$ gegeben. Dem Produktterm $K=x_{2} \wedge \bar{x}_{3} \wedge \bar{x}_{5} \wedge x_{6}$ ist der Würfel $C=(-, 1,0,-, 0,1)$ zugeordnet.
## Veranschaulichung
- Ein $n$-Tupel, das an $m \leq n$ Stellen ein $-$ besitzt, ist ein $m$-dimensionaler Würfel.
- Ein $n$-Tupel $\left(c_{1}, \ldots, c_{n}\right)$, das an keiner Stelle ein don't care $-$ besitzt, beschreibt einen 0-dimensionalen Würfel, also einen Punkt.
- Der Begriff Würfel lässt sich für $n=3$ besonders leicht veranschaulichen. Der gesamte Kubus aus Abbildung $3.2$ wird durch den Würfel $(-,-,-)$ beschrieben, und jeder der acht möglichen Minterme von $\left(x_{1}, x_{2}, x_{3}\right)$ repräsentiert eine Ecke eines Würfels.
	![[Pasted image 20220520092540.png]]
## Würfelmengen
- Da jeder Würfel einem Produktterm entspricht, repräsentiert eine Würfelmenge $\boldsymbol{C}:=\left(C_{1}, \ldots, C_{m}\right)$ eine boolesche Funktion als Disjunktion dieser Produktterme. Folglich kann jede [[Disjunktive Normalform]] als Würfelmenge ausdrücken
## Überdeckung
- Ein Würfel $A:=\left(a_{1}, \ldots, a_{n}\right)$ überdeckt den Würfel $B:=$ $\left(b_{1}, \ldots, b_{n}\right), B \subseteq A$ wenn in jeder Komponente $\left(a_{i}=b_{i}\right)$ oder $a_{i}=-$ gilt. Also Würfel $A$ enthält alle Variablenbelegungen, die in Würfel $B$ enthalten sind.
- Ein Würfel $A$ wird durch eine Würfelmenge $\boldsymbol{C}:=\left(C_{1}, \ldots, C_{m}\right)$ überdeckt, $A \subseteq \boldsymbol{C}$, wenn alle [[Minterm|Minterme]] von $A$ durch mindestens einen Würfel in $\boldsymbol{C}$ überdeckt werden.
^c-fFK1JLhNIG
---
**Tags**: 