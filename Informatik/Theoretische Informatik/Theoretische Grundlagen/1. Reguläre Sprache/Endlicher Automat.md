## Definition deterministischer EA

![[CleanShot 2022-10-31 at 10.06.01@2x.png]]

## Zweck

Ein endlicher Automat erkennt oder akzeptiert eine Sprache $L$, d.h. eine Menge von Wörtern über dem Alphabet $\Sigma$ des Automaten, wenn er nach Abarbeitung eines Wortes $w$ genau dann in einem Endzustand ist, wenn das Wort $w$ in der Sprache $L$ ist $(w \in L)$

## Beispiel deterministischer EA

![[CleanShot 2022-10-31 at 10.08.39@2x.png]]

## Definition nichtdeterministischer EA

![[CleanShot 2022-11-03 at 17.10.56@2x.png]]
![[CleanShot 2022-11-03 at 17.11.23@2x.png]]

## Beispiel nichtdeterministischer EA

![[CleanShot 2022-11-03 at 17.12.08@2x.png]]

## Beziehung zwischen NEA und DEA

Jeder DEA ist automatisch auch ein NEA und jeder NEA kann mittels [[Endlicher Automat#Potenzmengenkonstruktion card|Potenzmengenkonstruktion]] in einen DEA überführt werden. Also gilt:
$\text{DEA} \Leftrightarrow \text{NEA}$

## Potenzmengenkonstruktion

![[CleanShot 2022-11-03 at 17.17.06@2x.png]]

## Entfernen von $\epsilon$-Übergängen

![[CleanShot 2022-11-03 at 17.28.25@2x.png]]
