---
cards-deck: Theoretische Informatik
---

# Landau Notation
## Motivation #card 
Die Landau Notation wird verwendet, um die Laufzeit von Algorithmen in Klassen einteilen zu können. Es werden grobe Laufzeitklassen gebildet, da es zu aufwändig und unpraktikabel ist einen Algorithmus ins Detail zu analysieren.
^1651073591955

## Definitionen #card 
### Original Definition
![[Pasted image 20220420162108.png]]
### Grenzwert Definition
![[Pasted image 20220420162729.png]]
^1651073591964

## Ordnung auf Funktionen #card 
![[Pasted image 20220420162332.png]]
![[Pasted image 20220420163015.png]]
Merke: Alle Logarithmen wachsen langsamer als [[Polynom|Polynome]] mit positiven reellen Exponenten
^1651073591986

## Rechenregeln #card 
![[Pasted image 20220420162416.png]]
![[Pasted image 20220420162430.png]]
![[Pasted image 20220420162446.png]]
$\sum_{i} c^{i}$ wird asymptotisch vom größten Summanden dominiert, also: $\sum_{i=a}^{b} c^{i} \in \Theta\left(c^{a}+c^{b}\right),$ falls $c \neq 1$. Die Indizes $a$ bis $b$ dürfen von $n$ abhängen.
^1651073591992

## Rechentipps #card 
- Abschätzungen sind in der Ungleichung erlaubt, sofern diese die Ungleichung einschränken.
- Oft bietet sich an den Logarithmus zu ziehen
- Manchmal bietet sich Substitution an
^1651073591997

## Anmerkungen #card 
- $\Theta$ ist eine [[Äquivalenzrelation]] 
- $\Theta (n \log n)$ wird als quasi-linear bezeichnet
^1651073592002
