Sehr einfaches [[ARQ]] Verfahren

## Verfahren
- Sender sendet Paket
- Sender wartet auf [[Quittung]] des Pakets
- Sender sendet nächstes Paket

- Empfänger Quittiert jedes Paket einzeln
- Falls keine Quittung erhalten wird, wird das Paket nach Ablauf des [[Timer|Timers]] erneut geschickt.

- Um zu verhindern dass der Empfänger ein Paket doppelt erhält werden 1-Bit [[Sequenznummern]] verwendet.
- Somit können Paket nun unterschieden werden

![[Pasted image 20230731160837.png]]

## Auslastung
Fehlerfreie Übertragung:
![[Pasted image 20230731162826.png]]
Mit Fehlerwahrscheinlichkeit $p$:
![[Pasted image 20230731164230.png]]

## Szenarien
![[Pasted image 20230731160632.png]]

## Verwendung
- [[WLAN]]