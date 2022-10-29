## Definition #card 
Sei $\Omega$ ein [[Grundraum]] und $\mathbb{P}$ ein [[diskretes Wahrscheinlichkeitsmaß]], dann heißt $(\Omega, \mathbb{P})$ diskreter Wahrscheinlichkeitsraum.
^c-Y87atCS0ab

## Satz: Rechengesetze #card 
Sei $(\Omega, P)$ ein diskreter Wahrscheinlichkeitsraum. Dann gilt
- $P (\emptyset)=0$
- $\forall A_1, \ldots, A_m \subseteq \Omega$ disjunkt, $m \in N : \quad P \left(\bigcup_{n=1}^m A_n\right)=\sum_{n=1}^m P \left(A_n\right)$
- $\forall A \subseteq \Omega: \quad P \left(A^c\right)=1- P (A)$
- $\forall A, B \subseteq \Omega, A \subseteq B: \quad P (B \backslash A)= P (B)- P (A)$, insbes. $P (A) \leq P (B)$
- $\forall A, B \subseteq \Omega: \quad P (A \cup B)= P (A)+ P (B)- P (A \cap B)$
^c-dIAIHwAclE