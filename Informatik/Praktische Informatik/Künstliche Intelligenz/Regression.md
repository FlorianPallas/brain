- Daten in Trainings- und Testdaten aufteilen
- Trainiere auf Trainingsdaten
- Prüfe auf Testdaten

- Minimiere Fehler in den Trainingsdaten
- Minimiere Lücke zwischen den Trainings- und Testdaten

#### Bias
Bias ist die Ausgabe wenn alle Feature Inputs 0 sind. Dieser kann entsprechend berechnet und angepasst werden.

### Generalisierung
Das Modell soll nicht nur für das Testset gute Ergebnisse liefern, sondern mit ungesehenen Daten zurecht kommen.

### Underfitting
Großer Fehler auf Trainingsdaten
Das Modell kennt den Zusammenhang zwischen Input und Output noch nicht genügend.
z.B. Zufallsdaten
### Overfitting
Große Lücke zwischen Trainings- und Testfehler
Das Modell hält zu stark an den Trainingsdaten fest. Es kann nicht auf ungesehene Daten reagieren.
z.B. Trainingsset auswendig gelernt
### Kapazität
Beschreibt die Möglichkeit eines Modells, viele unterschiedliche Funktionen zu beschreiben. z.B. Grad der Funktion (z.B. linear vs quadratisches Polynom)

Niedrige Kapazität -> Tendenz zu Underfitting
Hohe Kapazität -> Tendenz zu Overfitting

### Regularisierung
Methoden um Overfitting zu verhindern.

Hohe Weights von einzelnen Inputs signalisieren eine potenziell unnatürliche Abhängigkeit zu den Trainingsdaten. Im Idealfall wollen wir kleine Gewichte.

Um Overfitting zu verhindern addieren wir die Summe der Gewichte auf den Fehler des Modells. Somit bestrafen wir das Modell für Overfitting. Die Stärke dieses Faktors kann variiert werden.

### Loss Funktionen
Die Loss Funktion definiert das Fehlermaß des Modells, und ist daher maßgeblich an dem Lernerfolg beteiligt. Meist wird der [[Mean Squared Error]] verwendet.

L1 Loss -> [[Mean Absolute Error|MAE]]
L2 Loss -> [[Mean Squared Error|MSE]]
Huber Loss -> Kombination: Quadratisch um 0, dann linear

L1 ist robuster gegen Ausreißer, hat aber Probleme bei kleinen Fehlern im Konvergieren.


### Accuracy
Beschreibt wie viele richtige Vorhersagen das Modell produziert. Ähnlich zu Spezifität und Sensitivität, oder Precision und Recall.

$$ACC = \frac{TP + TN}{P + N}$$
![[Pasted image 20250303165545.png]]

Wenn wir den Schwellwert für eine Klassifikation variieren können:
- Receiver Operator Curve
- Area Under Curve

![[Pasted image 20250303165724.png]]