The User Datagram Protocol provides an unreliable, best effort service. It does not require a connection, it just sends data.

## Header
The UDP pseudo header is not sent along with the data. Instead UDP uses the [[IP]] header. However the pseudo header is still calculated for the checksum.

![[Pasted image 20230803135523.png]]

### Error Detection
Errors are detected using a checksum. Invalid packages are simply dropped. While the checksum may be disabled by setting it to zero when using [[IPv4]], for [[IPv6]] it is mandatory as the protocol does not provide its own checksum.

## Usage
- VoIP, Multimedia
- DNS