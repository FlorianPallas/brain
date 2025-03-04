Systems in a subnet can communicate with each other without the need of a router. A subnet is uniquely defined using its subnet prefix.

## Subnet prefix
The subnet prefix is variable length address that identifies the network and the addresses used within it (`192.168`). Typically the prefix is part of a formatted string that also includes the suffix and the amount of bits assigned to the subnet (`192.168.0.0/16`).

## Subnet mask
The subnet mask defines which part of an address is part of the subnet. The bits belonging to the subnet are written as `1`, the bits of the target system as `0`. This allows the subnet prefix to be calculated using `prefix = address AND subnet mask`.

![[Pasted image 20230806172337.png]]

## Special addresses
Assuming `192.168.178` is the subnet prefix there are two special addresses:
- `192.168.178.0` identifies the network itself
- `192.168.178.xxx` defines a system within the network
- `192.168.178.255` is a broadcast address