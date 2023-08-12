The internet protocol provides an unreliable, best effort, connection less service. It is responsible for forwarding IP [[Datagram|datagrams]] within the internet.

![[Pasted image 20230806173501.png]]

## Receiving
The following checks are performed when receiving an IP [[Packet|packet]]:
- Header length?
- IP version?
- Data length?
- Checksum?
- TTL (Time to Live)?
- Protocol?
If an error is detected an [[ICMP]] [[Datagram|datagram]] might be sent.