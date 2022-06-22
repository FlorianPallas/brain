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


# Inhalte von Mengen
Der Inhalt eines Rechtecks $I = [a_{1},b_{1}] \times \cdots \times [a_{n}, b_{n}]$ ist $|I| = (b_{1}-a_{1}) \cdot \;\dots \; \cdot (b_{n}-a_{n})$.

## Motivation
Wie soll man nun den Inhalt einer beliebigen Menge $B \subseteq \mathbb{R}^{n}$ definieren?
Man wähle ein Rechteck $I \subseteq \mathbb{R}^{n}$ mit $B \subseteq I$ und setze $|B| := \int\limits_{I} c_{B}(x) dx$.
Dabei ist die charakteristische Funktion $c_{B(x})$ gleich $1$ wenn $x \in B$ und $0$ wenn $x \notin B$.

### Problem
$c_{B}(x)$ muss integrierbar sein und es gibt nur Rechtecke um beschränkte Mengen.

## Definition
Eine beschränkte Menge $B \subseteq \mathbb{R}^n$ heißt **messbar**, wenn es ein Rechteck $I$ mit $B \subseteq I$ gibt auf dem $c_{B}(x)$ integrierbar ist. Dann heißt
$$
|B| := \int\limits_{I} c_{B}(x) dx
$$
der **Inhalt von $B$**.
(In der Praxis sind alle Mengen messbar)

Ist $B \subseteq \mathbb{R}^{n}$ messbar und sind $f,g: B \to \mathbb{R}$ stetig mit $f \leq g$, dann ist auch $M_{f,g} := \{(x,y) \in \mathbb{R}^{n+1}: x \in B \;\text{und}\; f(x) \leq y \leq g(x) \}$ messbar.



---
**Tags**: #todo 