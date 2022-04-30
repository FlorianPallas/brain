---
aliases: LGS
---

# Lineare Gleichungssysteme
## Definition
Ein lineares Gleichungssystem (LGS) mit $m$ Gleichungen und $n$ Unbestimmten $x_{1}, \ldots, x_{n}$ ist gegeben durch
$$\begin{aligned}
&a_{11} x_{1}+a_{12} x_{2}+\ldots+a_{1 n} x_{n}=b_{1}\\
&a_{21} x_{1}+a_{22} x_{2}+\ldots+a_{2 n} x_{n}=b_{2}\\
& \;\;\;\; \vdots \;\;\;\;\;\;\;\;\;\;\; \vdots
\;\;\;\;\;\;\;\;\;\;\;\;\;\;\;\;\;\;\;\; \vdots
\;\;\;\;\;\;\;\;\ \vdots \\
&a_{m1} x_{1}+a_{m2} x_{2}+\ldots+a_{m n} x_{n}=b_{m}
\end{aligned} $$
Die $a_{i j}, b_{i}$ für $i=1, \ldots, m$ und $j=1, \ldots, n$ heißen Koeffizienten und sind gegebene reelle Zahlen. Die $x_{j}$ für $j=1, \ldots, n$ heißen Unbestimmte (oder Unbekannte oder Variablen) und sind gesucht.
### Homogenes LGS
Sind in alle $b_{i}=0(i=1, \ldots, m)$, so heißt das LGS homogen, und sonst inhomogen.
## Alternative Darstellung
### Erweiterte Matrix
Einem Linearen Gleichungssystem kann eine [[Matrix]] und eine erweiterte [[Matrix]] zugeordnet werden:
$$\left(\begin{array}{ccccc}
a_{11} & a_{12} & \cdots & a_{1 n}  \\
a_{21} & a_{22} & \cdots & a_{2 n}  \\
\vdots & \vdots & \ddots & \vdots  \\
a_{m 1} & a_{m 2} & \cdots & a_{m n} 
\end{array}\right) \text{ und } \left(\begin{array}{ccccc}
a_{11} & a_{12} & \cdots & a_{1 n} & b_{1} \\
a_{21} & a_{22} & \cdots & a_{2 n} & b_{2} \\
\vdots & \vdots & \ddots & \vdots & \vdots \\
a_{m 1} & a_{m 2} & \cdots & a_{m n} & b_{m}
\end{array}\right)$$
### Lineare Abbildung
Ein linearen Gleichungssystem kann auch als [[Lineare Abbildung]] aufgefasst werden:
$$\left(\begin{array}{ccccc}
a_{11} & a_{12} & \cdots & a_{1 n}  \\
a_{21} & a_{22} & \cdots & a_{2 n}  \\
\vdots & \vdots & \ddots & \vdots  \\
a_{m 1} & a_{m 2} & \cdots & a_{m n} 
\end{array}\right) \cdot \left(
\begin{array}{c}
x_1 \\
x_2 \\
\vdots  \\
x_n \\
\end{array}
\right)
= \left(
\begin{array}{c}
b_1 \\
b_2 \\
\vdots  \\
b_n \\
\end{array}
\right)
$$
## Lösungsmenge
### Definition
Die Lösungsmenge des reellen linearen Gleichungssystems ist die Teilmenge $\mathcal{L}$ von $\mathbb{R}^{n}$ bestehend aus allen $n$-Tupeln $\left(x_{1}, \ldots, x_{n}\right)$, die bei gegebenen Koeffizienten $a_{i j}, b_{i}(i=1, \ldots, m$ und $j=1, \ldots, n)$ alle $m$ Gleichungen in simultan erfüllen.
### Bestimmung
Die Lösungsmenge eines linearen Gleichungssystem wird mit dem [[Gauß Algorithmus]] bestimmt.
### Größenordnung
- Keine Lösung :: Wenn die Matrix eine Nullzeile enthält, aber die erweiterte Matrix keine aufweist. Also, wenn das entsprechende $b$ von einer Zeile mit nur Nullen als $a$ nicht null ist. 
- Eine Lösung :: Wenn die Matrix [[Vollrang]] hat.
- Unendlich viele Lösungen :: Wenn die erweiterte Matrix eine Nullzeile enthält.
### Lösbarkeitskriterien
1. Das LGS $A x=b$ ist genau dann lösbar, wenn für die lineare Abbildung $\Phi: \mathbb{K}^{n} \longrightarrow \mathbb{K}^{m} ; x \mapsto A x$ gilt, dass $b \in \operatorname{Bild} \Phi$.
2. Das LGS $A x=b$ ist genau dann lösbar, wenn gilt $\operatorname{Rang} A=\operatorname{Rang}(A \mid b)$.
3. Ein homogenes lineares Gleichungssystem besitzt genau dann eine nicht triviale Lösung, wenn $\operatorname{ Kern } \Phi \neq\{0\}$ also wenn es kein [[Vollrang]] besitzt.
## Verwandte Themen
[[Lineare Gleichung]]
