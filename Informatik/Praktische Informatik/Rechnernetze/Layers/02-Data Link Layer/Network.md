

## Topologies
### Fully Connected Mesh
Every device is connected to all other devices with a physical [[Link|link]]. Requires $\frac{n(n-1)}{2}$ links in total.
![[Pasted image 20230806190009.png]]

### Partially Connected Mesh
Only some devices are directly connected. Communication over multiple devices necessary.
![[Pasted image 20230806190013.png]]

### Hierarchical / Tree
- Devices are order in a tree like structure (e.g. old telephone network)
![[Pasted image 20230806190024.png]]

### Star
- Centralized component every device communicates with
- Single point of failure
![[Pasted image 20230806190140.png]]

### Ring
- Every device is connected with the previous and following device
- Communication is restricted when multiple links fail
![[Pasted image 20230806190226.png]]

### Bus
- All devices are connected with a single link
- Link failure stops all communication
![[Pasted image 20230806190240.png]]