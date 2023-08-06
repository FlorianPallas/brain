- Multiplexing: Uses varying, random, time multiplexing using [[CSMA CD|CSMA/CD]] with 1-persistent exponential back off. When using duplex no collision detection is required.
- Topology:
	- Used a bus topology - today star topology
- Different data rates
	- 10 Mbit/s, 100 Gbit/s+
- Wired, Varying media
	- Coaxial, Fiber, Twisted Pair

## Frame
![[Pasted image 20230806195521.png]]
If type or length is used depends on the specific standard. In reality both are used.

Ethernet requires a minimum packet length. Smaller packages are padded.

![[Pasted image 20230806195432.png]]

## Variants
![[Pasted image 20230806200441.png]]

### 1000Base-T
- Speeds up to 1 Gbit/s
- Requires high minimum frame length for collision detection -> Only supports duplex, No busses, repeaters or hubs anymore
- Frame is untouched