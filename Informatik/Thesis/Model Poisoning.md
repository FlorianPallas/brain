Model Poisoning is an attack in [[Federated Learning]] systems where a malicious user can share invalid gradients to reduce the accuracy of the global model. This is different to [[Data Poisoning]], where the dataset itself is poisoned but the training process is untouched.

## Strategies
- Label Flipping: Training on purposefully flipped labels of the dataset
- Malicious Gradients: Generate harmful gradients with high magnitudes to negate or overshadow the impact of other nodes

## Mitigations
Byzantine-robust aggregation
- Outlier Removal
- Trimmed Mean
- Median Aggregation

## References
- [[YCK+18]]