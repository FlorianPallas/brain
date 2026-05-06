
# Anntrittsvortrag

Anmerkungen vom Prof in den Antrittsvortrag
- Simulation vs Emulation
- Latencies und Topologien simuliert, Rest emuliert
Immich Beispiel hätte genauer beschrieben werden sollen

Abschlussvortrag: Was hab ich gemacht? - 20m

# Pläne
- [x] Modernization
- [ ] Main simulation
	- [x] Differential privacy
	- [x] Label Flipping
		- Modell zeigt 10% Accuracy - Random Guess
		- Training zerbricht
	- [x] Trimmed Mean Aggregation
		- Konfigurierbar
		- Training ist robust gegen Poisoning
		- Modell trotz Poisoning akkurat
		- Viel Variation - Topologie?
		- Malicious Nodes sollten wahrscheinlich nicht aggregieren
	- [ ] Compression

- [x] Template setup
- [x] Typst Template
	- [x] Logos im Gitlab
	- [x] LATEX battle tested

- Experimentieren wie weit man auf der Hardware simulieren kann. z.B. mehr Nodes
	- 128 Nodes schon schwierig
	- Eventuell GPU möglich? - VRAM Probleme?

- Imagenet oder andere Datesets mit mehr Auflösung ist interessanter
	- Imagenet sehr groß - 256, 128
		- https://huggingface.co/datasets/ILSVRC/imagenet-1k
		- https://huggingface.co/datasets/benjamin-paine/imagenet-1k-128x128
	- CelebA Federated - 224, 64
		- https://huggingface.co/datasets/flwrlabs/celeba
	- Camelyon17 Medical - 50k,96
		- https://huggingface.co/datasets/jxie/camelyon17
		- https://huggingface.co/datasets/wltjr1007/Camelyon17-WILDS
	- Andere textbasierte
		- https://huggingface.co/flwrlabs/datasets

- AI
	- Was wurde gemacht
	- Was hat geklappt was nicht
	- etc.
	- Nicht sehr genau, keine Prompt. Wenn nur als Beispiel

Implementierung nur wichtige Teile erklären
- z.B. Differential Privacy, Trimmed Mean, und co.
- Librariers erklären wie Opaqus relativ genau
- Architekturdiagramm, etc.

Vergleich zwischen DP von Text und Image wäre interessant
Alle Sachen im Proposal sollten gemacht sein. Nur aus guten Grund nicht.
