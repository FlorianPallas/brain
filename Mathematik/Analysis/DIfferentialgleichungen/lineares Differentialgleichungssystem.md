---
aliases: [DGL-System, DGL-Systems, homogenes DGL-System, inhomogenes DGL-System, homogen, inhomogen]
---

# lineares Differentialgleichungssystem #card
## Definition
Ein System von [[Differentialgleichung|Differentialgleichungen]] der Form
$$
\begin{pmatrix} 
y_{1}'(x) = a_{11} y_{1}(x) + \cdots + a_{1n} y_{n}(x) + b_{1} \\ \vdots \\ 
y_{n}(x) = a_{n1} y_{n}(x) + \cdots + a_{nn} y_{n}(x) + b_{n}
\end{pmatrix}
$$
heißt **lineares DGL-System** erster Ordnung für $y_{1}, \cdots, y_{n}: I \subseteq \mathbb{R} \to \mathbb{R}$.
Äquivalent: $y'(x) = A \cdot y(x) + b$ (Matrixschreibweise)

Es heißt **homogen** wenn $b = 0$ und **inhomogen** sonst.

## Verfahren
### homogene Systeme
Die [[Lösungsmenge]] eines homogenen DGL-Systems erster Ordnung, bilden einen $n$-dimensionalen [[Untervektorraum]] von $C(\mathbb{R}, \mathbb{R}^n)$. Eine [[Basis]] davon heißt Fundamentalsystem und lässt sich wie folgt bestimmen.
1. Bestimme alle [[Eigenwerte|Eigenwerte]] $\lambda_{j}$ und ihrere [[Vielfachheiten|algebraischen Vielfachheiten]] $k_{j}$ ($j \in [1,r]$, $r \in \mathbb{N}$).
2. Für jeden _reellen_ Eigenwert  $\lambda \in \mathbb{R}$, bestimme eine Basis des [[Eigenraum|Eigenraums]] $E_{A}(\lambda)$ und ergänze diesen zu eine Basis vom [[Hauptraum]] $H_{A}(\lambda)$.
$$
    \{0\} \neq E_{A}(\lambda) =  Kern(A - \lambda I_{n}) \subseteq Kern((A - \lambda I_{n})^{2}) \subseteq \cdots \subseteq Kern((A - \lambda I_{n})^{k}) = H_{A}(\lambda)
$$
3. Für jeden Basisvektor $v \in \mathbb{R}^{n}$ von $H_{A}(\lambda)$ ist
$$
    y(x) = e^{\lambda x} \sum\limits_{i=0}^{k-1} \frac{x^{i}}{i!} (A - \lambda I_{n}) ^{i} v
$$
eine Lösung des homogenen DGL-Systems.
4. Die nicht-reellen Eigenwerte treten in Paaren mit dem komplex-konjugierten auf. Bestimme für nur einen davon, mit dem gleichen Verfahren wie bei (2), $y(x)$, dann sind für jeden Basisvektor $v$ von $H_{A}(\lambda)$ die Funktion
$$
Re(y(x)) \ {\text{und}} \ Im(y(x))
$$
ebenso Lösungen des homogenen Systems.

Die gefundenen Lösungen ergeben zusammen ein Fundamentalsystem. Die allgemeine Lösung ist $y(x) = c_{1} y^{(1)}(x) + \cdots + c_{n} y^{(n)}(x)$ mit $c_{1}, \cdots, c_{n}$ beliebig.

### inhomogene Systeme
^c-nlsUGxLCDE

---
**Tags**: #todo 