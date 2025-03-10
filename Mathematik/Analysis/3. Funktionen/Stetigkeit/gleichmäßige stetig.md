## Definition

![[CleanShot 2023-01-13 at 10.01.22@2x.png]]

## $\epsilon, \delta$ - Definition

![[CleanShot 2023-01-13 at 10.02.02@2x.png]]

## Intuition

Die gleichmäßige Stetigkeit hängt nur von dem Abstand der beiden Stellen ab, während die allgemeine Stetigkeit von dem Abstand und der zu untersuchenden Stelle abhängt.
Folglich kann man sich intuitiv vorstellen, dass die gleichmäßige Stetigkeit kaputt geht, wenn die Funktion zu stark steigt/fällt.
![[CleanShot 2023-01-13 at 11.24.50@2x.png]]

## Zusammenhang mit Stetigkeit

Eine gleichmäßig stetige Funktion ist stets auch stetig. Die Umkehrung gilt nur wenn der Satz von Heine erfüllt ist. Also im Allgemeinen nicht. #relation

Bei der allgemeinen Stetigkeit hängt bei der $\epsilon, \delta$-Definition das $\delta$ von $\epsilon$ und $x_0$ ab. Bei der gleichmäßigen Stetigkeit hängt das $\delta$ nur vom $\epsilon$ ab.

## Satz von Heine

![[CleanShot 2023-01-13 at 10.04.21@2x.png]]

## Beweis

Der Beweis fällt i.d.R. mit $\epsilon, \delta$-Definition leichter
Laut Definition gilt $|x-y| < \delta$. Man bringt nun $|f(x) - f(y)|$ auf eine Form in der $|x-y|$ vorkommt und somit durch $\delta$ nach oben abgeschätzt werden kann. Man wähle nun $\delta$ abhängig von $\epsilon$ (z.B. $\delta := \epsilon^{2}$), sodass $|f(x) - f(y)| < \epsilon$ gilt.

## Widerspruch

Wähle zwei Folgen aus $D$, sodass $|x_{n}-y_{n}| \to 0 \; (n \to \infty)$ gilt, aber $|f(x_{n}) - f(y_{n})| \not\to 0 \; (n \to \infty)$.
