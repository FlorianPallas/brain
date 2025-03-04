IPv6 is meant to be the successor to [[IPv4]] and improves upon the standard. It provides larger addresses to support more addressable devices. It gets rid of fragmentation, checksums, header length and options (-> header extensions) in the datagram header to provide a easier header format. It adds flow labels to identify [[Packet|packets]] in data streams.

## Header
![[Pasted image 20230806175313.png]]

### Comparison to [[IPv4]]
![[Pasted image 20230806175348.png]]

## Address
An IPv6 address consists of 8 groups of 16 bits (128 bits), separated by colons. Each group is displayed using a 4 digit hex string. For ease of use leading zeros can be removed. **ONE** series of zeroes can even be replaced with `::` (typically the largest one).

![[Pasted image 20230806172015.png]]

There are three types of IPv6 addresses:
- Unicast: Identifies a single interface a datagram is sent to
- Multicast: Identifies a group of interfaces which all receive the same datagram.
- Anycast: Identifies a group of interface from which ONE receives the datagram.