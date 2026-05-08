---
created: "2026-05-07"
tags:
  - note-fleeting
---
- Sample-Level LDP
	- Protects individual pieces of data
	- Noise gets added to every training sample
	- Completely blocks data extraction and reconstruction attacks
		- e.g. Deep Leakage from Gradients
	- Heavy to compute
	- Tool: Opacus
- Client-Level LDP
	- Protects the node or user
	- Node trains normally, adds noise to final deltas
	- Hides whether a device participated in a round
	- Easier to compute
	- Tool: Custom

For my thesis I probably want Sample-Level LDP, since the idea is to prevent Deep Leakage from Gradients.
