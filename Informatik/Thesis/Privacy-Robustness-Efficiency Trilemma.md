---
aliases:
  - PRE Trilemma
---
The Privacy-Robustness-Efficiency Trilemma states that it is infeasible for [[Machine Learning]] systems to perfectly maintain Privacy, Robustness, and Efficiency simultaneously under worst-case threat assumptions.

![[Pasted image 20260325125701.png|340]]


## Privacy
A machine learning system is private if no source data can be retrieved from the model gradients.
### Metrics
- $(\epsilon, \delta)$-[[Differential Privacy|DP]] budget: How much noise do I need to add to achieve a certain level of privacy? Higher noise necessary -> Scenario is less private
- [[Membership Inference]] attack success rate


## Robustness
A machine learning system is robust, if it maintains a certain measure of availability and accuracy under threat.
### Metrics
- Attack success rate of a robustness attack under a state thread model


## Efficiency
A machine learning system is efficient, if it converges to reach a desired accuracy in a reasonable time frame and using reasonable compute.
### Metrics
- Convergence: Training time
- Bandwidth: Per-client bytes/round
- Accuracy: Gap compared to no-defense baseline
### Comparison to Utility
While theoretical research often uses utility as a measure, more practical research uses efficiency as a metric. While they are distinct topics, they are linked. Utility refers to the actual performance of a model like accuracy and learning error. But in practical applications perfect utility might be theoretically possible but not feasible. Efficiency therefore instead refers to computational efficiency, required bandwidth, and convergence speed of the model.

## References
- [[AGS23]]
- [[AGG+23]]
