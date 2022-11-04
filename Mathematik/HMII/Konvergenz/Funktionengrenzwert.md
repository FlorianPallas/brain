# Funktionengrenzwert
## Definition #card 
Der [[Mathematik/HMII/Konvergenz/Grenzwert]] $y_{0} \in \mathbb{R}^m$ einer [[Funktion]] $f: D \subseteq \mathbb{R}^{n} \to \mathbb{R}^m$ gegen ein $x_{0}\in \mathbb{R}^n$ ist definiert genau dann wenn für jede [[Folge]] $(x^{(k)})$ in $D \setminus \{x_0\}$ mit $x^{(k)} \to x_{0}$ $(k \to \infty)$ gilt: $f(x^{(k)}) \to y_{0}$ $(k\to\infty)$.
In diesem Fall existiert der Grenzwert der Funktion $f$ und man schreibt: $f(x) \to y_{0}$ $(x \to x_{0})$.

Gibt es nun auch nur eine Folge unter obigen Bestimmungen welche [[Divergenz|divergiert]], oder zwei Folgen welche nicht gegen den selben Wert [[Mathematik/HMII/Konvergenz/Konvergenz|konvergieren]], existiert der Grenzwert nicht.

Im $\mathbb{R}^n$ müssen nun alle Folgen berücksichtigt werden, nicht nur Folgen welche sich von links und rechts dem Grenzwert nähern.
![[Pasted image 20220503143105.png]]
^c-ZoSKvSAnQv

## Verfahren #card
- [[Definitionsmenge]] bestimmen
- (Ist der Punkt gegen den die Funktion geht ein [[Häufungspunkt]]?)
- Zeigen dass der Grenzwert nicht existiert
  - Widerspruch mittels divergierender Folge
  - Widerspruch mittels zweier Folgen mit unterschiedlichen Grenzwerten
- Zeigen dass der Grenzwert existiert
  - Simples einsetzen
  - Grenzwert Rechenregeln anwenden
  - [[Sandwich-Lemma]] nutzen (geg. komponentenweise anwenden)
^c-XJzxFwCWDr

## Beispiele
### Grenzwert existiert nicht
Mittels Divergenz
![[Pasted image 20220503143806.png]]

Mittels verschiedener Folgen Grenzwerte
![[Pasted image 20220503144231.png]]

### Grenzwert existiert
Simples einsetzen
![[Pasted image 20220503144135.png]]

Mittels Grenzwert Rechenregeln
![[Pasted image 20220503143916.png]]

Mittels Sandwich-Lemma
![[Pasted image 20220503144015.png]]

---
**Tags**: 