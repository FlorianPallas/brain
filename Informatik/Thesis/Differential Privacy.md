---
aliases:
  - Gradient Perturbation
  - DP
---
**Differential Privacy** is a privacy-preserving measure, which clips or adds noise to gradients before sharing them with other clients in [[Federated Learning]] systems. This makes it harder to infer if data was part of the original training data set, or reconstruct parts of the training data.

## $(\epsilon,\delta)$-DP Budget
The $(\epsilon,\delta)$-DP budget is a popular measure for privacy guarantees of machine learning systems.

When comparing a data point that is part of the training set and another that is not, $\epsilon$ is the maximum change in probability between them. This makes sure that [[Membership Inference]] is hindered. $\delta$ is the probability that the $\epsilon$ bound might be broken. For strong privacy guarantees, this value should be below $1/|d|$, where $|d|$ is the size of the dataset.

Common values for $\epsilon$ are 8 for balance, 2 and 4 for higher privacy with noticeable accuracy loss and 0.5 for high privacy use cases.

## References
- [[ACG+16]]
- https://flower.ai/docs/framework/explanation-differential-privacy.html
