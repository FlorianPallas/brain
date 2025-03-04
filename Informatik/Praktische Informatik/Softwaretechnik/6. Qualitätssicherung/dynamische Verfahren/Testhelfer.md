---
aliases: []
---

# Testhelfer #card
## Motivation
- Objekte leben nicht isoliert, Objekte arbeiten in einer Anwendung zusammen.
- Zusammenarbeit resultiert in Abhängigkeiten beim Testen. Wie können einzelne Eigenschaften getestet werden im Hinblick auf diese Abhängigkeiten?
## Definition
Wenn Klassen voneinander abhängen, können noch nicht implementierte Klassen durch Testhelfer (Stummel, Attrappe oder Nachahmung) ersetzt werden.
- Stummel oder Attrappen vertreten die noch fehlende Implementierungen.
- Stummel und Attrappen werden sukzessive durch echte Implementierungen ersetzt; Nachahmungen sind für zukünftiges Testen auch weiterhin nützlich.
^c-0pv81TWjUN
---
**Tags**: 