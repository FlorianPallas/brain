---
aliases: []
---

# Umwandeln des Hauptraums in ein Jordanblock #card
## Idee
Vereinfache den [[Hauptraum]] soweit, dass bis auf die Diagonale und eine Nebendiagonale nur nullen in der Abbildungsmatrix stehen.
## Ziel
Für jeden [[Hauptraum]] eine [[Basis]] $B$ zu bestimmen, sodass die [[Darstellungsmatrix]] $D_{B B}\left(\left.f\right|_{H_{\lambda}}\right)$ folgende Gestalt besitzt (die Jordankästchen werden der Größe nach angeordnet):
![[Pasted image 20220510095329.png]]
## Eigenschaften
- Die [[Dimension]] des [[Eigenraum]] von $\lambda$ gibt die Anzahl an Jordankästchen an.
## Allgemeines Verfahren
1. Wie bei der Berechnung des [[Hauptraum|Hauptraums]] müssen die Kerne $K_1=E_1, \quad K_2, \quad ... \quad$ sukzessive zu bestimmen, bis $K_{q+1}=K_q$ erfüllt ist. Dabei gilt, dass $q$ gleich der algebraischen Vielfachheit des [[Eigenwerte|Eigenwertes]] ist.
2. Nun wird der [[Hauptvektor]] $v_s$ mit höchster [[Stufe eines Vektors|Stufe]] genommen (also ein Vektor, der in $K_q$ und nicht in $K_{q-1}$ liegt). Mit diesem erzeugt man sich dann jeweils ein Vektor jeder niedrigeren Stufe:  
	1. $v_{s-1}=(A-\lambda)v_s$
	2. $v_{s-2}=(A-\lambda)^2v_s =(A-\lambda)v_{s-1}$
	3. $v_{s-3}=(A-\lambda)^3v_s =(A-\lambda)v_{s-2}$
	4. ...
	5. $v_1 =(A-\lambda)^{s-1}v_s =(A-\lambda)v_{2}$
	Diese Vektoren erzeugen dann eine Basis $B_q$ des größten Jordankästchens mit $B_q=(v_1, ..., v_s)$. Die Anzahl der Basisvektoren bestimmt die Länge des Jordankästchens.
3. Der 2. Schritt wird solange mit den noch nicht verwendeten [[Hauptvektor|Hauptvektoren]] wiederholt, bis es keine mehr gibt. Jede Ausführung des 2. Schritts erzeugt einen Jordanblock, der jeweils kleiner gleich dem vorherigen ist.
4. Zusammenfassen der im 2. Schritt ermittelten Basen zu einer. Dabei stehen die früher ermittelten Basen links von den später ermittelten.
^c-TSDBam4Vrb
---
**Tags**: 