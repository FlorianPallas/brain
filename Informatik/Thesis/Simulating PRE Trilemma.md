## Setup
- Define Dataset
	- [[CIFAR-10]]
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
	- $\epsilon < 10$

## Benchmarking
How often are benchmarks run?

## Privacy Evaluation
- Measure the required $(\epsilon,\delta)$-[[Differential Privacy|DP]] budget
- Perform a [[Membership Inference Attack]] and measure the success rate
- (Perform a [[Gradient Leakage Attack]] and measure the reconstruction error)

## Robustness Evaluation
- Perform a [[Model Poisoning]] attack and measure the success rate

## Efficiency Evaluation
- Measure training time
- Measure accuracy gap to baseline
- Measure used bandwidth per-client per-round
