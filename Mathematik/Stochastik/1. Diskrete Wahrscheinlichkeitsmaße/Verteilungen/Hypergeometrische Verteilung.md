## Definition

Das Wahrscheinlichkeitsmaß $P =$ $\operatorname{Hyp}(N, M, n)$ auf $N _0$ gegeben durch die Zähldichte
$P ^X(\{m\})= P (X=m)=\frac{\left(\begin{array}{c}M \\ m\end{array}\right) \cdot\left(\begin{array}{c}N-M \\ n-m\end{array}\right)}{\left(\begin{array}{l}N \\ n\end{array}\right)}  \quad \forall m \in N _0$
mit $m \in \{\max(0, n+M-N), \dots , \min(n,M)\}$
heißt hypergeometrischen Verteilung.

## Zweck

Die hypergeometrische Verteilung $\operatorname{Hyp}(N, M, n)$ beschreibt die Anzahl der markierten Gegenstände beim $n$-maligem Ziehen ohne Zurücklegen aus $N$ Gegenständen, von denen $M$ markiert sind.

## Zusammenhang mit der [[Binomialverteilung]]

Zieht man mit Zurücklegen, so ist die Wahrscheinlichkeit, einen markierten Gegenstand zu ziehen, bei jeder Ziehung $M / N$. Die Anzahl der gezogenen markierten Gegenstände hat daher gerade die Binominalverteilung $\operatorname{Bin}(n, M / N)$.
Falls $n \ll N$, dann ist Ziehen mit oder ohne Zurücklegen fast identisch und daher
![[CleanShot 2022-11-16 at 18.20.28@2x.png]]
