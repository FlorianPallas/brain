---
aliases: [DGL, Differentialgleichung, Anfangswertproblem, AWP, separabel, separable DGL, getrennte DGL, DGL mit getrennten Variablen]
---

# Differentialgleichungen #card
## Definition
Eine [[Gleichung]] für eine [[Funktion]] $y: I \subseteq \mathbb{R} \to \mathbb{R} x \mapsto y(x)$, in der neben $x$ und $y(x)$ (nur genau $x$, auch nicht $2x$) auch [[Ableitung|Ableitungen]] $y^{(k)}(x)$ (auch nur $x$) vorkommen, heißt **Differentialgleichung ($k$-ter Ordnung) für $y$** oder auch **DGL**.

## Anfangswertproblem
Ein **Anfangswertproblem** oder auch **AWP** für $y$ ist eine DGL für $y$ zusammen mit einer Bedingung der Form $y(x_{0}) = y_{0}$.

## Eigenschaften
Eine DGL für $y$ heißt **separabel** oder **DGL mit getrennten Variablen**, wenn sie in der Form $y'(x) = F(x) \cdot G(y(x))$ mit [[Stetigkeit|stetigen]] Funktionen $f$ und $g$ geschrieben werden kann. Wobei $F(x)$ nur von $x$, $G(y(x))$ nur von $y$ Abhängig sind.

Eine DGL für $y$ heißt **lineare DGL erster Ordnung**, wenn sie in der Form $y'(x) = \alpha(x) \cdot y(x) + s(x)$ mit [[Stetigkeit|stetigen]] Funktionen $\alpha , s: I \subseteq \mathbb{R}^{n} \to \mathbb{R}$ geschrieben werden kann. Sie heißt zudem **homogen** falls $s = 0$, ansonsten **inhomogen**.

## Satz
Jedes lineare AWP hat eine eindeutige Lösung auf einem eindeutig gegebenen maximalen Intervall.

## Verfahren
### Separable DGL (Trennung der Veränderlichen)
Eine separable DGL der Form $y'(x) = F(x) \cdot G(y(x))$ mit $G(t) \neq 0$ für alle $t$ lässt sich durch Auflösen von
$$
\int \frac{1}{G(y)} dy = [\int \frac{1}{G(t)} dt]_{t=y(x)} = \int F(x) dx + c
$$
nach $y(x)$, wobei $c$ ein frei wählbarer Parameter ist. Bei den Integralen selbst ist keine Integrationskonstante notwendig. Die eckige Klammer stellt eine Re-substitution der Stammfunktion dar.

### homogene lineare DGL
Jede homogene lineare DGL erster Ordnung ist separabel: $y'(x) = \alpha(x) y(x)$ mit $F(x) = \alpha(x)$ und $G(t) = t$. Die Lösung ist $y(x) = c \cdot e^{\beta(x)}$ mit $c \in \mathbb{R}$ beliebig. Wobei $\beta(x) := \int \alpha(x) dx$ eine beliebige Stammfunktion von $\alpha$ ist.
(Herleitung: Verfahren für separable DGL)

### inhomogene lineare DGL
Jede inhomogene DGL erster Ordnung der Form $y'(x) = \alpha(x) y(x) + s(x)$ kann wie folgt gelöst werden:
1. Bestimme die allgemeine Lösung $y_{H}(x) = c \cdot e^{\beta(x)}$ der zugehörigen homogenen DGL $y'(x) = \alpha(x) y(x)$ ohne $s(x)$.
2. Bestimme eine spezielle Lösung $y_{S}$ der gesamten DGL mit dem Ansatz $y_{S}(x) = d(x) \cdot e^{\beta(x)}$ (Variation der Konstanten, $c$ wird zu $d(x)$) durch Einsetzen von $y_{S}$ in die DGL.
3. Allgemeine Lösung der DGL ist $y(x) = y_{S}(x) + y_{H}(x)$. Wobei $y_{H}(x)$ eine beliebige Lösung aus 1. ist.

---
**Tags**: #todo 