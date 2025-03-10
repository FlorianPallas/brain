## Definition

Ist $(\Omega, P )$ ein diskreter Wahrscheinlichkeitsraum und $S \neq \varnothing$ eine beliebige Menge, so wird die Abbildung $X: \Omega \rightarrow S$ auch $S$-wertige Zufallsvariable genannt.

## Verteilung von $X$

Ist $X: \Omega \rightarrow S$ eine Zufallsvariable auf einem [[diskreter Wahrscheinlichkeitsraum]] $(\Omega, P )$, dann wird durch

$$
P ^X(B):= P \left(X^{-1}(B)\right), \quad \forall B \subseteq S,
$$

ein [[diskretes Wahrscheinlichkeitsmaß]] $P ^X$ auf $S$ definiert, welches Verteilung von $X$ genannt wird. $\left(S, P ^X\right)$ ist ein [[diskreter Wahrscheinlichkeitsraum]].

Veranschaulichung für $X: \Omega \rightarrow \mathbb{R}$:
![[CleanShot 2022-11-14 at 13.46.03@2x.png]]

## Notation für Urbilder

$\begin{aligned}\{X \in B\} &:=\{\omega \in \Omega \mid X(\omega) \in B\}=X^{-1}(B) \\\{X=x\} &:=\{\omega \in \Omega \mid X(\omega)=x\}=X^{-1}(\{x\}) \\\{X>x\} &:=\{\omega \in \Omega \mid X(\omega)>x\}=X^{-1}((x, \infty)) \quad(\text { im Fall } S= R ) \end{aligned}$

## Beispiel Indikatorfunktion

![[CleanShot 2022-11-14 at 13.28.07@2x.png]]

## Beispiel Augensumme zweier fairer Würfel

![[CleanShot 2022-11-14 at 13.35.09@2x.png]]

## Unabhänigkeit

Sei $(\Omega, P )$ ein [[diskreter Wahrscheinlichkeitsraum]] und $S_i, i \in\{1, \ldots, n\}$, nichtleere Mengen. Zufallsvariablen

$$
X_i: \Omega \rightarrow S_i, \quad i \in\{1, \ldots, n\},
$$

heißen [[stochastisch unabhänig]], wenn für beliebige $B_i \subseteq S_i, i \in\{1, \ldots, n\}$, die Ereignisse

$$
\left\{X_1 \in B_1\right\}, \ldots,\left\{X_n \in B_n\right\}
$$

stochastisch unabhängig sind. Aka die Urbilder disjunkt sind.

## Satz Unabhänigkeitskriterien

![[CleanShot 2022-11-14 at 15.40.34@2x.png]]
(II) besser verständlich:
![[CleanShot 2022-11-28 at 15.51.58@2x.png]]

## Beispiel Bernoulli-verteilte Zufallsvariablen

![[CleanShot 2022-11-16 at 18.01.00@2x.png]]

## Satz Summe von Bernoulli-verteilten Zufallsvariablen

![[CleanShot 2022-11-16 at 18.06.48@2x.png]]

## Definition: Randverteilung

![[CleanShot 2022-12-05 at 16.16.04@2x.png]]

## Beispiel Randverteilung

![[CleanShot 2022-12-05 at 16.05.33@2x.png]]

## Erwartungswert

![[CleanShot 2022-12-12 at 16.11.33@2x.png]]
