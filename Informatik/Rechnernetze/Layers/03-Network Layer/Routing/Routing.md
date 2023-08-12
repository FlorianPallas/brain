To get packages from point A to B the routers in the network need to know what the quickest path to B is. We commonly differentiate between two approaches to routing called [[Vector Distance Routing]] and [[Link State Routing]]. 

## Static Routing
Routes change only rarely. Route changes are rarer than changes in traffic. Does not necessarily the current state of the network.
-> Static routing tables

## Centralized Routing
A centralized component performs path calculations and distributes routing tables. This component needs a global map of the network.
-> Routing control center

## Dynamic Routing
Routes change based on traffic and topology. Makes loops and oscillations more likely. Can operate as reaction to events or periodically. Routers might have outdated information. Might create a lot of traffic because routers need to exchange routing information.
-> Dynamic routing tables

## Decentralized Routing
Routing decisions and calculations are performed in the routers. Does not require a centralized system. Routers only have access to data they collect themselves. Routers share data with neighboring routers.

- Isolated
	- Flood
	- Hot Potato
- Distributed
	- [[Vector Distance Routing]]
	- [[Link State Routing]]
