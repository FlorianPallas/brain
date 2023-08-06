Uses time multiplexing with varying, random access.

## Usage
- Just start sending
- No check of the medium or send request or notification
- Useful for networks with high latency and little communication
- Collisions possible

![[Pasted image 20230806191715.png]]

## Collision Detection
- Explicit
	- Acknowledgements of upper layers
	- Requires extra communication channel
- Implicit
	- Broadcast received frames
	- Sender can read and check if his frame was received
	- Used for satellites

When a collision is detected the frame is sent again. To prevent another collision the time when the frame is repeated is randomized and includes a back off period. The communication is aborted after a certain number of retries is reached.
