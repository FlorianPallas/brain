Signale können verschieden codiert werden um später übertragen zu werden.

## Kriterien
![[Pasted image 20230807190704.png]]

## Non-Return to Zero (NRZ)
- 1 hoher Pegel über ganzes Bitintervall +1
- 0 niedriger Pegel über ganzes Bitintervall -1
- Taktrückgewinnung: schlecht, schwierig bei langen 1 oder 0 Folgen
- Baudrate: gut
- Gleichstromanteil: schlecht, RDS kann gegen unendlich gehen
- Komplexität: einfach

![[Pasted image 20230807191038.png]]

## Manchester Code
- Biphasen Code: Symbolwerte durch Signalwechsel
- Wechsel in Intervallmitte. Erste Hälfte momentanes Signal.
- Immer Wechseln
- Taktrückgewinnung: gut, aufgrund der Signalwechsel
- Baudrate: schlecht, viele Wechsel für wenig Daten
- Komplexität: einfach, über XNOR erzeugbar

![[Pasted image 20230807191315.png]]

## Alternate Mark Inversion (AMI)
- Ternärer Code: Symbolwerte werden auf 0,+,- abgebilted
- 1 durch abwechselnden hohen und negativen Pegel über das gesamte Intervall
- 0 durch Nullpegel
- Signalerkennung: Absoluter Wert im Intervall
- Taktrückgewinnung: nur gut bei langen 1 Folgen, bei langen 0 Folgen schwierig
- Gleichstromfreiheit: gut
- Baudrate: gut

![[Pasted image 20230807191604.png]]

