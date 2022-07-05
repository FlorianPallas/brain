---
aliases: []
---

# Kontrollflussgraph #card
## Definition
Ein Kontrollflussgraph (engl. control flow graph) eines Programms $P$ ist ein gerichteter Graph G mit
$$
G=\left(N, E, n_{\text {start }}, n_{\text {stopp }}\right)
$$
wobei
- N die Menge der Grundblöcke in P,
- $\mathrm{C} \subseteq \mathrm{N} \times \mathrm{N}$ die Menge der Kanten, wobei die Kanten die Ausführungsreihenfolge von je zwei Grundblöcken angeben (sequentielle Ausführung oder Sprünge)
$\mathrm{n}_{\text {start }}$ der Startblock und
$\mathrm{n}_{\text {stopp }}$ der Stoppblock ist.
## Elemente
- Eine Kante e $\in E$ in einem KFG G wird Zweig (engl. branch) genannt. Zweige sind grundsätzlich gerichtet.
- Pfade im KFG die mit dem Startknoten $\mathrm{n}_{\text {start }}$ anfangen und beim Stoppknoten $\mathrm{n}_{\text {stopp }}$ aufhören heißen vollständige Pfade.
## Kontrollflussgraph finden
1. Schritt: Transformiere in Zwischensprache
2. Schritt: Fasse alle Folgen, die mit einem Sprung enden, zu je einem Grundblock zusammen
3. Schritt: Prüfe, ob Eintritt nur am Anfang
4. Schritt: Teile ggf. auf
## Beispiel
![[Pasted image 20220705143058.png]]
![[Pasted image 20220705142820.png]]
![[Pasted image 20220705142739.png]]
![[Pasted image 20220705142750.png]]
![[Pasted image 20220705142848.png]]
^c-Aj6pfoe7Pe
---
**Tags**: 