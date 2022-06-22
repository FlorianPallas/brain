---
aliases: [Integral, integrierbar, ib.]
---

# Integrierbarkeit
## Definition
$f$ heißt **integrierbar** über $I$, wenn $s_{f} = S_{f}$ ist. Dann ist das **Integral** $\int\limits_{I} f(x_{1},...,x_{n}) d(x_{1},\cdots ,x_{n}) := s_{f}$

## Fakt
Aus [[Stetigkeit]] folgt Integrierbarkeit
$f$ stetig $\Rightarrow$ $f$ integrierbar
Es gibt allerdings auch Funktionen welche zwar nicht stetig aber trotzdem integrierbar sind.

### über Rechtecke
Gegeben eine Funktion $f: I \subseteq \mathbb{R}^{n}\to \mathbb{R}$ mit $I:=[a_{1},b_{1}] \times [a_{2},b_{2}] \times \cdots \times [a_{n},b_{n}]$. Wie soll man $\int\limits_{I} f(x_{1},...,x_{n}) d(x_{1},\cdots ,x_{n})$ definieren?
#todo 
Das Integral soll das jeweilige Volumen messen.

Idee: Wähle Zerlegungen $Z_{1}:=\{u_{1}, \cdots, u_{k}\}$ von $[a_{1};b_{1}]$ mit $a_{1}=u_{1} < u_{2} < \cdots < u_{k}=b_{1}$
#todo 

$Z:= Z_{1} \times Z_{2}$ heißt Zerlegung von $[a_{1};b_{2}] \times [a_{2};b_{2}]$ 
#todo

## Satz von Fubini
Sei $f: I_{1} \times I_{2} \to \mathbb{R}$ integrierbar.
Wenn für jedes feste $y \in I_{2}$ das Integral $\int\limits_{I_{1}} f(x,y)dx$ existiert, dann ist $$\int\limits_{I_{1}\times I_{2}} f(x,y) \; d(x,y) = \int\limits_{I_{2}} \int\limits_{I_{1}}f(x,y)\;dx\;dy = \int\limits_{I_{1}} \int\limits_{I_{2}}f(x,y)\;dy\;dx$$Die Reihenfolge der iterierten Integration ist nicht relevant.

### Bemerkung
Wenn $f$ nicht integrierbar sind die Ausdrücke eventuell nicht gleich.


---
**Tags**: #todo 