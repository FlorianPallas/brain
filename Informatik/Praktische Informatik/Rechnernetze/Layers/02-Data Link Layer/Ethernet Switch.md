Switches that use [[Ethernet]]. They learn from the traffic they send and construct a minimum spanning tree.

## Learning
When a frame is received by the switch it remembers that the sender of that frame is reachable from that interface. Next time it needs to forward a packet to that sender it know where to send it. These entries have a TTL and look like this: `<MAC, Interface, TTL>`. If the address is unknown it floods the frame on all interfaces.