Das Alternating Bit Protocol bietet einen [[Zuverlässiger Dienst|zuverlässigen Dienst]] auf Basis von [[Stop and Wait]] an.

## Fazit
Da immer gewartet werden muss bietet ABP eine sehr geringe Leistungsfähigkeit wenn die Distanz zwischen Sender und Empfänger groß ist.

## Paket
![[Pasted image 20230731161103.png]]

## Ablauf
### Sender
- [[Sequenznummern|Sequenznummer]] abwechselnd 0 oder 1
- Wartet auf [[Quittungen|Quittung]] für zuletzt gesendetes Paket
- Zeitüberschreitung -> Sendewiederholung

### Empfänger
- Quittiert korrekte Pakete anhand von Sequenznummer
	- Duplikate (wenn eine Quittung verloren ging) werden erkannt
- Verwirft Pakete mit ungültigem [[CRC]]

