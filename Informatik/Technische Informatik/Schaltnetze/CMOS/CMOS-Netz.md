---
aliases: []
---

# CMOS-Netz #card
## Funktionsweise
Im Allgemeinen wird eine n-stellige Boolesche Funktion in CMOS mit zwei Teilnetzen, einem n-Netz und einem p-Netz, realisiert. 
## n-Netz
- Besteht aus [[nMOS-Transistor|nMOS-Transistoren]] 
- Schaltet genau einen Pfad von GND nach y durch, wenn der Funktionswert für die Eingangsbelegung gleich 0 ist
## p-Netz
- Besteht aus [[pMOS-Transitior|pMOS-Transistoren]] 
- Schaltet genau einen Pfad von $V_{dd}$ nach y durch, wenn der Funktionswert für die Eingangsbelegung gleich 1 ist
## Hinweis
- Komplexere Funktionen werden als [[Konjunktive Normalform|KNF]] oder [[Disjunktive Normalform|DNF]] mit den folgenden Gattern realisiert: [[CMOS-Inverter]], [[CMOS-NAND]], [[CMOS-NOR]]
^c-0cnl5W3Kyg
---
**Tags**: 