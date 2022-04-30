---
cards-deck: Technische Informatik
---

# Euklidischer Algorithmus #card 
## Funktionsweise
- Ziffern werden sukzessive, beginnend mit der höchstwertigen Ziffer, berechnet
- 1. Schritt: Berechne $p$ gemäß der Ungleichung
$$
b^{p} \leq X_{10}<b^{p+1} \quad \text { setze } i=p, D_{i}=X_{10}
$$
- 2. Schritt: Ermittle $y_{i}$ und den Rest $R_{i}$ durch Division von $D_{i}$ durch $b^{i}$
$$
y_{i}=\frac{D_{i}}{b^{i}} \quad R_{i}=D_{i} \bmod b^{i}
$$
- 3. Schritt: Wiederhole 2. Schritt für $i=p-1, \ldots$ und setze $D_{i}=R_{i+1}$ bis $R_{i}=0$ oder bis $b^{i}$ (und damit der Umrechnungsfehler) gering genug ist
## Beispiel
Tipp: Statt $16^x$ zu berechnen, berechne $2^{4 \cdot x}$, da $2$-er Potenzen geläufiger sind. 
![[Pasted image 20220424162044.png]]
^c-x6ZBrZpVRF
