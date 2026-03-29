In comparison to the [[Byzantine Threat Model]], the **Sybil Attacker** does not attack a [[Network]] through malicious behavior of nodes, but through control of identity.

The attacker creates multiple fake nodes that are now under his control. However, they act like any other node would. This impacts how consensus is formed within the network, since the attacker controls more of the vote than one would assume.

## Example
A [[P2P Network]] consists of 1000 nodes and achieves consensus through a majority vote. A sybil attacker can influence the outcome of that vote by spinning up enough nodes to control more than 50% of the networks nodes. The nodes act normally, but the attacker maintains full control.
