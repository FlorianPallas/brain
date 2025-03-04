---
aliases: []
---

# Versionsverwaltung und Kontrolle #card
## Motivation
Versucht Änderungschaos zu vermeiden indem
- Identifikation und (Rück-)Verfolgung von Änderungen und
- Versionsselektion
ermöglicht werden
## Ursprung
US-amerikanische Raumfahrtindustrie in 50 er und 60 er Jahren
$\rightarrow$ Konfigurationsverwaltung sollte alle Änderungen von Raumfahrzeugen dokumentieren, so dass jeder Entwicklungsstand wieder hergestellt werden konnte.
## Definition
Softwarekonfigurationsverwaltung (engl. software configuration management) ist die Disziplin zur Verfolgung und Steuerung der Evolution von Software.
## Check-In / Check-Out
- Software-Elemente werden in Depots (engl. repositories) gesammelt
- Ausbuchen (Check-Out)
	- Holt Kopie aus Depot
	- Reserviert Kopie für den Ausbucher, was heißt, dass nur dieser die nächste Revision ablegen darf (striktes Ausbuchen)
	- Kopie darf geändert und wieder eingebucht werden
- Einbuchen (Check-In)
	- Schreibt Kopie in Depot zurück
	- Löscht Reservierung
	- Hält fest: Autor des Elements/der Änderung, Einbuchungszeitpunkt und Logbucheintrag, der Änderung zusammenfasst
	- Eingebuchtes Element ist nicht mehr änderbar
	- Erst erneutes Ausbuchen erlaubt Änderungen
## Änderungskonflikte vermeiden
### Konfliktvermeidung durch Sperren
![[Pasted image 20220622172916.png]]
#### Probleme
1. Technische Probleme:
	- Technische Sperren vs. Ankündigung auf Mailingliste
	- Vergessen zu entsperren typisch
1. Unnötige Sequentialisierung der Arbeit: Gleichzeitige Änderungen an unterschiedlichen Stellen nicht möglich
2. Falsches Gefühl von Sicherheit: Zwei Nutzer arbeiten getrennt auf den Dokumenten A und B. Was passiert, wenn A von $B$ abhängig ist? A und B passen nicht mehr zusammen. Die Nutzer müssen
### Konfliktlösung durch Merging
Optimistisches Ausbuchen von Dateien und spätere Zusammenführung der Versionen
- Stand der ausgebuchten Version hat sich im Depot evtl. geändert
- Verschmelzen (engl. merging) der Änderungen und ggf. Auflösen von Konflikten nötig
![[Pasted image 20220622173407.png]]
![[Pasted image 20220622173423.png]]
## Verwaltung der Versionen
Vollständiges Abspeichern jeder Versionen ist platzaufwändig.
Alternative
- Vorwärts-Deltas: Speichere Grundversion und die daran durchgeführten Änderungen
- Rückwärts-Deltas: Speichere aktuelle Version und die Änderungen für frühere Versionen
Ein Delta ist der Unterschied zwischen zwei Versionen; ein komprimiertes Änderungs-Skript, das eine Version in die andere überführt. Bei Software ist ein Delta i.d.R. etwa 1-2\% des Umfanges einer (Voll-)Version.
### Vorwärts-Deltas
![[Pasted image 20220622173626.png]]
Vorteil: Schneller Zugriff aus frühere Versionen
Nachteil: Langsamer Zugriff auf aktuellere Versionen
Oftmals wird die Aktuelle Version häufiger benötigt -> Rückwärts-Deltas
### Rückwärts-Delta
![[Pasted image 20220622173739.png]]
^c-phseonz5ht
---
**Tags**: 