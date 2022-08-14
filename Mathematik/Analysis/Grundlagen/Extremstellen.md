---
aliases: [kritische Stelle, stationäre Stelle, Extremstelle, Minimalstelle, Maximalstelle, Sattelstelle]
---

# Extremstellen
## Definition #card
Sei $f: D \subseteq \mathbb{R}^{n}\to \mathbb{R}$, so heißt $u \in D$  **kritische Stelle** oder **stationäre Stelle**, wenn der [[Gradient]] verschwindet, also $grad f(u) = (0, \; \dots \; , 0)$.

Ist $f$  [[Partielle Differenzierbarkeit|pdb.]] auf einer [[offene Mengen|offenen Menge]] $D \subseteq \mathbb{R}^{n}$ definiert, dann ist jede **Extremstelle** von $f$ eine **kritische Stelle**.

Daher müssen nur kritische Stellen geprüft werden um Extremstellen zu finden.
Aber: Es kann kritische Stellen geben, die keine Extremstellen sind. Diese Stellen heißen **Sattelstellen** von $f$.
^c-JcTJXBk2hA

## Kriterien
### [[Definitheit]]
Ist $f \in C^{2}(D)$, dann gilt für jede **kritische Stelle** $u \in D$ von $f$:
- $H_{f}(u)$ positiv definit $\Rightarrow$ $u$ ist lokale **Minimalstelle**
- $H_{f}(u)$ negativ definit $\Rightarrow$ $u$ ist lokale **Maximalstelle**
- $H_{f}(u)$ indefinit $\Rightarrow$ $u$ ist **Sattelstelle**
- sonst - keine Aussage

### $2 \times 2$ Matrizen:
$$A = \begin{pmatrix} \alpha  & \beta \\ \beta  & \gamma \end{pmatrix}$$
- $det(a) > 0$ und $\alpha > 0$ $\Leftrightarrow$ positiv definit
- $det(a) > 0$ und $\alpha < 0$ $\Leftrightarrow$ negativ definit
- $det(a) < 0$ $\Leftrightarrow$ indefinit


## Verfahren #card
- Kritische Stellen bestimmen
    - [[Gradient]] berechnen
    - Nullstellen des Gradients bestimmen
- [[Hesse-Matrix]] aufstellen
    - Allgemeine Hesse-Matrix berechnen
    - Falls Variablen übrig bleiben, Hesse-Matrix aller kritischer Stellen berechnen
- Kriterien anwenden
    1. Bei Diagonalmatrix über [[Eigenwerte]] bestimmen (oder [[Diagonalisierbarkeit|diagonalisieren]])
    2. $2\times2$ Kriterium anwenden
    3. Anderweitig argumentieren
        - Beweis durch Widerspruch - Punkt ist keine Extremstelle
        - $\dots$
^c-WvAzkFj55a

## Beispiele
### Alle möglichen Fälle im Schaubild
![[Pasted image 20220525123416.png|400]]
### Bestimmung aller Extrempunkte (Sattelpunkt)
![[Pasted image 20220525123203.png|400]]
### Bestimmung aller Extremstellen
![[Pasted image 20220525123538.png|400]]

---
**Tags**: 