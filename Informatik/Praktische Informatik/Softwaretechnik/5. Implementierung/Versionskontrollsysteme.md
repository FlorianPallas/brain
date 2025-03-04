---
aliases: []
---

# Versionskontrollsysteme #card
## Verwendungsgründe
- Parallele Bearbeitung von Software durch mehrere Personen
- Protokollierung durchgeführter Änderungen
- Rücknahme von Änderungen möglich
- Datensicherung des Quelltextes
## Arten
### Lokale Versionsverwaltung
- Lokale Archivierung (meist einzelner) Dateien
- Beispiel: RCS
### Zentrale Versionsverwaltung
- Revisionen liegen auf zentralem Server
- Clients erfragen Updates, senden Änderungen
- Beispiele: CVS, SVN
### Verteilte Versionsverwaltung
- Verteilte Repositories (mit allen bekannten Revisionen) die synchronisiert werden können
- Beispiel: Git
## Systeme
### Revision Control System (RCS) by Tichy
- Verwaltet mehrere Versionen einer Datei
- Automatisiert
	- Aufbewahrung
	- Wiederherstellung
	- Logbuch
	- Automatische Identifikation der Software-Elemente
	- Verschmelzen von Versionen
- Versionierung von Verzeichnissen nicht unterstützt.
- Nicht netzwerkfähig
- Eines der ersten quelloffenen Systeme (1983)
### Concurrent Versions System (CVS)
- Versioniert ganze Verzeichnisbäume
- Ist netzwerkfähig
- Verwendet intern RCS
### Subversion (SVN)
- Weiterentwicklung von CVS
- Internetfähig, d.h. das Depot wird auf einem Dienstgeber abgelegt, auf den Arbeitsplatzrechner über das Internet zugreifen.
- SVN versioniert das gesamte Projektdepot, inklusive dem Verschieben, Umbenennen und Kopieren von Verzeichnissen und Dateien.
- Das Einbuchen von Änderungen geschieht atomar, d.h. eine Änderung wird ganz oder gar nicht in das Projektdepot übertragen.
- Optimistisches Ausbuchen
### Git
- Abstraktion von Dateien; alles ist ein Objekt: Dateiinhalte, Verzeichnisse, Konfigurationen, Varianten
- Umgang mit Varianten ist integraler Bestandteil
- Kryptografische Sicherung der Historie
- Gesamtes Depot ist für jeden Benutzer lokal
- Dafür zusätzlicher Kommunikationsschritt: push/pull/fetch zur Übertragung von Objekten zwischen Depots
- Abbildung von „Befehlshierarchien“ und Arbeitsabläufen (Freigaben von Konfigurationen)
![[Pasted image 20220622184004.png]]
### Vergleich SVN mit Git
![[Pasted image 20220622184059.png]]
![[Pasted image 20220622184520.png]]
## Benutzungsrichtlinien
$\checkmark$ Vor jeder Arbeitsphase ein Update machen
$\checkmark$ Vor jedem Commit ein Update machen, um den aktuellen Projektstand zu erhalten und ggf. Konflikte zu beheben
$\checkmark$ Nur lauffähigen (kompilierbaren) Code commiten
$\checkmark$ Commits müssen gut kommentiert werden
$\checkmark$ Nur Quellcode und Dokumente ablegen
$\checkmark$ i.A. keine systemspezifischen oder generierten Daten ablegen (z.B. absolute Klassenpfade oder .class-Dateien)
^c-Xop9Z2rzoO
---
**Tags**: 