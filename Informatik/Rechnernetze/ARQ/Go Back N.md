Komplexeres [[ARQ]] Verfahren.

## Verfahren
- Sender
	- Kann bis zu $n$ Pakete senden bevor er eine [[Quittungen|Quittung]] erhalten muss
	- Anzahl nicht quittierter Pakete durch Sendefenster begrenzt
- Empfänger
	- Nutzt kumulative [[Quittungen]]

- Pakete sind mit [[Sequenznummern]] nummeriert
- Wird ein Paket nicht quittiert, wird es nach Ablauf eines [[Timer|Timers]] erneut gesendet
- Korrekt übertragene, aber in falscher Reihenfolge erhaltene Pakete werden trotzdem verworfen (kein Puffer)

## Auslastung
Abhängig von der Größe des Sendefensters $W$. Annahme: Fehlerfrei Übertragung.

![[Pasted image 20230731163911.png]]

Mit Fehlerwahrscheinlichkeit $p$:
![[Pasted image 20230731164054.png]]

![[Pasted image 20230731164028.png]]
## Szenarien
![[Pasted image 20230731163747.png]]
![[Pasted image 20230731163758.png]]