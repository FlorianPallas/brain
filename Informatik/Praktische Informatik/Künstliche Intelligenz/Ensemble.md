- Trainiere mehr als einen Regressor / Klassifizierer
- Mittle alle Vorhersagen
- -> Leicht bessere Ergebnisse als jedes einzelne Modell, da Mittelung über verschiedene Vorhersagen
	- Nur wenn Modelle unabhängig
	- Ansonsten aber zumindest gleich gut

## Bagging und Boosting
Wie erreichen wir Unabhängigkeit?
- Bagging
	- Paralleles Training von unabhängigen Modellen
	- Training auf zufällige Subsets der Daten (gezogen mit Zurücklegen)
- Boosting
	- Sequentielles Training von Modellen
	- Fokus auf bisher falsch vorhergesagte Trainingspunkte

## Bias und Varianz
Für $m$ unabhängige Modelle
- Reduktion der Varianz auf $1/m$
- Bias bleibt unverändert
