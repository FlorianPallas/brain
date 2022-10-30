---
aliases: [linear, linearen DGL]
---

# lineare DGL #card
## Definition
Eine [[Differentialgleichung|DGL]] für $y$ heißt **lineare DGL erster Ordnung**, wenn sie in der Form $y'(x) = \alpha(x) \cdot y(x) + s(x)$ mit [[Stetigkeit|stetigen]] Funktionen $\alpha , s: I \subseteq \mathbb{R}^{n} \to \mathbb{R}$ geschrieben werden kann. Sie heißt zudem **homogen** falls $s = 0$, ansonsten **inhomogen**.

## Satz
Jedes lineare AWP hat eine eindeutige Lösung auf einem eindeutig gegebenen maximalen Intervall.

## Verfahren
### homogene lineare DGL
Jede homogene lineare DGL erster Ordnung ist separabel: $y'(x) = \alpha(x) y(x)$ mit $F(x) = \alpha(x)$ und $G(t) = t$. Die Lösung ist $y(x) = c \cdot e^{\beta(x)}$ mit $c \in \mathbb{R}$ beliebig. Wobei $\beta(x) := \int \alpha(x) dx$ eine beliebige Stammfunktion von $\alpha$ ist.
(Herleitung: Verfahren für separable DGL)

### inhomogene lineare DGL
Jede inhomogene DGL erster Ordnung der Form $y'(x) = \alpha(x) y(x) + s(x)$ kann wie folgt gelöst werden:
1. Bestimme die allgemeine Lösung $y_{H}(x) = c \cdot e^{\beta(x)}$ der zugehörigen homogenen DGL $y'(x) = \alpha(x) y(x)$ ohne $s(x)$.
2. Bestimme eine spezielle Lösung $y_{S}$ der gesamten DGL mit dem Ansatz $y_{S}(x) = d(x) \cdot e^{\beta(x)}$ (Variation der Konstanten, $c$ wird zu $d(x)$) durch Einsetzen von $y_{S}$ in die DGL.
3. Allgemeine Lösung der DGL ist $y(x) = y_{S}(x) + y_{H}(x)$. Wobei $y_{H}(x)$ eine beliebige Lösung aus 1. ist.
^c-sG5BNqyz7d

---
**Tags**: #todo 