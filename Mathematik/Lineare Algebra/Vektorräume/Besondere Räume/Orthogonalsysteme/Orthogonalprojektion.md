---
aliases: []
---

# Orthogonalprojektion #card
## Definition
Es sei V ein [[Vektorraum]] mit [[Standardskalarprodukt]] und U ein endlich-dimensionaler Untervektorraum. Die Abbildung
$$
\Pi_{U}: V=U \oplus U^{\perp} \rightarrow V, \quad v=u+u^{\perp} \mapsto u
$$
heißt Orthogonalprojektion auf U. In diesem Fall lässt sich auch die Orthogonalprojektion auf den (möglicherweise unendlich-dimensionalen) Untervektorraum $U^{\perp}$ definieren durch
$$
\Pi_{U^{\perp}}: V=U \oplus U^{\perp} \rightarrow V, \quad v=u+u^{\perp} \mapsto u^{\perp}
$$
## Berechnung
Ist $\left(b_{1}, b_{2}, \ldots, b_{k}\right)$ eine [[Orthonormalbasis]] von $U$, so gilt für alle $v \in V$
$$
\Pi_{U}(v)=\sum_{i=1}^{k}\left\langle v, b_{i}\right\rangle b_{i}
$$
Ist $\left(b_{1}, b_{2}, \ldots, b_{k}\right)$ eine [[Basis]] lässt sich nach dem [[Gram-Schmidt-Verfahren]] die Orthogonalprojektion folgendermaßen berechnen:
$$
\Pi_{U}(v)=\sum_{i=1}^{k} \dfrac{\left\langle v, b_{i}\right\rangle}{\left\langle b_i, b_{i}\right\rangle} b_{i}
$$
## Folgerungen
- $\Pi_{U}$ ist linear
- $\operatorname{ker}\left(\Pi_{U}\right)=U^{\perp}$
- $\operatorname{Bild}\left(\Pi_{U}\right)=U$, und für die Einschränkung $\Pi_{U} \mid u: U \rightarrow U$ gilt $\Pi_{U} \mid u=\mathrm{id}_{U}$.
- $\Pi_{U}^{2}=\Pi_{U}$
- $\Pi_{U^{\perp}}=\mathrm{id}_{V}-\Pi_{U}$
- $\left\|\Pi_{U}(v)\right\| \leq\|v\|$  $\forall v \in V$

^c-RxJKcZhQCA
---
**Tags**: 