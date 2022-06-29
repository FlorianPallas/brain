---
aliases: []
---

# orthogonale Komplement #card
## Definition
Ist $M \subset V$ eine Teilmenge von Vektoren in $V$, so heißt
$$
M^{\perp}:=\{x \in V: x \perp M\}=\{x \in V:\langle x, y\rangle=0 \quad \forall y \in M\}
$$
das orthogonale Komplement von $M$ in $V .$
## Folgerungen
- $M^\perp$ ist ein [[Untervektorraum]] von $V$
- $U \subseteq (U^\perp)^\perp$ 
- Für endlichdimensionale [[Vektorraum|Vektorräume]] gilt: 
	- $U=(U^\perp)^\perp$ 
	- $V=U \oplus U^\perp$ wobei $U^\perp$ **eindeutig** ist.
	- bekannten [[Dimension|Dimensionsformeln]].    
- Für unendlichdimensionale [[Vektorraum|Vektorräume]] ist im Allgemeinen: 
	- $U \oplus U^{\perp} \subsetneq V$
	- $U \subsetneq\left(U^{\perp}\right)^{\perp}$
## Berechnung
### Über LGS
(Beispiel im Skript S. 52)
1. Bestimmen einer Basis $B$ von $M$
2. Skalarmultiplikation von jedem Basisvektor $b_j$ mit einem generischen Element aus $V$
3. Zusammenfassen der Ergebnisse zu einem hom. [[Lineares Gleichungssystem|LGS]]
4. Lösen des LGS
^c-cLlSWRXdy1
---
**Tags**: 