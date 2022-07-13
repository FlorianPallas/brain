---
aliases: [bernoulli DGL, bernoullischen DGL]
---

# bernoullische DGL #card
## Definition
Eine [[Differentialgleichung|DGL]] für $y$ heißt **Bernoullische DGL**, wenn sie mit [[Stetigkeit|stetigen]] Funktionen $a,b: I \subseteq \mathbb{R} \to \mathbb{R}$ geschrieben werden kann als
$$
y'(x) = a(x) \cdot y(x) + b(x) \cdot (y(x))^{\alpha}
$$
mit $\alpha \in \mathbb{R}$.

### Bemerkung
Für $a \in \{0,1\}$ ist die DGL [[lineare DGL|linear]]. Jede lineare DGL ist als Konsequenz auch eine bernoullische DGL.

## Verfahren
Eine bernoulli DGL mit $\alpha \notin \{0,1\}$ lässt sich mit dem Ansatz $z(x) := (y(x))^{1-\alpha}$ in eine [[lineare DGL]] für $z$ transformieren. Lösen dieser linearen DGL und Rücksubstituieren der Lösungen nach $y$ liefert die Lösungen der originalen DGL. Zudem kann $y(x) = 0$ eine weitere Lösung sein.
^c-dsLA8GmH45

---
**Tags**: #todo 