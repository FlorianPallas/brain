---
aliases: [total db., db., differenzierbar, total differenzierbar]
---

# Totale Differenzierbarkeit
## Motivation
Die [[Partielle Differenzierbarkeit|partiellen Ableitungen]] von $f: D \subseteq \mathbb{R}^n \to \mathbb{R}$ berücksichtigen nur das Veralten von $f$ entlang der Achsenrichtungen. Wir wollen nun einen Differenzierbarkeitsbegriff aus dem (wie im Reellen) [[Stetigkeit]] folgt.

## Definition
$f$ heißt **(total) differenzierbar** in $a \in D$, wenn $f$ [[Partielle Differenzierbarkeit|pdb.]] ist und
$$
\lim_{h\to 0} \frac{f(a+h) - f(a) - grad f(a) \cdot h}{||h||} = 0
$$
existiert.

### Bemerkung
Im Eindimensionalen ($n=1$) ist Differenzierbarkeit gleichbedeutend mit [[Partielle Differenzierbarkeit|partieller Differenzierbarkeit]]. Im Fall $n \geq 2$  stimmt das nicht mehr.

Auch wenn alle Richtungsableitungen (partiellen Ableitungen in jede Richtung) existieren, gilt nicht direkt totale Differenzierbarkeit!

## Folgerungen
### Aus Differenzierbarkeit folgt Stetigkeit der Funktion.
$f$ db. in $a$ $\Rightarrow$ $f$ stetig in $a$

### $C^1$-Kriterium
Wenn $f$ [[Partielle Differenzierbarkeit|pdb.]] auf $D$ ist und alle partiellen Ableitungen der Ordnung $1$ stetig in $a \in D$, so ist $f$ db. in $a$. Insbesondere gilt: $f \in C^1(D)$, dann ist $f$ db. auf ganz $D$.
z.B. [[Potenzreihen]] sind stets db.

## Verfahren
- (Stetigkeit wiederlegen)
- partielle Differenzierbarkeit prüfen (und $grad$ bestimmen)
- Differenzierbarkeit prüfen
    - $C^1$-Kriterium anwenden (kein Wiederlegen)
    - Definition anwenden ($\lim$ nachrechnen)

## Beispiele
### Differenzierbar, trotz fehlender Stetigkeit der partiellen Ableitungen im Nullpunkt
![[Pasted image 20220518123113.png]]
![[Pasted image 20220518123133.png]]
![[Pasted image 20220518123150.png]]

---
**Tags**: 