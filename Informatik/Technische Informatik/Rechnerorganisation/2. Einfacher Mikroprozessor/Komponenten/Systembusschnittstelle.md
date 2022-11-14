## Definition #card 
- Anbindung des Prozessors an den Bus (Adressbus, Datenbus, Steuerbus)
- Steuerung der Aktionen auf dem Bus
^c-F2ikvZ6KiP

## Aufbau #card 
![[CleanShot 2022-11-14 at 16.49.51@2x.png]]
Enthält diverse Register (Puffer) zur kurzfristigen Speicherung von Adressen und Daten, z.B.
- Befehlszähler: Adresse des nächsten zu holenden / auszuführenden Befehls (Instruction Pointer, Program Counter)
- Adressbuspuffer: Adresse des zu ladenden oder zu speichernden Datums im Hauptspeicher
- Datenbuspuffer: puffert den zu speichernden oder zu ladenden Wert
+ Enthält Aus- und Eingangstreiber (Tristate-Treiber)
^c-1CTGhksxqe