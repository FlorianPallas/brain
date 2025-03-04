---
aliases: []
---

# Pipeline #card
## Definition
![[Pasted image 20220622121340.png]]
- Jede Stufe oder Filter ist ein eigenständig ablaufender Prozess oder Faden, mit eigenem Befehlszähler
- Daten fließen durch das Fließband, wobei jede Stufe von der vorigen Daten empfängt, sie verarbeitet, und an die nächste weiterreicht.
- Aufeinanderfolgende Stufen sind mit einem größenbeschränkten Puffer verbunden, um Geschwindigkeitsschwankungen auszugleichen.
## Ziel
In einem System durchlaufen Datenströme verschiedene Bearbeitungsstufen.
- Der Datenfluß soll leicht änderbar sein.
- Bearbeitungsstufen sollen austauschbar, erweiterbar und wiederverwendbar sein.
## Stil
Beschreibung von Bearbeitungsstufen durch Filters und Datenströme durch Pipes.
- Filter-Komponenten haben Ein/Ausgänge und bearbeiten einen Datenstrom.
- Pipes: Datenstrom von einem Filter-Ausgang zu einem Filter-Eingang.
- Filter bearbeiten Eingangsdaten kontinuierlich.
## Beispiele
### Rechnungsverarbeitungssystem
![[Pasted image 20220622121546.png]]
### Unix-Shell
![[Pasted image 20220622121655.png]]
^c-wGzVz5yjUp
---
**Tags**: 