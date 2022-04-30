---
cards-deck: Technische Informatik
---

# Humming-Codes 
## $1$-Bit Fehlerkorrektur #card 
### Idee
Erweitere eine Codierung um [[Paritätsbit|Paritätsbits]], sodass ein $1$-Bit Fehler erkannt und verbessert werden kann. Angenommen das zu übermittelnde Codewort sei $n$ Bits lang. Dann müssen $n+1$ Fälle abgedeckt werden (Fehler an einer der n Bits oder kein Fehler). Die [[Paritätsbit|Paritätsbits]] müssen alle diese Fälle abdecken, also muss $2^k \geq n +1$ gelten. Die [[Paritätsbit|Paritätsbits]] müssen mit kodiert werden, sodass noch $m$ Bits für die eigentliche Nachricht übrig bleiben mit $2^k \geq k+m+1$.
### Umsetzung
1. Jeder Index einer $2$-er Potenz, also $\log_2 n$ Indizes werden für ein [[Paritätsbit]] reserviert. ![[Pasted image 20220429202835.png]]
2. An allen anderen Stellen wird das Codewort eingetragen. 
3. Berechnung der [[Paritätsbit|Paritätbits]]. Dabei ist jedes [[Paritätsbit]] ist für folgende Blöcke beginnend bei der $2$-er Potenz verantwortlich:
	![[Pasted image 20220429195032.png]]
4. Speichern / Übermitteln der Daten. Hierbei kommt es ggf. zu einem $1$-Bit Fehler.
5. Berechnung der Parität jeden Blockes
	- Alle Paritäten sind null: Es ist kein 1-Bit Fehler aufgetreten
	- Von null verschiedene Paritäten: Es ist ein 1-Bit Fehler aufgetreten.
6. Behebung des $1$-Bit Fehlers. Da jedes [[Paritätsbit]] nur in einem Block vorkommt, kann $k_j$ dem Wert des Blockes mit Blockgröße $2^j$ zugewiesen. Diese $k$ kodieren die Position des Fehlers. Die Fehlerposition lautet: $k_nk_{n-1}...k_2k_1$. Folgende Graphik veranschaulicht die Codierung der Fehlerposition:
	![[Pasted image 20220429200352.png]]
### Beispiel
![[Pasted image 20220429200604.png]]
![[Pasted image 20220429200637.png]]
^1651256948918

## $1$-Bit Fehlerkorrektur und $2$-Bit Fehlererkennung #card 
### Idee
Um 1-Bitfehler von 2-Bitfehlern unterscheiden zu können, fügt man dem Hammingcode ein weiteres [[Paritätsbit]] an der nullten Stelle hinzu. Dieses bezieht sich auf alle anderen Indizes.
![[Pasted image 20220429202619.png]]
### Beispiel
![[Pasted image 20220429202655.png]]
^1651256948925
