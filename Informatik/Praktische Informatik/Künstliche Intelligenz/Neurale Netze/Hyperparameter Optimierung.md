Hyperparameter sind Parameter die vor dem Trainieren festgelegt wurden (z.B. Regularisierung, oder Lernrate). Diese können auch optimiert werden.

Warum geht das nicht auf den Trainingsdaten?
Größere Modellkapazität -> Kleinere Trainingsfehler -> Würde z.B. gegen Regularisierung arbeiten

Deshalb splitten wir unsere Daten ein weiters mal: 60% Training, 20% Validierung, 20% Test
Optimieren der Hyperparameter auf Validationsdaten.
