# Gleitkommazahlen

## Verwendung

Für die Darstellung von betragsmäßig sehr kleinen oder großen Zahlen

## Allgemeine Darstellung

$$X=\pm \text { Mantisse } \cdot b^{\text {Exponent }}$$

- Die Basis $b$ ist für bestimmte Gleitkommadarstellungen fest (meist $2$ oder $16$)

## Maschinenformat

![[Pasted image 20220426180813.png]]

- Sowohl für Charakteristik als auch für Mantisse wird im Rechner eine feste Anzahl von Speicherstellen festgelegt
- Das erste Bit gibt das Vorzeichen an
- Charakteristik
  - ist die [[Exzess-q Darstellung|Charakteristik]] des Exponenten.
  - bestimmt die Größe des Zahlenbereichs
- Mantisse - bestimmt die Genauigkeit der Darstellung - ist die Lage des Kommas wieder durch Vereinbarung festgelegt - Meist links vom [[Most Significant Bit]]

## Normalisierung

Eine Gleitkommazahl heißt normalisiert, wenn für den Wert der Mantisse gilt:
$$\frac{1}{b} \leq 0, \text { Mantisse}_{2}<1$$

### Beispiel

$1\;1011\;1101\;1111_{2}$ normalisiert ergibt $0,1\;1011\;1101\;1111_{2} \cdot 2^{13}.$ Somit ist die normalisierte Mantisse $1011\;1101\;1111$.

### Sonderfall $b=2$

In der dualen Darstellung ist die erste Stelle nach dem Komma mit der Ausnahme der Zahl $0$ immer gleich 1. Deshalb wird dieses Bit meist erst gar nicht dargestellt. Dadurch wird Speicherplatz gespart oder die Genauigkeit wird erhöht bei gleichem Speicherbedarf. Bei arithmetischen Operationen und bei Konversion in andere Darstellungen muss diese Stelle natürlich wieder eingefügt werden.

### Maschinenformat Implementierungen

## Wichtige Konstanten

- **maxreal** ist die größte darstellbare normalisierte positive Zahl
- **minreal** ist die kleinste darstellbare normalisierte positive Zahl
- **smallreal** ist die kleinste Zahl, die man zu $1$ addieren kann, um einen von $1$ verschiedenen Wert zu erhalten

## Verletzte Rechenregeln

- Die Zahlenmenge ist nicht abgeschlossen
- [[Assoziativgesetz]] und [[Distributivgesetz]] gelten nicht, da bei der Anwendung der Gesetze evtl. der darstellbare Zahlenbereich verlassen wird
- Das [[Assoziativgesetz]] ist des Weiteren verletzt, wenn große mit kleinen Zahlen verrechnet werden $$\begin{aligned}
&(x+y)+z=\left(1+\frac{\text { smallreal }}{2}\right)+\frac{\text { smallreal }}{2}=1+\frac{\text { smallreal }}{2}=1 \\
&x+(y+z)=1+\left(\frac{\text { smallreal }}{2}+\frac{\text { smallreal }}{2}\right)=1+\text { smallreal } \neq 1
\end{aligned}$$

## IEEE-P 754-Floating-Point-Standard

## Varianten

![[Pasted image 20220509085714.png]]

## Eigenschaften

- Basis $b=2$
- Normalisiert wird so, dass das erste Bit der Mantisse (die implizite 1) vor dem Komma steht.
- Das erste Bit der Mantisse wird implizit zu 1 angenommen, wenn die Charakteristik nicht nur Nullen enthält.
- Ist die Charakteristik gleich 0, entspricht dies dem gleichen Exponenten wie die Charakteristik 1, nur wird dann das erste Bit der Mantisse explizit dargestellt (d. h. dadurch ist auch die Null darstellbar) und die Normalisierung folgt den üblichen Grundsätzen.
- Sind alle Bits der Charakteristik gleich 1, signalisiert dies eine Ausnahmesituation. Ist zusätzlich die Mantisse gleich Null, bedeutet dies einen „overflow" (bzw. $\pm \infty)$, andernfalls „NaN" (not a number). Dies erlaubt es dem Prozessor, eine Fehlerbehandlung einzuleiten.

## Veranschaulichung

![[Pasted image 20220509084436.png]]

## Hinweise

![[Pasted image 20220509084837.png]]

## Umrechnung

### Umrechnung von Dezimal zu Gleitkommazahl

- Vorzeichenbit wählen
- Zahl in Binär darstellen
- Zahl im Binären normalisieren nach IEEE-P 754-Floating-Point-Standard
- Exponent der normalisierten Zahl ablesen
- Charakteristik ausrechnen: $\text{Charakteristik} = 2^{8\text{ oder }11}-1+\text{Exponent}$
- Mantisse aufstellen = normalisierte Binärzahl ohne die erste Stelle und ohne den Faktor
  ![[Pasted image 20220509090016.png]]
