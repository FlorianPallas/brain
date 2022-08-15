---
aliases: ["L'Hospital"]
---

# Regel von de L'Hospital  #card
## Definition
Sei $I = (a,b)$ ein offenes Intervall ($a,b \in \mathbb{R} \cup \{  -\infty, \infty \}$) und $f,g: I \to \mathbb{R}$ auf $I$ [[Totale Differenzierbarkeit|differenzierbar]] mit $g'(x) \neq 0$ (auf allen $x \in I \setminus \{c\}$) und es sei $c = a$ oder $c = b$.
Zudem existiere der Grenzwert
$$
L := \lim_{x \to c} \frac{f(x)}{g(x)} \in \mathbb{R} \cup \{  -\infty, \infty \}
$$

Eine der folgenden Aussagen muss gelten:
- $\lim\limits_{x \to c} f(x) = \lim\limits_{x \to c} g(x) = 0$
- $\lim\limits_{x \to c} g(x) = \pm \infty$

Mit L'Hospital folgt nun:
$$
\lim_{x \to c} \frac{f'(x)}{g'(x)} = \lim_{x \to c} \frac{f(x)}{g(x)} = L
$$
Der Wert des originalen Grenzwert enspricht dem Grenzwert der abgeleiteten Terme.

### Bemerkungen
- Das $c$ muss nicht immer $\pm \infty$ sein. Trotzdem müssen die Funktionen entsprechend konvergieren!
- Existiert der Grenzwert der abgeleiteten Terme nicht, kann keine Aussage getroffen werden. Der originale Grenzwert kann trotzdem existieren!
- Die Umkehrung der Regel ist im allgmeinen nicht korrekt!


## Beispiele
### Korrekte Verwendung
![[Pasted image 20220810164642.png]]
### Inkorrekte Verwendung
![[Pasted image 20220810164713.png]]
Keine der Vorraussetzungen ist erfüllt, da $f(x) = \log x \neq 0$ und $g(x) = x \xrightarrow{x \to 1} 1 \neq \pm \infty$ gilt.

![[Pasted image 20220810164700.png]]
Existiert der Grenzwert nicht, kann keine Aussage auf den originalen Grenzwert getroffen werden.

### Klausuraufgabe
![[Pasted image 20220810171910.png]]
Beide Funktionen gehen gegen $0$ unabhänging des Parameters $m$.
^c-vgsKt18GcD

---
**Related:**
- [[Grenzwert]], [[Konvergenz]]
- https://en.wikipedia.org/wiki/L%27H%C3%B4pital%27s_rule
**Tags**: 