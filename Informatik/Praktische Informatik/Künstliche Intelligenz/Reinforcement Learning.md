- Wiederholte Interaktion mit der Welt
- Optimalitätskriterium
- Aber, anders wie bei MDPs, kein (oder begrenztes) Wissen wie die Welt funktioniert

## Anwendung
- Computerspiele
- Gehen Lernen von Robotern
- LLM Fine Tuning

## RL Agent
- Policy: Behaviour
- Value-Function: Evaluation-function for states and actions
- Model: Agent's representation of the environment

## Taxonomy
![[Pasted image 20250316141943.png]]

Wir können entweder mit Modell agieren

Oder wir können anhand der gesehenen Transitionen die V und Q Methoden schätzen:
- MC
- TD -> TD Learning, Q Learning
Es ist kein Modell nötig!

# Monte-Carlo Schätzung (MC)
Wir können einen Erwartungswert immer durch Stichproben approximieren.
![[Pasted image 20250316142133.png]]
Auch Sample-Average genannt

# Temporal Differences (TD)


# Q-Learning
- Beispiel für TD Learning
- Einer der bekanntesten, und am häufigsten verwendeten RL-Algorithmen
- Konvergiert zu optimaler Strategie, auch wenn (wegen explorieren) nicht immer optimal gehandelt wird!
	- Nur für tabellarischen Fall
	- Es muss aber genügend exploriert werden
	- Jedes Zustands-Aktionspaar muss theoretisch unendlich oft besucht werden

## Exploration vs Exploitation
- Greedy Policy kann bessere Aktionen verpassen
- -> Exploration, um subotimale Aktionen zu explorieren
- Aber wann explorieren? Und wann exploitieren? -> Kernproblem des RL

## Epsilon-Greedy-Policy
- Zufällige Aktion mit Wahrscheinlichkeit $\epsilon$ wählen, ansonsten optimal
![[Pasted image 20250316142813.png]]

## Soft-Max-Policy
- Höhere Q-Value, höhere Wahrscheinlichkeit
- $\beta$ als Temperature
![[Pasted image 20250316142819.png]]

TODO