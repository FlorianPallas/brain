- [x] JNF
- [x] Orthogonal Projektion
- [ ] Adjungierte Abbildungen
- [x] Skalarprodukt
- [x] INF


## JNF
1. Charakteristisches Polynom berechnen
2. Eigenräume berechnen
3. Wenn $AV \neq GV$ Haupträume berechnen
4. Vom Hauptverktor höchster Stufe Kernkette beginnen
	- Multiplizieren mit $A - \lambda I$ gibt nächsten Vektor
5. In Wechselmatrix neuesten bist zu ältesten Vektor eintragen -> 1sen über der Diagonale

## Determinante
- 2x2 Inversenregel: $\begin{pmatrix} a & b \\ c & d \end{pmatrix}^{-1} = 1/det(A) \begin{pmatrix} d & -b \\ -c & a \end{pmatrix}$

### Drehkästchen
$D_{\alpha} = \begin{pmatrix} \cos \alpha & -\sin \alpha \\ \sin \alpha & \cos \alpha \end{pmatrix}$
> $\cos$ auf der Diagonale

### GSV
#### Orthogonalisieren
$$
b_{j} := a_{j} - \sum_{k=1}^{j-1} \frac{<a_{j}, b_{k}>}{<b_{k}, b_{k}>} \cdot b_{k}
$$
> Ziehe vom Vektor alle orthogonalen Abhängigkeiten zu bisherigen Vektoren ab

#### Normalisieren
$c_j := \frac{1}{<b_{j}, b_{j}>} \cdot b_j$

## INF
1. Isometrie zeigen $A \cdot A^T = I$
2. Charakteristisches Polynom berechnen
3. Eigenwerte bestimmen

### Transpositionstrick
1. Berechne einfachrere Matrix $B = A + A^T$ auf
2. $\mathcal{X}_B(x)$ und Eigenwerte von $B$ berechnen
	- Eigenwerte $\lambda = \pm 2$ von $B$ entsprechen den Eigenwerten $\lambda = \pm 1$ von $A$. Die algebraischen Vielfachheiten bleiben erhalten.
	- Paare von Eigenwerte $\lambda \in (-2,2)$ entsprechen einem Drehkästchen / einem komplexen Eigenwert in $A$. Es gilt $\cos \alpha = \frac{1}{2} \lambda$ und $\sin \alpha = \sqrt{1 - \cos \alpha}$
3. Stelle ENF / INF $\widetilde{A}$ auf
4. Berechne Eigenräume von $B$
	- Benutze $B$ als Matrix im Kern!
5. Stelle für Eigenwerte $\lambda = \pm 2$ mit dem GSV eine ONB des Eigenraums auf.
6. Für Eigenwerte $\lambda \in (-2,2)$ muss der zweite Vektor mittels $y = A \cdot x$ berechnet werden. Berechne dann Analog zu den anderen Eigenwerten eine ONB von $[x,A \cdot x]$.
7. Schreibe die ONB Vektoren in der passenden Reihenfolge in die Wechselmatrix
8. Für die Drehkästchenvektoren prüfe die Reichenfolge
	- $A \cdot v_i$ muss die $i$-te Spalte von $A$ erzeugen
9. Es gilt $\widetilde{A} = S^{-1} \cdot A \cdot S$