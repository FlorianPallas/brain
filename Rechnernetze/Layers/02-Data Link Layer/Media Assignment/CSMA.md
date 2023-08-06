**Carrier Sense Multiple Access**

## Usage
- Listen before talk
	- Device checks if the medium is usable before sending
- Because of the time it takes for a signal to fill the medium collisions are still possible

## Repeat Strategies
### 1-Persistent / $p$-Persistent
- Device listens, medium is in use
- Device keeps listening until its free
- Device starts sending with a probability of $p$
	- Selecting a good $p$ is difficult and varies from network to network -> Exponential Back off

### Non Persistent
- Device listens, medium is in use
- Device waits a random amount of time
- Is the medium not in us: Device sends immediately

### Exponential Back off
- Device waits a random amount of time before sending
- Maximum time to wait is doubled after each retry
- When a frame is sent successfully the timer is reset to default