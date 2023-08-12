
- Zustandslos
- TCP

## Request
![[Pasted image 20230808145345.png]]
![[Pasted image 20230808145433.png]]

## Response
![[Pasted image 20230808145442.png]]
![[Pasted image 20230808145514.png]]

## Persistent HTTP
- Mehrere Object können gesendet werden
- Nach Verbindungsaufbau immer nur 1 RTT pro Objekt
## Non persistent HTTP
- Nur ein Objekt pro Verbindung
- $n$ Objekte -> $2 \cdot n \cdot RTT (+t_s)$ da Verbindung auch eine RTT braucht

![[Pasted image 20230808145816.png]]
![[Pasted image 20230808145739.png]]
![[Pasted image 20230808145750.png]]
