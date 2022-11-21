## Definition #card 
Sei $(\Omega, P )$ ein [[diskreter Wahrscheinlichkeitsraum]]. Zwei [[Ereignis|Ereignisse]] $A, B \subseteq \Omega$ heißen $\left( P _{-}\right)$stochastisch unabhängig, falls
$$
P (A \cap B)= P (A) \cdot P (B) .
$$

[[Ereignis|Ereignisse]] $A_1, \ldots, A_n \subseteq \Omega$ in einem 
[[diskreter Wahrscheinlichkeitsraum]] $(\Omega, P )$ heißen ( $P$-) stochastisch unabhängig, wenn für jede Indexmenge $I \subseteq\{1, \ldots, n\}, I \neq \varnothing$, gilt
$$
P \left(\bigcap_{i \in I} A_i\right)=\prod_{i \in I} P \left(A_i\right)
$$

Hinweise:
- Paarweise Unabhängigkeit reicht nicht aus
- Nur die Indexmenge $I=\{0,\dots,n\}$ reicht nicht aus
^c-6Ayg0oWVaZ

## Herleitung der Formel #card 
Es gilt $P(A|B)=\dfrac{P(A\cap B)}{P(B)}$. Falls $A$ und $B$ unabhänig sind, sollte gelten $P(A|B)=P(A)$.
Somit gilt:
$P(A)=\dfrac{P(A\cap B)}{P(B)}$
$\Leftrightarrow P(A) \cdot P(B) = P(A \cap B)$
^c-VzMRzD7FM8

## Zusammenhang mit Disjunktheit #card 
Disjunkt: $P(A \cap B) = 0$
Stoch. Unabhänig: $P(A \cap B) = P(A) \cdot P(B)$ 
Folglich sind disjunkte Ereignisse immer stochastisch unabhänig.
^c-A7wsgqSSMG