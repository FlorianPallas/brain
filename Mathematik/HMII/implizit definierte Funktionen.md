---
aliases: []
---

# implizit definierte Funktionen
## Motivation
Wir möchten Gleichungen oder Gleichungssysteme nach einer oder mehreren Variablen auflösen.

Will man $x-y^{2}=0$ auflösen, so folgt:
Auflösen nach $x$ ist einfach: $x = y^{2}$.
Die Gleichung nach $y$ aufgelöst ist allerdings nicht eindeutig: $y = \sqrt{x}$ oder $y = -\sqrt{x}$.

## Definition
Für jeden Punkt $(x_{0},y_{0}) \in \mathbb{R}^{2} \setminus \{0\}$ gibt es ein [[offene Mengen|offenes]] Rechteck $(x_0-\delta,x_0+\delta) \times (y_{0}-\gamma, y_{0}+\gamma) \subseteq \mathbb{R}^{2}$ auf dem die Gleichung eindeutig nach der Variable (hier $y$) aufgelöst werden kann.

Für jedes solche Rechteck gibt es eine eindeutige Funktion
$$
g: (x_{0}-\delta,x_{0}+\delta) \to (y_{0}-\gamma, y_{0}+\gamma)
$$
mit der Eigenschaft, dass für alle $x$ im Definitionsbereich von $g$ die gegebene Gleichung erfüllt ist (hier $x-g(x)^{2}=0$).

Man schreibt: $g$ wird **implizit** durch die Gleichung bei $(x_{0}, y_{0})$ **definiert**.


lokal implizit - gilt nur für Rechtecke, es gibt Rechtecke die nicht funktionieren
global implizit - gilt allgemein, es gibt beliebige Rechtecke




Das funktioniert auch für Gleichungen $F(x,y)=0$. Das heißt um nach $p$ Variablen $y_{1}, \cdots, y_{p}$ aufzulösen brauchen wir auch $p$ Gleichungen.

## Satz
Ist $f \in C^{1}(D, \mathbb{R}^p)$ mit $D \subseteq \mathbb{R}^{n+p} = \mathbb{R}^{n} \times \mathbb{R}^{p}$ mit $F(x_{0},y_{0})=0$ und $det (\frac{\partial F}{\partial y}(x_{0},y_{0})) \neq 0$, dann gibt es ein $\delta > 0$ und ein $\eta > 0$ und eine eindeutige Funktion $g: U_{\delta}(x_{0}) \to U_{\eta}(y_{0})$ mit $F(x,g(x))=0$ für alle $x \in U_{\delta}(x_{0})$.  Zudem ist $g$ [[Stetigkeit|stetig]] [[Partielle Differenzierbarkeit|pdb.]] mit
$$
g'(x) = -(\frac{\partial F}{\partial y}(x,g(x)))^{-1} \cdot \frac{\partial F}{\partial x}(x,g(x)) \subseteq \mathbb{R}^{p \times n}
$$

## Beispiele
![[Pasted image 20220615085914.png|400]]
![[Pasted image 20220615085941.png|400]]
![[Pasted image 20220615090006.png|400]]
![[Pasted image 20220615090022.png|400]]
![[Pasted image 20220615090219.png|400]]

---
**Tags**: #todo 