![[Pasted image 20250826184358.png]]
B ist die Basis. Meist 2.
M ist die Mantissenlänge, in IEEE 52 Bit, oder 24 Bit in Single.
E ist die Exponentenlänge, in IEEE 11 Bit, oder 8 Bit in Single.
-> 1 (Vorzeichen) + 52 + 11 = 64 Bit


$$
FL = \{ \text{Vorzeichen} + \text{Exponent} + \text{Mantissen Bits mit impliziter 1} \}
$$
$$
\text{Exponent} = \text{Minimaler Exponent} + {Exponenten Bits}
$$


Maschinengenauigkeit
![[Pasted image 20250826184605.png]]
Der maximale relative Rundungsfehler bei der Umwandlung zu einer Gleitkommazahl.

Ungefähre Werte für gängige Darstellungen
IEEE Double: $eps = 10^{-16}$
IEEE Single: $eps = 10^{-8}$


Ein Problem heißt **sachgemäß gestellt**, wenn es eindeutig lösbar ist und die Lösung stetig von den Daten abhängt.

Die **Kondition** eines Problems ist ein Maß dafür, wie stark die Lösung von den Daten abhängt.
-> Unvermeidbare Fehlerverstärkung bei optimaler Lösungsmethode

Die **Stabilität** eines numerische Algorithmus ist ein Maß dafür, wie stark die Daten-Abhängigkeit der numerischen Lösung zur tatsächlichen Lösung ist.
-> Der Algorithmus vergrößert den Fehler nicht zusätzlich

**Konditionszahl**
![[Pasted image 20250826211835.png]]

Addition und Multiplikation sind gut konditioniert

**Matrixkondition**
![[Pasted image 20250826212249.png]]

![[Pasted image 20250826213045.png]]

**Spaltensummenorm**: Beträge der Spalten summieren und den größten Wert wählen.
![[Pasted image 20250826213559.png]]

**Spektralnorm**: Wurzel des größten Eigenwerts von $A^\top A$
$A^T A$ ist symmetrisch, hat daher nur reelle Eigenwerte und EW >= 0, positiv semi-definit
![[Pasted image 20250826213501.png]]

**Zeilensummennorm**: Beträge der Zeilenelemente addieren und den größten Betrage wählen.
![[Pasted image 20250826213221.png]]

**Frobeniusnorm**: Alle Matrixelemente quadrieren, addieren und von der Summe die Wurzel ziehen
![[Pasted image 20250826213238.png]]

**Matrixkondition**
![[Pasted image 20250826213747.png]]