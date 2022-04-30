# Homomorphismus
---

Eine Abbildung $h: A^* \to B^*$ ist ein **Homomorphismus**, wenn gilt $h(w_1 \cdot w_2) = h(w_1) \cdot h(w_2)$. Zudem gilt $h(\epsilon) = h(\epsilon\epsilon) = h(\epsilon)h(\epsilon) \Rightarrow |h(\epsilon)|=0 \Rightarrow h(\epsilon)=\epsilon$.

Ein Homomorphismus ist **Epsilon-frei**, wenn kein $x \in A$ auf $\epsilon$ abgebildet wird.

Ein Homomorphismus ist **Präfix-frei**, wenn für zwei verschiedene Eingaben $x_1, x_2$ gilt $h(x_1)$ ist kein Präfix von $h(x_2)$. Dieser Fall ist besonders für Codierungen interessant.