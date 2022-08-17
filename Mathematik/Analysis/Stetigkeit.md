---
aliases: [stetig, gleichmäßig stetig, lipschitz stetig]
---

# Stetigkeit
## Definition
Eine [[Funktion]] ist **in $x_{0}$ stetig**, genau dann wenn $\lim\limits_{x \to x_{0}} f(x) = f(x_{0})$ gilt. Ist die Funktion in allen $x \in D$ stetig, so ist sie **stetig auf $D$**.

Die Verkettung von stetigen Funktionen ist im Allgemeinen wieder stetig.

## Beweis & Widerspruch
Auf Teilintervalle wo die Funktion durch eine Verkettung von bekannt stetigen Funktionen definiert ist herrscht Stetigkeit. Nur die Nahtstellen zwischen diesen Intervallen müssen mittels der Definition geprüft werden. Stimmt der Grenzwert mit dem Funktionswert an der Stelle überein (der Grenzwert von beiden Seiten) ist die Funktion an dieser Stelle stetig, andernfalls ist sie das nicht.

---
# Gleichmäßige Stetigkeit
## Definition
Eine [[Funktion]] heißt auf $D$ **gleichmäßig stetig**, genau dann wenn zwei Folgen $(x_{n}), (y_{n})$ in $D$ sind für die wenn $|x_{n} - y_{n}| \to 0$ gilt, auch $|f(x_{n}) - f(y_{n})| \to 0$ gilt.

Eine gleichmäßig stetige Funktion ist stets auch stetig. Die Umkehrung gilt im Allgemeinen nicht. #relation

## Beweis
### Mittels Definition
Laut Definition gilt $|x-y| < \delta$. Man bringt nun $|f(x) - f(y)|$ auf eine Form in der $|x-y|$ vorkommt und somit durch $\delta$ nach oben abgeschätzt werden kann. Man wähle nun $\delta$ abhängig von $\epsilon$ (z.B. $\delta := \epsilon^{2}$), sodass $|f(x) - f(y)| < \epsilon$ gilt.
### Satz von Heine
Ist $D$ [[kompakt]] und $f$ stetig auf $D$, so ist $f$ auf $D$ gleichmäßig stetig.

## Widerspruch
Wähle zwei Folgen aus $D$, sodass $|x_{n}-y_{n}| \to 0 \; (n \to \infty)$ gilt, aber $|f(x_{n}) - f(y_{n})| \not\to 0 \; (n \to \infty)$.

---
# Lipschitz Stetigkeit
## Definition
Eine [[Funktion]] heißt **lipschitz stetig** auf $D$, genau dann wenn es ein $L \geq 0$ gibt (**Lipschitzkonstante**), sodass für alle Werte $x,y \in D$ gilt $|f(x) - f(y)| \leq L |x-y|$.

Eine lipschitz stetige Funktion ist stets auch gleichmäßig stetig. Die Umkehrung gilt im Allgemeinen nicht. #relation 

## Beweis
Man formt den Term $|f(x) - f(y)|$ auf die Form $L|x-y|$ um. Dabei kann nach oben abgeschätzt werden. Der Term welcher $L$ repräsentiert muss konstant sein. Dies kann man zum Beispiel durch Abschätzen der Variablen innerhalb des gegebenen Intervalls erreichen.

## Widerspruch
Nehme an die Funktion sei lipschitz stetig. Folglich muss $|f(x) - f(y)| \leq L |x-y|$ gelten. Da dies für alle $x,y \in D$ liegt können wir diese im Intervall frei wählen. Wählt man nun zwei Werte (z.B. $x=2y, y \in D$) und formt man die Ungleichung nach $L$ um, sodass der andere Term nicht nach oben beschränkt ist (und somit $L$ nicht konstant sein kann), so ist die Funktion nicht lipschitz stetig.

---
**Related:**
- https://en.wikipedia.org/wiki/Continuous_function
- https://en.wikipedia.org/wiki/Uniform_continuity
- https://en.wikipedia.org/wiki/Lipschitz_continuity
**Tags**: 