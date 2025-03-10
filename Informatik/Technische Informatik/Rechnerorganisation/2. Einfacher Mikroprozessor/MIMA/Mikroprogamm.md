## Definition

Grundlegende [[Maschinenbefehl|Maschinenbefehle]] (wie z.B. `ADD`) können über Hardware aber auch mittels Mikroprogrammen implementiert werden. Diese Mikroprogramme verschieben dabei nur Daten zwischen [[Rehister|Registern]].

## Beispiele

### `LDV <a>`

- Schreibt die zu lesende Adresse ins [[SAR]]
- Setzt `R = 1` um zu lesen
- Wartet 3 Takte für den Speicher
- Verschiebt die gelesenen Daten in den Akku
  ![[Pasted image 20221111123417.png]]

### `JMP`

- Schreibt die nächste Adresse in das [[IAR]]
- In der nächsten [[Holphase]] wird das Programm an der gegebenen Adresse fortgefahren
  ![[Pasted image 20221111123808.png]]

---

**Related:**
**Tags**:
