Komplexeres [[ARQ]] Verfahren

## Ziel
- Erhöhung der Auslastung zu [[Stop and Wait]]
- Reduzierung des Datenaufkommens von [[Go Back N]]

## Verfahren
- Sender
	- Wie bei Go Back N
- Empfänger
	- Quittiert mit selektiven positive [[Quittungen]]

- Empfänger speichert Pakete in Empfangspuffer und bestätigt sie anstatt sie zu verwerfen wenn sie in falscher Reihenfolge sind
- Sender sendet nur fehlerhafte Pakete erneut

## Szenarien
![[Pasted image 20230731164756.png]]