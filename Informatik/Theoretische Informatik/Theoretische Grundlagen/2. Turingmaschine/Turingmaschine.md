## Definition

![[CleanShot 2022-11-15 at 13.23.52@2x.png]]

## Konventionen

![[CleanShot 2022-11-15 at 13.24.33@2x.png]]

## Konfiguration

![[CleanShot 2022-11-22 at 17.56.03@2x.png]]

## Definition: Akzeptanz einer Sprache

Sie akzeptiert eine Sprache L genau dann, wenn sie ausschließlich Wörter $w \in L$ als Eingabe akzeptiert (in einem akzeptierenden Zustand stoppt).

## Definition: Semi-Entscheidbarkeit

Eine Sprache $L \subseteq \Sigma^*$ heißt rekursiv-aufzählbar oder semi-entscheidbar, wenn es eine Turing-Maschine gibt, die genau die Eingaben $w$ akzeptiert für die $w \in L$.
Das Verhalten der Turing-Maschine für Eingaben $w \notin L$ ist damit nicht genau definiert. D.h., die Turing-Maschine stoppt entweder nicht in einem Endzustand oder aber stoppt gar nicht.

## Definition: Entscheidbarkeit einer Sprache

Eine Sprache $L \subseteq \Sigma^*$ heißt rekursiv oder entscheidbar, wenn es eine Turing-Maschine gibt, die auf **allen Eingaben stoppt** und eine Eingabe $w$ genau dann akzeptiert, wenn $w \in L$ gilt.
Wichtig: Dies ist ein echt stärkeres Kriterium als die Akzeptanz/Semi-Entscheidbar einer Sprache.

## Beispiel: Akzeptiert $0^n1^n$

![[CleanShot 2022-11-22 at 17.56.26@2x.png]]

## Berechnen einer Funktion

![[CleanShot 2022-11-22 at 17.59.11@2x.png]]

## Beispiel: Turingmaschine die Binärzahl um eins erhöht

![[CleanShot 2022-11-22 at 18.01.02@2x.png]]

## Church'sche These

Die Menge der (Turing-)berechenbaren Funktionen ist genau die Menge der im intuitiven Sinne überhaupt berechenbaren Funktionen.
Diese These wird allgemein akzeptiert. Jegliche Versuche ein mächtigeres Model aufzustellen sind bislang gescheitert.

## Mächtigkeit

Eine Turingmaschine mit $k$ Köpfen und $b$ Bändern ist immer noch gleichmächtig wie eine Turingmaschine mit nur einem Lesekopf und einem Band
![[CleanShot 2022-12-01 at 08.58.04@2x.png]]
![[CleanShot 2022-12-01 at 08.58.23@2x.png]]

## Zeitkomplexität

![[CleanShot 2022-11-29 at 10.04.35@2x.png]]
