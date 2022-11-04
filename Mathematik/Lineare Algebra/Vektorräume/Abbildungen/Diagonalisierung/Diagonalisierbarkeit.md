## Definition #card
Eine [[Matrix]] $A \in K^{nxn}$ heißt diagonalisierbar, wenn es eine [[Basis]] $S$ gibt, sodass die Matrix $A$ zu dieser Basis abgesehen von der Diagonale nur mit Nullen gefüllt ist.
Auf der Diagonale stehen dabei stets die zugehörigen [[Eigenwerte|Eigenwerte]] von $A$. Diese tauchen dabei gemäß ihrer [[geometrischen Vielfachheit]] auch mehrmals auf.
^c-PkErQuSXWr

## Kriterien
Die Matrix $A$ ist genau dann diagonalisierbar, wenn eines der folgenden Kriterien erfüllt ist.

### Standard Kriterium #card
Es gibt eine [[Basiswechsel]] der $A$ auf die gewünschte Form bringt.
$\exists S \in Gl_n(K): S^{-1} A S = \begin{pmatrix}\lambda_1 & 0 & 0 \\ 0 & \lambda_2 & 0 \\ 0 & 0 & \lambda_3\end{pmatrix}$
^c-BlSwpji56D

### Basen Kriterium #card
Es gibt eine Basis $B$ des Vektorraum $V$, welche aus den [[Eigenvektor|Eigenvektoren]] von $A$ besteht.
^c-B7FYZA3Q2b

### Summen Kriterium #card
Der $K^n$ ist die [[direkte Summe]] der jeweiligen [[Eigenraum|Eigenräume]]. Es gilt $K^n = \oplus E_\lambda$, wobei jedes $\lambda$ Eigenwert von $A$ ist.
^c-BODMISV0Mq

### Vielfachheiten Kriterium #card
Das [[charakteristisches Polynom|charakteristische Polynom]] $p_A(X)$ zerfällt vollständig in [[Linearfaktoren]] unter dem gegebenen Körper $K$. Als Konsequenz gibt es genau $n$ Eigenwerte.
Zudem müssen auch genügend Eigenvektoren existieren. Es muss also gelten $GV = AV$. Die Vielfachheiten stimmen überein.
^c-IO9P3p3q7Q

### Dimensions Kriterium #card
Die Summe der Dimensionen aller Eigenräume müssen $n$ ergeben. Es gilt $\sum dim(E_\lambda) = n$.
^c-stMIjYZEb3



