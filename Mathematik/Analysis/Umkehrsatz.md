---
aliases: []
---

# Umkehrsatz
## Motivation
Wann lässt sich eine Funktion $f: D \subseteq \mathbb{R}^{n} \to \mathbb{R}^{n}$ in der Nähe eine Punktes $u \in D$ umkehren?

Für eine Teilmenge $M \subseteq D$ schreiben wir
$$
F|_{M}: M \to \mathbb{R}^{n} {mit} f|_{M}(x) := f(x)
$$
(Einschränkung von $f$ auf $M$).

## Definition
Ist $D \subseteq \mathbb{R}^{n}$ [[offene Mengen|offen]] und $f \in C^{1}(D, \mathbb{R}^{n})$ sowie $u \in D$ mit $det(f'(u) \neq 0)$ dann gibt es ein $\delta > 0$, sodass $f|_{U_{\delta}(u)}: U_{\delta}(u) \to \mathbb{R}^n$ [[injektiv]] ist und $f|_{U_{\delta}(u)}^{-1}: f(U_{\delta}(u)) \to U_{\delta}(u)$ ist [[Stetigkeit|stetig]] [[Partielle Differenzierbarkeit|partiell differenzierbar]] mit
$$
(f|_{U_{\delta}(u)}^{-1})'(y) = f'(f|_{U_{\delta}(u)}^{-1}(y))^{-1}
$$
Um die Ableitung des Punktes $y$ in der Zielmenge von $f$ zu erhalten, genügt es das Urbild von $y$ in die Ableitung von $f$ einzusetzen. Aus der Reihenfolge `Invertieren - Ableiten` wird `Ableiten - Invertieren`.
Merke: $(f^{-1})' = f'(f^{-1})^{-1}$

### Bemerkung
Der Satz hängt stark mit [[implizit definierte Funktionen]] zusammen.


---
**Tags**: #todo 