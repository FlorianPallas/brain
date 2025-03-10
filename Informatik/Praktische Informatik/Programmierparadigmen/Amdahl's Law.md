The possible speedup of an algorithm executed on $n$ processors can be computed, with $T(n)$ being the time a program needs when processed by $n$ processors.
$$S(n) = \frac{T(1)}{T(n)}$$

Amdahl's law computes the maximal speedup possible, with $p$ being the percentage of the program that can be parallelized.
$$S(n) = \frac{1}{(1-p) + \frac{p}{n}}$$

This shows that the effective speedup is greatly limited by the non-parallel parts of a program, even for large $n$.
Due to overhead, even this limit is hardly reachable in practice.
