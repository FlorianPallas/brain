The Transmission Control Protocol provides a reliable service.
### Header
![[Pasted image 20230803135443.png]]

### Connection
#### Initiate
To initiate a TCP connection a three way handshake is performed (SYN, SYN-ACK, ACK).
The purpose of this is to communicate the initial sequence numbers and window sizes of both peers reliably before data is sent.

1. Client -> Server: `SYN, SEQ=ClientSEQ, RcvWnd=ClientRcvWnd`
2. Server -> Client: `SYN, ACK, SEQ=ServerSEQ, ACK=ClientSEQ+1, RcvWnd=ServerRcvWnd
3. Client -> Server: `ACK, SEQ=ClientSEQ+1, ACK=ServerSEQ+1`
#### Closing
To close a TCP connection each client requests the close and waits for confirmation. This results in 4 packets sent with two peers (FIN, ACK, FIN, ACK). Any peer can start closing the connection, so Client and Server can be switched here.

1. Client -> Server: `FIN, SEQ=ClientSEQ, ACK=ServerSEQ`
2. Server -> Client: `ACK, SEQ=ServerSEQ, ACK=ClientSEQ+1`
3. Server -> Client: `FIN, SEQ=ServerSEQ, ACK=ClientSEQ+1`
4. Client -> Server: `ACK, SEQ=ClientSEQ+1, ACK=ServerSEQ`

There is a short wait before the local context is deleted. To prevent this the `RST` flag may be set. Normally this is not set.

### Piggy Backing
When sending acknowledgements it is possible to include additional data by piggy packing it.

### ARQ
TCP uses the [[Go Back N]] [[ARQ]] Algorithm to make sure invalid or dropped packages are resent automatically.

### Error Detection
Errors are detected using a Checksum. Invalid packages do not get acknowledged and will eventually be resent by the sender.

The checksum is calculated by adding up all bytes individually. At the end the carry is added and the whole result is inverted (One Complement).

### Congesting Control
TCP Congestion can be defined in three stages:

- **Slow Start**: The congestion window CWND is set to 1 MSS initially and increased by 1 MSS for every ACK received. The window defines how many segments are allowed to be sent.
- **Congestion**: When packets are dropped, the CWIND is reset to 1. Additionally SSThresh is set to $max(FlightSize \div 2, 2 \cdot MSS)$. Then we switch back to Slow Start. Initally SSThresh is a large number, to allow Slow Start to rapidly find the real threshold of the connection.
- **Congestion Avoidance**: As soon as CWND $\geq$  SSThresh the state changes from Slow Start to Congestion Avoidance. Now the CWIND is only increased if the full windows sent (so multiple packages) are ALL acknowledged. And it is only increased by $1 \div CWD$. Which results in an increase of 1 in the CWD.
