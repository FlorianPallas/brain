## Definition #card 
![[CleanShot 2023-01-13 at 11.25.40@2x.png]]
^c-vuRz2rSpwy

## Zusammenhang mit Stetigkeit #card 
Ist $f$ Lipschitz-stetig auf $D$, so ist $f$ gleichmäßig stetig auf $D$. Die Umkehrung gilt i.A. nicht #relation 
^c-lwUsiejUpz

## Intuition #card 
![[CleanShot 2023-01-13 at 11.30.46@2x.png]]
^c-KrkyMCxUAw

## Beispiele #card 
![[CleanShot 2023-01-13 at 11.28.04@2x.png]]
^c-PYdujdxTpd

## Beweis
Man formt den Term $|f(x) - f(y)|$ auf die Form $L|x-y|$ um. Dabei kann nach oben abgeschätzt werden. Der Term welcher $L$ repräsentiert muss konstant sein. Dies kann man zum Beispiel durch Abschätzen der Variablen innerhalb des gegebenen Intervalls erreichen.

Alternativ kann mit dem [[Mathematik/HMII/Mittelwertsatz]] argumentiert werden, da
$|f(x) - f(y)| = f'(\xi) |x-y| \leq \max_{\xi \in [x,y]} f'(\xi) |x-y|$ gilt. Berechnet man (mittels der zweiten Ableitung) das Maximum der Funktion mit $\xi \in [x,y]$, dann entspricht dies der Lipschitzkonstante $L$.

## Widerspruch
Nehme an die Funktion sei lipschitz stetig. Folglich muss $|f(x) - f(y)| \leq L |x-y|$ gelten. Da dies für alle $x,y \in D$ liegt können wir diese im Intervall frei wählen. Wählt man nun zwei Werte (z.B. $x=2y, y \in D$) und formt man die Ungleichung nach $L$ um, sodass der andere Term nicht nach oben beschränkt ist (und somit $L$ nicht konstant sein kann), so ist die Funktion nicht lipschitz stetig.