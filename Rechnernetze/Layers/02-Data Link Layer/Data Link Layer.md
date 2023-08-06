The data link layer provides a service upon the [[Physical Layer]]. It does not guarantee that bits are communicated correctly.

## Tasks
- Providing reliable and unreliable services
	- Reliable services require error detection and correction of the data from the [[Physical Layer]].
- Addresses
	- Provide addresses for the devices connected to the physical medium.
- Buffering data when sending and receiving
- Structured communication of [[Frame|frames]]
- Abstraction from the [[Physical Layer]]

## Implementation
The logic of the data link layer is located in network interface cards, network chips (e.g. Ethernet adapter, WiFi adapter) or buses within a system (e.g. PCI bus). The are a combination of software and hardware.