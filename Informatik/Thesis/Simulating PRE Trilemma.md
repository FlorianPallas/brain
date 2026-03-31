## Setup
- Define Dataset
	- [[CIFAR-10]]
	- [[MNIST]]
	- [[FEMNIST]]
- Define utility metrics (Accuracy, F1-Score) of baseline
- Establish Threat model
	- Decentralized
	- Infrastructure secured
	- [[Sybil Attacker]]

## Scenarios
- Baseline
	- No mitigations
	- Performance baseline
- Privacy-Robustness
	- e.g. SaaS platforms
	- Privacy and Attack resistance is key
	- Increased cost is managable
- Robustness-Efficiency
	- e.g. Fleets
	- Availability and Latency is key
	- Privacy not feasible for these real-time applications
- Privacy-Efficiency
	- e.g. GBoard, Hospitals
	- Privacy and Bandwidth concerns
	- Mitigations: DP
	- Breakpoint: DP budget

## Scenarios
### Baseline
### Keyboard Predictions
Focus: Privacy & Efficiency
Threat Model:
- Location: Insider
- Behavior: Malicious
- Collusion: up to 10%
- Knowledge: White box

## Scenarios
1. State the threat model and focus properties
2. Implement techniques to improve focus properties
	1. Define DP budget bound
	2. Define malicious nodes fraction bound
	3. Define bandwidth limits
3. Simulate
	1. Implement malicious nodes
	2. Implement attacks
	3. Run until DP budget is reached, or convergence
4. Evaluate
	- Privacy
		- Target DP budget
		- Membership inference
			- Split dataset equally in trained on and never-seen
			- Feed all images into the model & classify into member or non-member
			- Measure
				- Precision: Out of all the records the attacker claimed were in the training set, how many actually were?
				- Recall / TPR: Out of all the true training records, how many did the attacker successfully identify?
				- ROC-AUC: This is the most robust metric for MIA ASR, as it measures the attacker's success across all possible threshold values.
	- Robustness
		- Attack success rate
			- $A$ How many data points does the model now get wrong that it got correct initially?
			- $B$ How many data points did the model predict correctly initially?
			- Success Rate = $A / B * 100\%$ 
	- Efficiency
		- Training time
		- Bandwidth per-round per-client
		- Gap to baseline accuracy

## Techniques
- Privacy
	- [[Differential Privacy]] against [[Membership Inference]]
- Robustness
	- [[Trimmed Mean Gradient Descent]] against [[Label Flipping]]
- Efficiency
	- [[Gradient Sparsification]], [[Quantization]], or train more rounds locally using [[FedAvg]] to lower bandwidth
