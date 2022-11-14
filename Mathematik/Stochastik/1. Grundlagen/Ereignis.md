## Definition #card 
Ereignisse sind Teilmengen $A \subseteq \Omega$ des [[Grundraum]], denen prinzipiell eine Wahrscheinlichkeit zugeordnet werden kann.
^c-LQ9UQNdvmZ

## Sprechweise #card 
Ereignis $A$ tritt ein $\Leftrightarrow$ Ergebnis $\omega$ liegt in $A$
^c-0X0xlaVHWC

## Hinweis #card 
- Nicht immer wird jede Teilmenge als Ereignis bezeichnet, sondern nur Mengen aus einem Mengensystem $A \subseteq P (\Omega)$, wobei
$P (\Omega):=\{A: A$ ist Teilmenge von $\Omega\}$ die Potenzmenge bezeichnet.
- Ist $\Omega$ endlich (oder allgemeiner höchstens abzählbar), dann wählt man typischerweise $A = P (\Omega)$, d.h. jede mögliche Teilmenge des Grundraums soll eine Wahrscheinlichkeit erhalten.
^c-7LmA1NUtfa

## Verknüpfungen von Ereignissen #card 
Seien $A, B \subseteq \Omega$ Ereignisse
- $A \cup B=\{\omega \in \Omega \mid \omega \in A$ oder $\omega \in B\}$ das Ereignis, dass $A$ eintritt oder $B$ eintritt (nicht exklusiv, d.h. es können auch beide Ereignisse eintreten),
- $A \cap B=\{\omega \in \Omega \mid \omega \in A$ und $\omega \in B\}$ das Ereignis, dass $A$ und $B$ eintritt,
- $A \backslash B=\{\omega \in \Omega \mid \omega \in A, \omega \notin B\}$ das Ereignis, dass $A$ eintritt, aber nicht $B$ eintritt,
- $B^c$ das Ereignis, dass $B$ nicht eintritt.
- $A \subseteq B$ bedeutet: Wenn $A$ eintritt, dann tritt auch $B$ ein.
^c-Do8bYaHLNM

## Beispiele
### Münzwurf #card 
Werfen einer Münze:
$$
\Omega=\{K, Z\}
$$
Das Ereignis "Es fällt Kopf" entspricht $A=\{K\}$.
^c-nIo84ZkGr2

### Würfelwurf #card 
Werfen eines Würfels:
$$
\Omega=\{1, \ldots, 6\}
$$
Das Ereignis "Augenzahl ist gerade" ist gegeben durch $A=\{2,4,6\}$.
^c-6KBaozREPB

### Netzwerk #card 
In einem Netzwerk werden Längen (in Byte) der ersten $n=10^5$ Datenpakete beobachtet, die an einem Router ankommen:
$$
\Omega= N ^n=\left\{\left(\omega_1, \ldots, \omega_n\right) \mid \omega_i \in N \text { für alle } 1 \leq i \leq n\right\}
$$
Interpretation: $\omega_i=$ Länge des $i$-ten Paketes
Das Ereignis "Das größte Paket umfasst maximal $10^7$ Byte" entspricht
$$
A:=\left\{\left(\omega_1, \ldots, \omega_n\right) \mid \omega_i \leq 10^7 \text { für alle } 1 \leq i \leq n\right\} .
$$
^c-zJQaiPDau9