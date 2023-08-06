The address resolution protocol solves the issue of finding the [[MAC Address]] when we only know the [[IP]] address of the target device.

- ARP cache / ARP table holds `<IP address, MAC address, TTL>`.
- If the target address is not cached, send a ARP request to all interfaces using the broadcast MAC address (`FF-FF-FF-FF-FF-FF`).
- Only the device that has the requested address sends a ARP reply.


## Packet
![[Pasted image 20230806201045.png]]

## Attacks
### DoS
- Send random ARP replies
- Caches are invalid and trigger more requests
- Good for wired, bad for wireless networks

### Man in the middle
- Send faked ARP replies
- Receive and modify packets