---
cards-deck: Technische Informatik
---

# Horner Schema #card 
## Funktionsweise
Der ganzzahlige und gebrochene Anteil der Zahl wird getrennt betrachtet.
### Ganzzahl Anteil
Eine ganze Zahl $X_{b}$ kann auch in der Form
$$
X_{b}=\left(\left(\ldots\left(\left(y_{n} b+y_{n-1}\right) b+y_{n-2}\right) b+\cdots+y_{2}\right) b+y_{1}\right) b+y_{0}
$$
geschrieben werden, wobei die $y_{i}$ ganzzahlig sind. Die gegebene Dezimalzahl wird nun sukzessive durch die Basis $b$ dividiert. Die jeweiligen ganzzahligen Reste ergeben die Ziffern $y_{i}$ der Zahl $X_{b}$ in der Reihenfolge von der niedrigstwertigen zur höchstwertigen Stelle.
#### Beispiel
Umwandlung von $31562_{10}$ ins Hexadezimalsystem:
![[Pasted image 20220424180443.png]]
### Gebrochener Anteil
Die Umwandlung des Nachkommateils gebrochener Zahlen geschieht in ähnlicher Weise, denn er kann in der Form
$$
Y_{b}=\left(\left(\ldots\left(\left(y_{-m} b^{-1}+y_{-m+1}\right) b^{-1}+y_{-m+2}\right) b^{-1}+\ldots y_{-2}\right) b^{-1}+y_{-1}\right) b^{-1}
$$
dargestellt werden. Eine sukzessive Multiplikation des Nachkommateils der Dezimalzahl mit der Basis $b$ des Zielsystems ergibt nacheinander die $y_{-i}$.
#### Beispiel
Umwandlung von $31562_{10}$ ins Hexadezimalsystem:
![[Pasted image 20220424180632.png]]
^c-lH11muSVZN
