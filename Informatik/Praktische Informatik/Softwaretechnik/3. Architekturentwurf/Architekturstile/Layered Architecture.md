---
aliases: [Schichtenmodell]
---

# Layered Architecture #card
## Definition Layer
- Eine Schicht (engl. layer, tier) ist ein Subsystem, welches Dienste für andere Schichten zur Verfügung stellt, mit folgenden Einschränkungen:
	- Eine Schicht nutzt nur Dienste von niedrigeren Schichten
	- Eine Schicht nutzt keine höheren Schichten
- Eine Schicht kann horizontal in mehrere, unabhängige Subsysteme, auch Partitionen genannt, aufgeteilt werden
	- Partitionen bieten Dienste für andere Partitionen der gleichen Schicht an
## Definition Layered Architecture
- Eine Layered Architecture ist die Gliederung einer Softwarearchitektur in hierarchisch geordnete Schichten.
- Eine Schicht besteht aus einer Menge von Software-Komponenten (Module, Klassen, Objekte, Pakete) mit einer wohldefinierten Schnittstelle, nutzt die darunter liegenden Schichten und stellt seine Dienste darüber liegenden Schichten zur Verfügung.
- Zwischen den einzelnen Schichten ist die Benutztrelation linear, baumartig, oder ein azyklischer Graph. Innerhalb einer Schicht ist die Benutztrelation beliebig.
## Besondere Varianten 
### Opaque Layered Architecture
- Bei einer intransparenten Schichtenarchitektur werden undurchlässige Schichten (engl. opaque layers) verwendet
- Eine Schicht in einer solchen Architektur kann nur auf Dienste der Schicht direkt unter ihr zugreifen
![[Pasted image 20220622114411.png]]
### Transparent Layered Architecture
- Bei einer transparenten Schichtenarchitektur werden durchlässige Schichten (engl. transparent layers) verwendet
- Eine Schicht in einer solchen Architektur kann auf Dienste jeder Schicht unter ihr zugreifen.
![[Pasted image 20220622114450.png]]
### 3 Layered Architecture
Ein Architekturstil, bei welchem die Anwendung aus 3 hierarchisch geordneten Subsystemen besteht Oftmals: Eine Benutzerschnittstelle, Anwendungskern und einem Datenbanksystem.
### 3 Tier Architecture
Eine 3-Schichten-Architektur, bei welcher die Schichten auf unterschiedlichen Rechnern laufen.
Beispiel: Benutzerschicht läuft auf einem Klienten, Anwendungskern und Datenbank auf einem Dienstgeber
![[Pasted image 20220622120223.png]]
## Vorteile
- Übersichtliche Strukturierung in Abstraktionsebenen oder virtuelle Maschinen (die Schichten stellen abstrakte Maschinen dar)
- Keine zu starke Einschränkung des Entwerfenden, da er neben einer strengen Hierarchie noch eine liberale Strukturierungsmöglichkeit innerhalb der Schichten besitzt
- Es werden die Wiederverwendbarkeit, die Änderbarkeit, die Wartbarkeit, die Portabilität und die Testbarkeit unterstützt (Schichten können ausgetauscht, hinzugefügt, portiert, verbessert und wieder verwendet werden; Testen von unten oder von oben her).
## Nachteile / Probleme
- Bei intransparenter Schichtung kann es Effizienzverluste geben, da Aufrufe, die mehrere Schichten überschreiten, durch mehrere Schichten weitergereicht werden müssen, und mehrfache Parameterübergabe und Ergebnisrückgabe erfordern.
	- Dies gilt auch für Fehlermeldungen (mit catch/throw aber kein Problem mehr)
- Eindeutig voneinander abgrenzbare Abstraktionsschichten lassen sich nicht immer definieren.
- Innerhalb einer Schicht darf kein Chaos herrschen!
## Beispiele
![[Pasted image 20220622113930.png]]
![[Pasted image 20220622113943.png]]
![[Pasted image 20220622120257.png]]
^c-rt4S77Xlrr
---
**Tags**: 