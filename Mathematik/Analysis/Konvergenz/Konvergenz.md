---
aliases: [konvergiert, Divergenz, divergiert, abs. konvergen, absolute konvergen, absolute Konvergenz]
---

# Konvergenz
## Definition
#todo

---
# Absolute Konvergenz
#todo

---
# Punktweise Konvergenz
## Definition
Eine [[Funktionenfolge]] $(f_n)$ heißt auf $D$ **punktweise konvergent,** genau dann wenn für jedes $x \in D$ die Folge $(f_{n}(x))$ [[Konvergenz|konvergent]] ist. In diesem Fall sei $f(x) := \lim\limits_{n \to \infty} f_{n}(x)$ die **Grenzfunktion** von $(f_{n})$.

#todo Definition für Funktionenreihen

---
# Gleichmäßige Konvergenz
## Definition
Während bei der Punktweisen Konvergenz die Grenzfunktion nur in einem Punkt der dem Grenzwert der Funktionenfolge gleicht, stellt die gleichmäßige Konvergenz anschaulich die Anforderung, dass sich $(f_{n})$ für alle $x \in D$ in einem $\epsilon$-Schlauch um die Grenzfunktion $f(x)$ befindet.

#todo Definition für Funktionenreihen

Aus gleichmäßiger Konvergenz folgt punktweise Konvergenz.

---
# Konvergenzkriterien für Folgen
## Monotoniekriterium
Eine monotone Folge konvergiert genau dann, wenn sie beschränkt ist.

## Cauchy-Kriterium
Eine Folge konvergiert genau dann, wenn sie eine Cauchy-Folge ist.

## Sandwichkriterium
Eine Folge konvergiert, wenn sie nach oben und unten durch konvergente Folge abgeschätzt werden kann, welche den gleichen Grenzwert haben.

## Reihenkriterien
Die Kriterien für Reihen können ebenfalls genutzt werden um auf eine Nullfolge und daraus folgende Konvergenz zu schließen.

---
# Konvergenzkriterien für Reihen
## Leibniz-Kriterium
Sei $(a_{n})$ eine monoton fallende, reelle Nullfolge, dann konvergiert die alternierende Reihe $\sum\limits_{n=0}^{\infty} (-1)^{n} a_{n}$.

## Majorantenkriterium
Sei $S = \sum\limits_{n=0}^{\infty} a_{n}$ beliebig und $T = \sum\limits_{n=0}^{\infty} b_{n}$ eine konvergente unendliche Reihe. Gilt für fast alle $n$ nun $|a_{n}| \leq b_{n}$, dann ist $S$ absolut konvergent.

## Minorantenkriterium
Gilt stattdessen für fast alle $n$ nun $a_{n} \geq b_{n}$ und ist $T$ ist divergent, dann ist auch $S$ divergent.

## Wurzelkriterium
Sei $S = \sum\limits_{n=0}^{\infty} a_{n}$.
Ist $\limsup \sqrt[n]{|a_{n}|} < 1$ für fast alle $n$, dann ist $S$ absolut konvergent. Ist der Wert $=1$ kann keine Aussage getroffen werden. Ist der Wert $> 1$, dann divergiert die Reihe.

## Quotientenkriterum


---
**Tags**: 