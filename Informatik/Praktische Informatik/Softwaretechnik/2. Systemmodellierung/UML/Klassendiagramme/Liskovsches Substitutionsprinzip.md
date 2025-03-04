---
aliases: []
---

# Liskovsches Substitutionsprinzip #card
## Definition
In einem Programm, in dem U eine Unterklasse von $\mathrm{O}$ ist, kann jedes Exemplar der Klasse $\mathrm{O}$ durch ein Exemplar von U ersetzt werden, wobei das Programm weiterhin korrekt funktioniert.
## Eigenschaften
- Alle Eigenschaften der Oberklasse müssen in der Unterklasse vorhanden sein.
- Die Unterklasse hat die gleichen oder schwächere Vorbedingungen.
- Die Unterklasse bietet die gleichen oder stärkere Nachbedingungen.
## Folgerungen
- Vererbte Eigenschaften stehen in der Unterklasse zu Verfügung, wie sie in der Oberklasse definiert sind.
- Die Unterklasse darf noch zusätzliche Eigenschaften definieren, die sie spezieller machen.
- Die Unterklasse kann keine Eigenschaften der Oberklasse weglassen.
	- Wäre dies nötig, handelt es sich nicht um eine Vererbungsbeziehung.
	- Substitution der Oberklasse durch die Unterklasse wäre nicht möglich.
- Die Unterklasse kann gleiche oder schwächere Vorbedingungen als die Oberklasse haben (Kontravarianz - Verwendung einer Verallgemeinerung des Parametertyps in der überschreibenden Methode)
- Die Unterklasse kann gleiche oder stärkere Nachbedingungen als die Oberklasse haben (Kovarianz - Verwendung einer Verallgemeinerung des Parametertypes in der überschreibenden Methode)
^c-TduyuOoZQR
---
**Tags**: 