The **Dynamic Host Configuration Protocol** distributes [[IP]] addresses of a [[Subnet|subnet]] to clients. The assigned addresses are temporary and maybe be changed after the claim expires.

DHCP also provides some basic information about the subnet. This may include:
- Address of the default [[Router|router]]
- Name and [[IP]] address of the [[DNS]] server
- Subnet mask
- Time server ([[NTP]])

## Commands
- discover: client requests dhcp guidance
- offer: the dhcp server offers an address to the client
- request: the client requests a certain address / accepts the offer
- ack: the dhcp server assigns an ip address

![[Pasted image 20230806184533.png]]
![[Pasted image 20230806184541.png]]