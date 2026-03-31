# Deep Learning with Differential Privacy
#literature 

## Summary
The paper introduces a practical framework for training deep neural networks with rigorous differential privacy guarantees. The authors demonstrate that models can be trained without exposing the sensitive information of individual records in the training data, while keeping the costs to model accuracy, software complexity, and training time manageable.

## Algorithms
- Differentially Private Stochastic Gradient Descent (DP-SGD)

## Simulations
DP-SGD was tested on both [[CIFAR-10]] and [[MNIST]] datasets. The authors proved that models can be trained under tight privacy gurantees $(8, 10^{-5})$ while maintaining accuracy of 73% on CIFAR-10 and 97% on MNIST.
