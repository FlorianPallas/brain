---
aliases:
  - Parallelism
  - Concurrency
---

## Parallelism

Example: Two [[Thread|Threads]] are executed simultaneously.

## Concurrency

Example: At least two [[Thread|Threads]] make progress.
Concurrency is not strictly reliant on Parallelism, since it can also be achieved using virtual Parallelism, like time-slicing.

## Partitioning

The problem needs to be partitioned in order to allow parallel processing.

- Task parallelism: functional decomposition
  - Define tasks that can be executed in parallel
  - Tasks should be as independent as possible
- Data parallelism: data decomposition
  - Partition the data on which the same operation is executed on in parallel
  - Tasks should be able to work on the partitions as independently as possible

## Further Challenges

- [[Inter-Process Communication]]
- [[Race Condition|Race Conditions]]
- [[Deadlock|Deadlocks]]
