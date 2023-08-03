---
aliases: []
---

# Linearisierung #card
## Definition
Eine [[Funktion]] $f: D \subseteq \mathbb{R}^n \to \mathbb{R}$, welche in $u \in D$ [[Partielle Differenzierbarkeit|pdb.]] ist, heißt
$$
L_{f,u}: \mathbb{R}^{n}\to \mathbb{R}, L_{f,u}(x):=f(u) + f'(u) \cdot (x-u)
$$
oder mit $h = x-u \Rightarrow x = u + h$
$$
L_{f,u}(u+h) = f(u)+f'(u) \cdot h
$$
die **Linearisierung** von $f$ bei $u$.

## Konzept
Die **Linearisierung** einer Funktion $f$ an einer Stelle $u$, versucht die Funktion anzunähern indem sie die Steigung an der Stelle $u$ beibehält, vergleichbar mit der Tangente im Punkt $(u, f(u))$. An der Stelle $u$ ist die Linearisierung identisch mit der originalen Funktion.

## Folgerungen
f ist [[Totale Differenzierbarkeit|db.]] in u $\Leftrightarrow \lim_{x\to u} \frac{f(x) - L_{f,u}(x)}{x-u} = 0 \Leftrightarrow \lim_{h\to 0} \frac{f(u+h)-L_{f,u}(u+h)}{h}=0$

## Beispiele
### Beispiel im $\mathbb{R}^1$
![[Pasted image 20220601121816.png|400]]
### Beispiel im $\mathbb{R}^n$
![[Pasted image 20220601121909.png|400]]
^c-9W6wTzn6Ue

---
**Tags**: #todo 