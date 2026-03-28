---
aliases:
  - Gradient Perturbation
  - DP
---
Differential Privacy adds noise to gradients before sharing them with other clients in [[Federated Learning]] systems. This makes it harder to reconstruct source data.

## $(\epsilon,\delta)$-Budget

$\epsilon$ defines the trade-off between privacy and utility. The lower the value of $\epsilon$ the more private the solution, however accuracy of the resulting model might decrease. Higher privacy is achieved by increasing the added noise.

https://arxiv.org/abs/2402.02230
https://flower.ai/docs/framework/explanation-differential-privacy.html
https://arxiv.org/abs/1203.3453
