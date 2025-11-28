Mit dem Lambda Kalkül lassen sich Funktionale Programmiersprachen wie Haskell theoretisch beschreiben. Auf deren Grundlage kann man dann Analysen, wie zum Beispiel [[Typinferenz]] ausführen.

---

## Terminologie

### Variablen
$x,y$
### Funktionen
$\lambda x.t$
Das ist nichts anderes als die anonyme Funktion $f(x) = t$. $x$ hat dabei keinen festen Typ. Bei der Auswertung wird $x$ in den Ausdruck $t$ eingesetzt.
$f(x) = x$ ist $\lambda x.x$
### Redex
Alle Ausdrücke die ein $\lambda$ besitzen werden Redex gennannt.

---

## Reduktion
- Die Auswertung ist links-assoziativ
- Die Auswertung erfolgt für jede Variable einzeln
- Die Auswertung ist damit gecurried

Beispiel

Quadrieren
$\lambda x.x \cdot x$
$(\lambda x.x \cdot x)2 = 2 \cdot 2 = 4$

Multiplizieren
$\lambda x. \lambda y. x \cdot y$
$(\lambda x. \lambda y. x \cdot y)4 \ 2 = 4 \cdot 2 = 8$
$(\lambda x. \lambda y. x \cdot y)4 \ 2 = (\lambda y. 4 \cdot y) 2 = 4 \cdot 2 = 8$

---

## Alpha Äquivalenz
[Video](https://www.youtube.com/watch?v=CeU5CrvsPuw&list=PLNmsVeXQZj7oBz3PP5sGIkLnmBbw10UUP&index=2)
Zwei Funktionen sind Alpha Äquivalent, wenn sie bis auf die Variablennamen identisch sind. Die Funktionen liefern bei selben Eingaben, die selben Ausgaben. Es gibt eine Zuweisung der Variablen von Funktion A zu Funktion B, sodass A und B identische sind.
$\lambda x.x = \lambda y.y$

---

## Beta Reduktion
[Video](https://www.youtube.com/watch?v=9sFgP105EJg&list=PLNmsVeXQZj7oBz3PP5sGIkLnmBbw10UUP&index=3)
Wir können Redexe in beliebiger Reihenfolge reduzieren. Bei meheren Funktionsvariablen natürlich aber von links nach rechts ($(\lambda x. \lambda y = x \cdot y) (1 \ 2)$ hier erst $x$ dann $y$).

### Beispiel
$(\lambda x.x)(\lambda x. \lambda y.x \cdot y(\lambda z. (\lambda x.x) z))$
Wir können hier also wählen:
- $\lambda x.x$ (vorne)
- $\lambda x.x$ (hinten)
- $\lambda z. (\dots) z$
- $\dots$

$(\lambda x.x)(\lambda x. \lambda y.x \cdot y(\lambda z. (\lambda x.x) z))$
$(\lambda x.x)(\lambda x. \lambda y.x \cdot y(\lambda z.z))$
$(\lambda x.x)(\lambda y.(\lambda z.z) \cdot y)$
$(\lambda y.(\lambda z.z) \cdot y)$
-> Keine weitere Reduktion möglich (keine Variablenwerte)

---

## Normalform
[Video](https://www.youtube.com/watch?v=rNmPopvqAzc&list=PLNmsVeXQZj7oBz3PP5sGIkLnmBbw10UUP&index=4)
Immer den links äußersten Redex zuerst reduzieren -> Normalreihenfolge

### Beispiel
$(\lambda x. (\lambda y. x (\lambda z.z)y))((\lambda a.a)(\lambda b.b))$
$(\lambda y. ((\lambda a.a)(\lambda b.b)) (\lambda z.z)y)$
$(\lambda y. (\lambda b.b) (\lambda z.z)y)$
$(\lambda y. (\lambda z.z)y)$
$(\lambda y. y)$
-> Normalform

---

## Call by Name
[Video](https://www.youtube.com/watch?v=qx5h6-uLork&list=PLNmsVeXQZj7oBz3PP5sGIkLnmBbw10UUP&index=5)
- Immer nur den links äußersten Redex reduzieren (Normalreihenfolge)
- Aber: Reduktionen innerhalb eines Lambda Terms sind nicht erlaubt

### Beispiel
$(\lambda x. (\lambda y. x (\lambda z.z)y))((\lambda a.a)(\lambda b.b))$
$(\lambda y. ((\lambda a.a)(\lambda b.b)) (\lambda z.z)y)$
Eigentlich jetzt $\lambda a.a$ reduzieren. Aber dieser Ausdruck ist von $\lambda y$ umgeben
-> Keine weitere Reduktion möglich

Call by Name findet Anwendung in Haskell.

---

## Call by Value
[Video](https://www.youtube.com/watch?v=qx5h6-uLork&list=PLNmsVeXQZj7oBz3PP5sGIkLnmBbw10UUP&index=5)
- Immer nur den links äußersten Redex reduzieren (Normalreihenfolge)
- Aber: Reduktionen innerhalb eines Lambda Terms sind nicht erlaubt
- Aber: Nur wenn die rechte Seite des Redex bereits in Normalform ist

$(\lambda x. (\lambda y. x (\lambda z.z)y))((\lambda a.a)(\lambda b.b))$
Eigentlich jetzt $\lambda x$ reduzieren. Aber $((\lambda a.a)(\lambda b.b))$ ist nicht in Normalform. Daher wird dieser Ausdruck zuerst reduziert.
$(\lambda x. (\lambda y. x (\lambda z.z)y))(\lambda b.b)$
Jetzt ist reduzieren von $\lambda x$ möglich
$(\lambda y. (\lambda b.b) (\lambda z.z)y)$
Eigentlich jetzt $\lambda b.b$ reduzieren, aber ist von $\lambda y$ umgeben.
-> Keine weitere Reduktion möglich

Call by Value findet Anwendung in Java und C.

---

## Church Zahlen
[Video](https://www.youtube.com/watch?v=qx5h6-uLork&list=PLNmsVeXQZj7oBz3PP5sGIkLnmBbw10UUP&index=6)

Der Lambda Kalkül hat eigentlich keine natürlichen Zahlen, sondern nur Variablen und Funktionen. Deswegen definiert man sich die Church Zahlen $c_n$.

$c_0 = \lambda s. \lambda z. z$
$c_1 = \lambda s. \lambda z. s \ z$
$c_2 = \lambda s. \lambda z. s \ (s \ z)$
$c_3 = \lambda s. \lambda z. s \ (s \ (s \ z))$
$\dots$
$c_n = \lambda s. \lambda z. s^n \ z$
-> Die Funktion $s$ wird $n$ mal angewendet

### Successor Funktion
Gibt den Nachfolger einer natürlichen Zahl $n$ an.
$succ = \lambda n . \lambda s. \lambda z. s (n \ s \ z)$

$succ \ c_1$
$\lambda n . \lambda s. \lambda z. s (n \ s \ z) (c_1)$
$\lambda n . \lambda s. \lambda z. s (n \ s \ z) (\lambda s. \lambda z. s \ z)$
$\lambda s. \lambda z. s ((\lambda s. \lambda z. s \ z) \ s \ z)$
Wir reduzieren jetzt hinten zuerst ($\beta$ Reduktion)
$\lambda s. \lambda z. s ((\lambda z. s \ z) \ z)$
$\lambda s. \lambda z. s (s \ z)$
$c_2$

$succ \ c_n$
$\lambda n . \lambda s. \lambda z. s (n \ s \ z) (c_n)$
$\lambda n . \lambda s. \lambda z. s (n \ s \ z) (\lambda s. \lambda z. s^n \ z)$
$\lambda s. \lambda z. s ((\lambda s. \lambda z. s^n \ z) \ s \ z)$
$\lambda s. \lambda z. s ((\lambda z. s^n \ z) \ z)$
$\lambda s. \lambda z. s (s^n \ z)$
$c_{n+1}$

---

## Addition
[Video](https://www.youtube.com/watch?v=L1YbhqcBXDw&list=PLNmsVeXQZj7oBz3PP5sGIkLnmBbw10UUP&index=7)

$add = \lambda n . \lambda m . \lambda s . \lambda z \ n \ s (m \ s \ z)$

$add \ c_2 \ c_2$
$\lambda n . \lambda m . \lambda s . \lambda z \ n \ s (m \ s \ z) (c_2) (c_2)$
$\lambda n . \lambda m . \lambda s . \lambda z \ n \ s (m \ s \ z) (\lambda s. \lambda z. s (s \ z)) (\lambda s. \lambda z. s (s \ z))$
$n$ und $m$ reduzieren
$\lambda s . \lambda z \ (\lambda s. \lambda z. s (s \ z)) \ s \ ((\lambda s. \lambda z. s (s \ z)) \ s \ z)$
$\lambda s . \lambda z \ (\lambda z. s (s \ z)) \ ((\lambda s. \lambda z. s (s \ z)) \ s \ z)$
$\lambda s . \lambda z \ (s (s \ (\lambda s. \lambda z. s (s \ z)) \ s \ z))$
$\lambda s . \lambda z \ (s (s \ (\lambda z. s (s \ z)) \ z))$
$\lambda s . \lambda z \ (s (s \ (s (s \ z))))$
$c_4$

---

## Multiplikation

---

## Boolsche Ausdrücke

---

## Typsysteme
[Video](https://www.youtube.com/watch?v=xgQRhVQY3mM&list=PLNmsVeXQZj7oBz3PP5sGIkLnmBbw10UUP&index=10)

- $\Gamma$ Typkontext der alle relevanten Variablen enthält (z.B. x -> int; y -> bool)
- $|-$ Herleitung

---

## Abstrakionsregel
[Video](https://www.youtube.com/watch?v=dQnoxO4SQUI&list=PLNmsVeXQZj7oBz3PP5sGIkLnmBbw10UUP&index=11)

$\Gamma: x \to int; y \to bool;$
$\Gamma \ |- (\lambda x.x \ 0) : (int \to bool) \to bool$



## Let Regel
[Video](https://www.youtube.com/watch?v=ZL3kqMmMyZg&list=PLNmsVeXQZj7oBz3PP5sGIkLnmBbw10UUP&index=15)

