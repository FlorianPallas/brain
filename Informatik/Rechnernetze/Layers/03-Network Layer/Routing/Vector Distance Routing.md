## Protocols
- [[RIP]]

## Behavior
### Routing Table
In Vector Distance Routing all routers on a network hold a routing table. This includes the distance to any node in the network via all neighboring routers. These routing tables are replicated to all neighbors of a router on a certain time interval.

![[Pasted image 20230803181654.png]]

When a router receives the routing table of another route it adjust its table to reflect the distances to each node through that neighboring router. This is done by adding the shortest distance to the node as advertised by the neighbor and adding the distance to said neighbor to get the total distance to the node.

### Routing Packages
The shortest distance to a node can then be read by calculating the minimum of the corresponding row. The column of the entry reflects the neighboring router the packet needs to be sent to to follow that shortest path in the network.

## Count to Infinity Problem
When a link goes down, the router attached to the link will stop advertising the connection. However, because the routing tables are replicated to the neighboring routers, they will still advertise that connection through the original router.

The original router will try to find and alternate route to replace the missing link, however it does not know if the advertised route by his neighbors are actual routes around the link, or outdated values pointing back to the original router.

This creates an infinite loop, as the distance between the original router and his chosen neighbor is added each time the routing tables are replicated.

### Poison Reverse
To make sure this kind of loop does not happen. Any router A in the network that advertises a route through a neighboring router B will advertise that route to all neighbors, except to B itself. Router A will instead advertise the route with an infinite weight (Depending on the protocol the actual value of *infinite* may vary).

This makes sure any router will never consider an alternative route through itself. Solving the count to infinity problem.

## Problems
- Count to Infinity Problem
- Slow to propagate links that go down