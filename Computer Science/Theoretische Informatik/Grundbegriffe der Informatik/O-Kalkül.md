# O-Kalkül
---

# Schranken

## Obere Schranke
In $O(f(n))$ sind alle Funktionen die langsamer oder gleich schnell wachsen wie $f$.

Es gilt $O(f(n)) = \{g(n)|\exists c \in \mathbb{R}^+ : \exists n_0 \in \mathbb{N}_0 : \forall n \geq n_0 : g(n) \leq c · f(n)\}$.

### Mittlere Schranke
In $\Theta(f(n))$ sind alle Funktionen die gleich schnell wachsen wie $f$.

Es gilt $\Theta(f(n)) = \{g(n)|\exists c_1, c_2 \in \mathbb{R}^+ : \exists n_0 \in \mathbb{N}_0 : \forall n \geq n_0 : c_1 f(n) \leq g(n) \leq c_2 f(n)\}$ oder $O(f(n)) \cap \Omega(f(n))$.

### Untere Schranke
In $\Omega(f(n))$ sind alle Funktionen die schneller oder gleich schnell wachsen wie $f$.

Es gilt $\Omega(f(n)) = \{g(n)|\exists c \in \mathbb{R}^+ : \exists n_0 \in \mathbb{N}_0 : \forall n \geq n_0 : g(n) \geq c · f(n)\}$.


## Master-Theorem
Das Master-Theorem ermöglicht Laufzeitabschätzungen für rekursive Algorithmen. Die Funktionen der Algorithmen müssen dabei folgende Form besitzen: $T(n) = a \cdot T(n/b) + f(n)$. Dabei ist $a$ die Anzahl der Teilprobleme, $n/b$ die Größe der Teilprobleme und $f(n)$ eine von $T(n)$ unabhängige Funktion zur Kombination der Teilprobleme.

## Beispiele
