---
aliases: []
---

# Singleton #card
## Zweck
Sichere zu, dass eine Klasse genau ein Exemplar besitzt, und stelle einen globalen Zugriffspunkt darauf bereit.
## Motivation
Die Klasse ist selbst für die Verwaltung ihres einzigen Exemplars zuständig. Die Klasse kann durch Abfangen von Befehlen zur Erzeugung neuer Objekte sicherstellen, dass kein weiteres Exemplar erzeugt wird.
## Struktur
![[Pasted image 20220621182411.png]]
## Anwendbarkeit
- Wenn es von einer Klasse nur eine einzige Instanz geben darf und diese Instanz den Clients an einer bekannten Stelle zugänglich gemacht werden soll.
- Wenn es schwierig oder unmöglich ist, festzustellen, welcher Teil der Anwendung die erste Instanz erzeugt.
- Wenn die einzige Instanz durch Unterklassenbildung erweiterbar sein soll und die Clients ohne Veränderung ihres Quelltextes diese nutzen sollen.
^c-DH09boDTlF
---
**Tags**: 