---
aliases:
  - Byzantine Fault Tolerance
  - BFT
---
The **Byzantine Threat Model** is popular in applications where a [[Network]] is involved. It is assumed that the environment is a network of compromised and uncompromised nodes.

Compromised nodes have the ability to:
- Lie about their state
- Send different data to different peers
- Stop responding

Systems that implement mitigations to success are labeled **Byzantine Fault Tolerant (BFT)**.
