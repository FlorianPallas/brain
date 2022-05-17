---
aliases: []
---

# Disjunktive Normalform #card
## Definition
Es sei eine [[Boolesche Funktionen|Booleschen Funktion]] $y\left(x_{1}, \ldots, x_{n}\right)$ gegeben. Ein Boolescher Ausdruck heißt disjunktive Normalform (Abk.: DNF) der Funktion y, wenn er aus einer disjunktiven Verknüpfung von [[Minterm|Mintermen]] $K_{i}$ besteht:
$$
y=K_{0} \vee K_{1} \vee \cdots \vee K_{k} \quad, k \leq 2^{n}-1
$$
Dabei darf es keine zwei Konjunktionen $K_{i}, K_{j}$ mit $i \neq j$ geben, die zueinander äquivalent sind.
## Beispiel
- $f(a, b, c)=a b c \vee a \bar{b} c \vee \bar{a} \bar{b} \bar{c} \vee \bar{a} \bar{b} c$ ist ein Ausdruck in disjunktiver Normalform.
- $f(a, b, c)=a b c \vee a \bar{b} \vee c a b \vee a(b c \vee \bar{b} \bar{c})$ ist aus drei Gründen kein Ausdruck in disjunktiver Normalform:
	- $a \bar{b}$ ist kein [[Minterm]], da nicht alle auftretenden Variablen enthalten sind,
	- $a b c$ und $c a b$ sind äquivalent und
	- $a(b c \vee \bar{b} \bar{c})$ ist kein Produktterm.
## Eigenschaft
- Die disjunktive Normalform ist bis auf Vertauschung der Disjunktionen eindeutig.
^c-6l8HxhArCV
---
**Tags**: 