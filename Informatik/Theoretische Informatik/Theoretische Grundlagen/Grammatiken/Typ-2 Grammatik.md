## Definition

![[CleanShot 2023-01-25 at 09.03.17@2x.png]]

## Mächtigkeit

## Laufzeit Wortproblem

Das Wortproblem ist in poly Zeit lösbar (Umwandlung in erweiterte Chomsky-Normalform + CYK Algorithmus)

## Laufzeit Überprüfen auf leere Sprache

![[CleanShot 2023-01-27 at 09.45.08@2x.png]]

## Laufzeit: Überprüfen auf endliche Sprache

![[CleanShot 2023-01-27 at 09.45.55@2x.png]]

## Laufzeit: Nutzlose Variablen

![[CleanShot 2023-01-27 at 09.46.57@2x.png]]

## Rechenregeln

![[CleanShot 2023-01-27 at 09.43.47@2x.png]]
![[CleanShot 2023-01-27 at 09.46.13@2x.png]]

## Syntaxbaum

![[CleanShot 2023-01-25 at 08.58.53@2x.png]]
Zu jeder Ableitung gehört genau ein Syntaxbaum. Zu einem Syntaxbaum können mehrere Ableitungen gehören.
![[CleanShot 2023-01-25 at 08.59.55@2x.png]]

## Eindeutig

![[CleanShot 2023-01-25 at 09.05.43@2x.png]]
![[CleanShot 2023-01-25 at 09.07.30@2x.png]]
![[CleanShot 2023-01-25 at 09.07.41@2x.png]]

## Chomsky Normalform

![[CleanShot 2023-01-25 at 09.10.11@2x.png]]
![[CleanShot 2023-01-25 at 09.10.31@2x.png]]

## Chomsky Normalform Verfahren

### Schritt 1

![[CleanShot 2023-01-25 at 09.28.05@2x.png]]

### Schritt 2

![[CleanShot 2023-01-25 at 09.30.03@2x.png]]

### Schritt 3

![[CleanShot 2023-01-25 at 09.36.35@2x.png]]
![[CleanShot 2023-01-25 at 09.38.24@2x.png]]

### Schritt 4

![[CleanShot 2023-01-25 at 09.57.42@2x.png]]
![[CleanShot 2023-01-25 at 10.07.30@2x.png]]
![[CleanShot 2023-01-25 at 10.08.31@2x.png]]
usw...
![[CleanShot 2023-01-25 at 10.10.50@2x.png]]

### Sonderbehandlung

![[CleanShot 2023-01-25 at 10.05.48@2x.png]]

## CYK-Algorithmus

![[CleanShot 2023-01-25 at 10.11.46@2x.png]]
![[CleanShot 2023-01-27 at 09.37.49@2x.png]]

## Pumping-Lemma

![[CleanShot 2023-01-27 at 09.38.40@2x.png]]
Wie auch bei dem normalen Pumping-Lemma für reguläre Sprachen, kann damit nicht die Regularität bzw. die Kontextfreiheit gezeigt werden, sondern lediglich die Verneinung des Lemmas kann angewandt werden um zu zeigen, dass eine Sprache nicht regulär / kontextfrei ist.

In Kurzfassung:
![[CleanShot 2023-01-27 at 09.42.01@2x.png]]
