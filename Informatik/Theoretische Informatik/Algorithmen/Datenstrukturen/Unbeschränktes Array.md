---
aliases: [unbeschränktes Array]
---

# Unbeschränktes Array #card
![[Pasted image 20220504172643.png]]
## Anmerkungen
- Die [[Landau Notation|Laufzeit]] ist [[Amortisierte Laufzeit|amortisiert]] konstant.
	- im Worst Case benötigt eine einzelne Operation $\Theta(n)$ Zeit ( $n=$ Arraygröße)
	- aber: im Schnitt benötigt jede Operation nur $\Theta(1)$ Zeit
- Es wird höchstens doppelt so viel Speicher alloziert als gebraucht wird.
- Laufzeittechnisch ist es egal mit welchem Faktor größer 1 die Kapazität erhöht, da sich dieser in der obigen Summe rauskürzt. Es ist aber Konvention, dass die Zahl 2 für den Faktor gewählt wird
^c-VDr5vUnFkH
---
**Tags**: 