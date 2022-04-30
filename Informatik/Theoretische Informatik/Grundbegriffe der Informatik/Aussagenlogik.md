# Aussagenlogik
---

**Formeln** sind Variablen, verbunden mit Konnektiven. Als **Konnektive** bezeichnet man die vier Symbole $\land$, $\lor$, $\lnot$ und $\rightarrow$ . **Variablen** sind Platzhalter, welche die Werte "wahr" oder "falsch" annehmen können.

Das **Alphabet** der Aussagenlogik ist definiert als $A_{AL}=\{(,),\land,\lor,\lnot,\rightarrow\} \cup Var_{AL}$. Es beinhaltet Symbole zur Klammerung, die Konnektive und alle Variablen.

Die formalen **Sprache** $For_{AL}$ beinhaltet alle syntaktisch korrekten Formeln. Dabei ist $For_{AL} \subseteq A_{AL}^*$.

Die Konnektive als Funktion dargestellt lauten:

![[assets/Pasted image 20220222135859 1.png]]

Eine **Interpretation** einer Menge an Variablen ist eine Abbildung $I:V \to \mathbb{B}$. Die Menge aller Interpretationen einer Variablenmenge ist also $\mathbb{B}^V$.

Hier beispielsweise alle Interpretationen der Variablenmenge $V=\{P_1,P_2,P_3\}$.

![[assets/Pasted image 20220222140318 1.png]]

Eine Interpretation legt eine **Auswertung** $val_I(F)$ fest. 

Besitzen zwei Formeln für alle Interpretationen die gleiche Auswertung, so sind sie **äquivalent**. Man schreibt $G \equiv H$.

Eine Interpretation ist ein **Modell** einer Formel, wenn $val_I(G) = {wahr}$ ist. Ist eine Interpretation Modell von zwei verschiedenen Formeln zugleich, so schreibt man $G \models H$.

Ist eine Formel allgemein gültig (**Tautologie**), so schreibt man $\models G$.

Eine Formel ist erfüllbar wenn es mindestens eine Interpretation gibt, sodass $var_I(G) = {wahr}$.

