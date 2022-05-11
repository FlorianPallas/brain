---
aliases: []
---

# Produktterm #card
## Definition
Ein Produktterm $K\left(x_{1}, \ldots, x_{m}\right)$ ist die Konjunktion von [[Literal|Literalen]] $\bigwedge_{i=1}^{m} L_{i}=L_{1} \wedge \cdots \wedge L_{m}$. Die Konstanten „0" oder „1" dürfen dabei auftreten.
Jeder Produktterm
$$
K\left(x_{1}, \ldots, x_{m}\right)=\bigwedge_{i=1}^{m} L_{i}
$$
kann so dargestellt werden, dass eine Variable $x$ in höchstens einem Literal vorkommt. Falls $L_{h}=x$ und $L_{j}=x$ ist, gilt $L_{h} \wedge L_{j}=x$, und es ist
$$
K\left(x_{1}, \ldots, x_{m}\right)=\bigwedge_{i=1, i \neq j}^{m} L_{i}
$$
Entsprechendes gilt für $L_{h}=L_{j}=\bar{x}$; ist jedoch $L_{h}=x$ und $L_{j}=\bar{x}$ (oder umgekehrt), so erhält $\operatorname{man} K\left(x_{1}, \ldots, x_{m}\right)=0$.
## Beispiele
- $a \wedge b$
- $\bar{a} \wedge b$
- $a \wedge \bar{b}$
- $\bar{a} \wedge \bar{b}$ 
^c-4TUysA7SxR
---
**Tags**: 