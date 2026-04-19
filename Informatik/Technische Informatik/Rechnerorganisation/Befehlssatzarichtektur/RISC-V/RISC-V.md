## Definition

Nicht patentierte RISC Prozessorarchitektur

## Datenspeicherung

- Byte (b): immer 8-Bit
- Half-Word (h): in RISC-V (wie meistens) 16-Bit
- Word (w): in RISC-V (wie meistens) 32-Bit

Eine Speicherzelle besitzt 32 Bit. Diese sind in vier Byteblöcken in [[Little-Endian]] abgespeichert.

## Befehlsformat

![[CleanShot 2022-11-23 at 18.24.22@2x.png]]
![[CleanShot 2022-11-23 at 18.24.48@2x.png]]

## Pseudobefehle

- Erweiterung des Befehlssatzes, ohne dass sich die Komplexität des CPU-Designs erhöht
- Werden nicht (direkt) auf einen Maschinenbefehl abgebildet, sondern durch einen oder mehrere native Befehle ersetzt
  Anwendungsfälle:
- Anbieten häufig verwendeter Spezialfälle zur Vereinfachung der Programmierung (z.B. neg )
- Ausgleich von Beschränkungen des Befehlssatzes (z.B. li )

## Einige Befehle

![[CleanShot 2022-11-23 at 18.27.39@2x.png]]

## Assemblerdirektiven

![[CleanShot 2022-11-23 at 18.28.13@2x.png]]

## Systemaufrufe

- Werden in RISC-V mit dem Befehl ecall ausgelöst
- Erlauben die Nutzung von vorgegebenen Betriebssystemfunktionen Details: Vorlesung Betriebssysteme
  Aufrufkonvention:
- Nummer des gewünschten Systemaufrufs muss vorher in das Register $\$ a 7$ geschrieben werden
- Übergabe von Parametern und Rückgabewerten ebenfalls über Register
