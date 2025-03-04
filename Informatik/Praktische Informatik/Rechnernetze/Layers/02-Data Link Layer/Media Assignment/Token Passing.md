Token passing is a way to control which sender within a network is allowed to send. It adds a special frame that transfer the right to send to the receiver. Token has to be passed along.

Requires token management as token frames might be dropped or duplicated.
## Token Ring
- Ring Network
- Unidrectional links
- Token holding time (THT) limits sending time
- Control information can be piggy backed
- Priority mechanism with 8 priority levels
- One device monitors the ring

![[Pasted image 20230806193956.png]]

The token ring can be implemented using a special relay to keep the ring up even if a link disconnects. Distributed token control. Signals are always regenerated on each device -> less noise


## Token Bus
- Bus network
- Tokens are passed using a logical ring (simulated ring network)

![[Pasted image 20230806194343.png]]

### Polling
- Bus network
- One device communicates with every other device and asks for data
- Communication only through the central device
- Single point of failure
- Used for [[Bluetooth]], [[HLDC]]

![[Pasted image 20230806194442.png]]