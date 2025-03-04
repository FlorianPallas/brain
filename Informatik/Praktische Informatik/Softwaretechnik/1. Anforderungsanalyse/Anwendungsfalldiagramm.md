---
aliases: [Use Case Diagramm]
---

# Anwendungsfalldiagramm #card
## Nutzen
- Zeigt die Kommunikationsbeziehung zwischen Akteuren und [[Use Cases|Anwendungsfall]].
- Zeigt die Beziehung zwischen [[Use Cases|Anwendungsfällen]].
- -> Modellierung der Struktur und des Verhaltens von Software und anderen Systemen
## Bestandteile
### Akteur
- Objekt der Systemumgebung, das mit dem System interagiert (und einen oder mehrere Anwendungsfälle auslösen kann).
- Akteure sind i.a. selbst nicht Bestandteile des Systems.
- Akteure können Personen (System-Nutzer), externe Geräte oder mit dem System verbundene Nachbarsysteme sein.
- Akteure tauschen mit dem System Nachrichten aus und können als Sender und/oder Empfänger von Nachrichten auftreten.
- Oft müssen Daten über sie jedoch (z.B. zur Regelung der Zugangsberechtigung) verwaltet werden.
### [[Use Cases|Anwendungsfälle]]
### Beziehungen zwischen [[Use Cases|Anwendungsfällen]]
![[Pasted image 20220504100154.png]]
### Generalisierung
- Anwendungsfälle als auch Akteure können generalisiert werden.
### Include-Beziehung
- Anwendungsfall A beinhaltet den Anwendungsfall B.
- Anwendungsfall B wird benötigt und ist somit nicht optional. 
- Keine explizite Reihenfolge, muss aber enthalten sein. 
### Extend-Beziehung
- Use Case B (Get Help On Registration) erweitert Use Case A (Registration).
- Use Case A ist komplett und Use Case B ist optional.
- Kann einen oder mehrere Einstiegspunkte besitzen.
- Kann optionale Bedingungen haben.
## Extension Points
![[Pasted image 20220730155251.png]]
## Beispiele
![[Pasted image 20220504094922.png]]
![[Pasted image 20220504094902.png]]
^c-CW3trb5V5N

---
**Tags**: