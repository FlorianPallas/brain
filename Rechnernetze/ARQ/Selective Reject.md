Adaption des [[Selective Repeat]] [[ARQ]] Verfahrens, **zusätzlich** zu positiven selektiver [[Quittungen]] hier auch negative selektive Quittungen verwendet werden.

## Verfahren
Bis auf Quittierungsverhalten gleich zu Selective Repeat
- Bei fehlerhaften Paket wird zusätzlich eine negative Quittung für diese Paket gesendet
- Der Sender kann bei erhalt einer negativer Quittung das Paket auch ohne Timeout direkt erneut senden

## Auslastung
Mit Fehlerwahrscheinlichkeit $p$
![[Pasted image 20230731165119.png]]
![[Pasted image 20230731165149.png]]

## Szenarien
![[Pasted image 20230731165140.png]]