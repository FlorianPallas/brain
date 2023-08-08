Schnittstelle für verteilte Anwendungen zur Transportschicht

- Von Anwendung erstellt, genutzt und freigegeben
- Adressierung über Port nummern
- Lesen und Schreiben wie Datei
- Können auch Puffern

![[Pasted image 20230808144907.png]]

## Beispiel TCP
- Server nutzt zwei Sockets
	- Welcome Socket
		- Immer aktive
		- Zum Verbindungsaufbau genutzt
	- Connection Socket
		- Wird beim Verbindungsaufbau erstellt

![[Pasted image 20230808145144.png]]