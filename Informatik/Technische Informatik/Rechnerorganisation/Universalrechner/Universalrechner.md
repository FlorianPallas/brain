---
aliases: [Prozessor, Steuerwerk, Rechenwerk, Hauptspeicher, Ein-/Ausgabesystem, Adressleitung, Steuerleitung, Datenleitung]
---

## Modell #card
![[Pasted image 20221104132712.png]]
^c-GPyTXhviCF

## Komponenten
### Prozessor #card
- Verarbeitet Daten gemäß eines Programms
- Besteht aus Steuerwerk und Rechenwerk
^c-ztbwGH080u

### Steuerwerk #card
- Holt die Befehlt eines Programms aus dem Speicher
- Dekodiert die Befehle
- Steuert ihre Ausführung in der verlangten Reihenfolge mittels Steuer- und Status-Signalen

![[Pasted image 20221104134231.png]]
^c-ZJyrMw8mqC

### Rechenwerk #card
- Führt Rechenoperationen aus
- Steuersignale bestimmen die Art von Operation
- Liefert Statussignale an das Steuerwerk zurück (z.B. Zahl ist positiv, Zahl ist 0 - Erlaubt effiziente Abfragen)
^c-JT3Onyo7tB

### Hauptspeicher #card
- Besteht aus adressierbaren Speicherzellen
- von-Neumann-Konzept: Daten und Programm auf dem Hauptspeicher
- Harvard-Architektur (heutiger Standard): getrennter Programm- und Datenspeicher
^c-ZERhdOyPnl

### Ein-/Ausgabesystem #card 
- Schnittstellen zur Anbindung peripherer Geräte (z.B. Drucker, Bildschirm)
^c-nWOBMhLRFZ

### Verbindungen
Sogenannte Busse verbinden Komponenten des Rechners.
- Adressleitungen: Addressübertragung
- Datenleitungen: Daten- / Befehlsübertragung (von/zum Prozessor)
- Steuerleitungen: Steuer- / Statussignalübertragung zum Prozessor

---
**Related:**
**Tags**: 