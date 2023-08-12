
## Datagram
![[Pasted image 20230806173556.png]]
The minimum IP header length is 20 byte.

The datagram can be split into multiple if necessary. To signal this we use the flag field in and the fragment offset (signals the position where the fragment has to be inserted to get the full datagram) of the IP header. This might be necessary as different systems require different frame lengths (MTU: Maximum Transfer Unit).
- Bit 0: reserved as 0
- Bit 1: AllowFragmentation: 0 = allow, 1 = disallow
- Bit 2: IsLastFragment: 0 = yes, 1 = no

![[Pasted image 20230806173924.png]]

## Address
A IPv4 address contains 4 groups of 8 bits separated by dots (32 bits). For ease of use leading zeroes can be left out.

![[Pasted image 20230806172836.png]]