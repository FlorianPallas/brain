---
aliases: []
---

# Abbilden von [[Klassendiagramm|Klassendiagrammen]] #card
## Klassen
Bei OO-Sprachen wird jede UML-Klasse auf eine Klasse in der Programmiersprache abgebildet (einschließlich Attributen und Methoden).
## Assoziationen
OO-Sprachen bieten per se keine Assoziationen, nur Referenzen. Letztere benutzt man, um die verschiedenen Arten von Assoziationen (uni-/bidirektional, Kardinalitäten) zu implementieren.
### Unidirektionale Eins-zu-Eins-Assoziation
Benutze in der Klasse, in der zur anderen navigiert wird, eine Instanzvariable, die eine Referenz zur anderen Klasse enthält.
### Bidirektionale Eins-zu-Eins-Assoziation
Benutze in beiden Klassen eine Instanzvariable, die eine Referenz zur anderen enthält.
Achtung: Echte 1:1-Beziehung bedeutet gegenseitige Abhängigkeit!
### 1:N-Assoziation
Vielfache Referenzen müssen durch mengenwertige Instanzvariablen (z.B. eine TreeSet in Java) ausgedrückt werden.
### M:N-Assoziation
Bei N:M-Assoziationen müssen zwei mengenwertige Attribute verwendet werden.
![[Pasted image 20220622165056.png]]
### Sonderfälle
![[Pasted image 20220622165217.png]]
^c-lG4HIpdpnw
---
**Tags**: 