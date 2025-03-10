## Definition

Eine Folge $\left(a_n\right)$ heißt konvergent

$$
: \Longleftrightarrow \exists a \in R :\left\{\begin{array}{l}
\text { Zu jedem } \varepsilon>0 \text { existiert ein } n_0=n_0(\varepsilon) \in N \text { so, } \\
\text { daß für jedes } n \geq n_0 \text { gilt }:\left|a_n-a\right|<\varepsilon .
\end{array}\right.
$$

In diesem Fall heißt a Grenzwert $(G W)$ oder Limes von $\left(a_n\right)$ und man schreibt

$$
a_n \rightarrow a(n \rightarrow \infty) \text { oder } a_n \rightarrow a \text { oder } \lim _{n \rightarrow \infty} a_n=a \text {. }
$$

## Äquivalente Definitionen

$\begin{aligned} a_n \rightarrow a(n \rightarrow \infty) & \Longleftrightarrow \forall \varepsilon>0 \exists n_0 \in N \forall n \geq n_0: a_n \in U_{\varepsilon}(a) \\ & \Longleftrightarrow \forall \varepsilon>0 \text { gilt: } a_n \in U_{\varepsilon}(a) \text { ffa } n \in N \\ & \Longleftrightarrow \forall \varepsilon>0 \text { gilt: } a_n \notin U_{\varepsilon}(a) \text { für höchstens endlich viele } n \in N \end{aligned}$

## Eigenschaften/Kriterien

- Eine [[Mathematik/Analysis/1. Folgen/Konvergenz/Konvergenz|konvergente]] Folge ist stets [[beschränkte Folge|beschränkt]] #relation
- Monotoniekriterium: Eine [[Monotonie (Folgen)|monoton wachsende]] (bzw. fallende) und [[nach oben beschränkte Folge]] (bzw. nach unten beschränkte) ist konvergent. #relation
- Cauchykriterium: Eine Folge ist konvergent, genau dann wenn sie eine [[Cauchyfolge]] ist. #relation

## Beweisführung anhand eines Beispiels

![[CleanShot 2022-11-09 at 08.32.57@2x.png]]

## Beweisführung für rekursive Folgen

0. Ersten paar Folgenglieder ausrechnen um die Folge besser kennenzulernen
1. Folge auf mögliche Grenzwerte überprüfen ("Fixpunktgleichung"). Ansatz: $\lim_{n \to \infty} a_n = A = \lim_{n \to \infty} a_{n+1}$
2. Monotonie zeigen (manchmal hilft es davor schon die Beschränktheit zu zeigen und dann abzuschätzen)
3. Beschränktheit mittels [[Beweisverfahren durch vollständige Induktion]] zeigen
4. Teilschritte vereinigen

## Beweisführung für rekursive Folgen Beispiel

![[CleanShot 2022-11-20 at 11.18.22@2x.png]]

## Rechentipps

- $|a_n-a|$ kann nach oben abgeschätzt werden

## Rechenregeln

![[CleanShot 2022-11-10 at 14.07.05@2x.png]]

## Beispiel: Sandwichteorem für $a_n = \sqrt[n]{3^n+1}$

![[CleanShot 2022-11-20 at 11.20.38@2x.png]]
