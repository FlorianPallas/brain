---
aliases: [separabel, getrennte DGL, DGL mit getrennten Variablen]
---

# separable DGL #card
## Definition
Eine DGL für $y$ heißt **separabel** oder **DGL mit getrennten Variablen**, wenn sie in der Form $y'(x) = F(x) \cdot G(y(x))$ mit [[Stetigkeit|stetigen]] Funktionen $f$ und $g$ geschrieben werden kann. Wobei $F(x)$ nur von $x$, $G(y(x))$ nur von $y$ Abhängig sind.

## Verfahren
### Separable DGL (Trennung der Veränderlichen)
Eine separable DGL der Form $y'(x) = F(x) \cdot G(y(x))$ mit $G(t) \neq 0$ für alle $t$ lässt sich durch Auflösen von
$$
\int \frac{1}{G(y)} dy = [\int \frac{1}{G(t)} dt]_{t=y(x)} = \int F(x) dx + c
$$
nach $y(x)$, wobei $c$ ein frei wählbarer Parameter ist. Bei den Integralen selbst ist keine Integrationskonstante notwendig. Die eckige Klammer stellt eine Re-substitution der Stammfunktion dar.
^c-Wy3XVDXvZm

---
**Tags**: #todo 