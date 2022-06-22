---
aliases: []
---

# Client-Server #card
## Definition
- Ein oder mehrere Server bieten Dienste für andere Subsysteme, Clients genannt, an.
- Jeder Client ruft eine Funktion des Servers auf, welcher den gewünschten Dienst ausführt und das Ergebnis zurückliefert. Dazu muss der Client die Schnittstelle des Servers kennen. Umgekehrt muss der Server die Schnittstelle des Clients nicht kennen.
![[Pasted image 20220622115732.png]]
## Funktionsweise
### Client
- Eingaben des Benutzers entgegennehmen
- Vorverarbeitung der Eingaben
### Server
- Datenverwaltung
- Datenintegrität und -Konsistenz
- Sicherheit
### Einsatz
Wird oft beim Entwurf von Datenbank-Systemen verwendet:
- Front-End: Benutzeroberfläche für den Benutzer (Client)
- Back-End: Datenbankzugriff und Manipulation (Server)
Client und Server laufen i.d.R. auf unterschiedlichen Rechnern, aber nicht unbedingt.
## Beispiel
![[Pasted image 20220622115819.png]]
^c-wq3cjKKdt6
---
**Tags**: 