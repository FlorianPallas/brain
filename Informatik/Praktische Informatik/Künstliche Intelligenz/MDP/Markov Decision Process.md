Nützlich wenn Zustandsübergänge des Modells nicht sicher sind (z.B. Blackjack). Bei voller Kontroller werden stattdessen [[Suchalgorithmen]] verwendet.


# Expectimax Suche
Unsicherheit trotzdem als Suchbaum darstellen mit Zufallsknoten. Diese gewichten ihre Werte nach dem Erwartetem Ergebnis.

Teilbäume können immer wieder auftreten. Viele sinnlose Berechnungen -> MDPs

## Markov Decision Processes (MDPs)
- Eine Menge Zustände $s \in S$
- Eine Menge Aktionen $a \in A$
- Eine Transitionsverteilung $p(s'|s,a)$
	- Wahrscheinlichkeit, dass a von s nach s' führt
	- Auch Modell oder Dynamik genannt
- Eine Belohnungsfunktion $r(s,a)$
- Außerdem
	- Eine Verteilung $\mu_0(s)$ über den Startzustand
	- Eine optionale Liste an Endzuständen

Ziel: Belohnungssumme maximieren

## Warum Markov?
Ergebnisse der Aktionen hängen nur vom aktuellen Zustand, nicht von der Vergangenheit ab.

## Policies
Eine Policy $\pi*: S \to A$ gibt eine Aktion für einen Zustand vor. Eine optimale Policy maximiert den erwarteten Reward.

- Stochastisch
- Deterministisch

## Agent Sucht nach optimaler Policy
$\gamma$ Discount Faktor definiert, wie kurzfristige (nahe 0) oder langfristige (nahe 1) Rewards gewichtet werden.

## Value Iteration
- Um den optimalen Value im Zustand s zu erreichen, müssen wir auch in den Folgezuständen optimal handlen -> Sehr tiefe Berechnungen notwendig
- Nur die nächsten $k$ Schritte betrachen

## Algorithmus
- Init: $V_0^\pi(s) = 0$
- Repeat: $V_k^* = max(r(s,a) + \gamma \sum_{s'} p(s'|s,a) V_{k-1}^*(s'))$ until convergence
	- Maximiere erwarteten Reward über alle $k$ Schritte
- Komplexität jeder Iteration: $O(S^2A)$

## Optimale Policy
Die optimale Policy, ist die Aktion im Zustand s für die der Erwartete Reward der zukünftigen Schritte maximal ist. Diese bleibt konstant für einen Zustand s, und kann daher auch gespeichert werden.

## Q-Values
$Q^*(s,a) =$ erwarteter summierter Reward wenn bei s Aktion a ausgeführt wird, und danach optimal gehandelt wird.

## Gotchas
Geht nur für diskrete Systeme, aber Welt ist nicht diskret.
Geht nur für Lineare System, Quadratische Belohnung, Gaußsches Rauschen (LQR), aber Welt ist nicht linear.
Ansonsten: Näherungswerte verwenden