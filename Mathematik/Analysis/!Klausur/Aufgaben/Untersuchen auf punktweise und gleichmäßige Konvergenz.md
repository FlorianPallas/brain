# Untersuchen auf punktweise und gleichmäßige Konvergenz
## Verfahren
Grenzfunktion bestimmen nach Definition $f(x) := \lim\limits_{n \to \infty} f_{n}(x)$. Existiert der Grenzwert, so ist $(f_{n})$ punktweise konvergent.

Aus der Stetigkeit der Grenzfunktion, etc. geg. auf gleichmäßige Konvergenz schließen (siehe Sätze).

Abstand von Funktionenfolge und Grenzfunktion betrachten (wenn nicht stetig in verschiedenen Teilintervallen). Ist der Abstand durch eine Nullfolge begrenzt, so konvergiert $(f_{n})$ gleichmäßig gegen $f$. Achtung! Hier ist nicht der Grenzwert gemeint, sondern die neue Folge selbst. Hier ist oft relevant welche Werte $x$ annehmen kann.

## Sätze
Ist die Funktionenfolge stetig, die Grenzfunktion allerdings nicht, herrscht nur punktweise Konvergenz.

Ist die Funktionenreihe eine Potenzreihe, so konvergiert sie gleichmäßig auf allen kompakten Intervallen des Konvergenzbereiches.

Ist der Abstand zwischen Funktionenfolge und Grenzfunktion durch eine Nullfolge (die kein $x$ enthält!) nach oben beschränkt $|f_{n}(x) - f(x)| \leq \alpha_{n}$, so konvergiert $(f_{n})$ gleichmäßig gegen $f$.

Ist der Betrag der Funktionenfolge einer Funktionenreihe durch eine die Funktionenfolge einer anderen Funktionenreihe nach oben beschränkt $|f_{n}(x)| \leq c_{n}$, so konvergiert die originale Funktionenreihe gleichmäßig (Kriterium von Weierstraß).

Ist der Abstand nicht die Nullfunktion (auflösen von $n$ mittels beliebigen $x$ notwendig, z.B. $x = \frac{1}{n}$), so definieren ein $\epsilon$, sodass das Ergebnis größer als Epsilon ist (Beweis durch Widerspruch).