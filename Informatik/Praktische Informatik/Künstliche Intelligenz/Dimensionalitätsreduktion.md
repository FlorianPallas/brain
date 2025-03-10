Ziel von Dimensionalitätsreduktion ist die "Struktur" der Daten zu finde. Dabei reiht sich diese Lernmethode in die Kategorie des unüberwachtem Lernen ein. Labeling der Daten ist also nicht notwendig.
![[Pasted image 20250310145913.png]]

Warum ist Reduktion hilfreich?
Wir arbeiten oft mit sehr vielen, hoch-dimensionalen Daten. Die Effizienz der Lernalgorithmen hängt maßgeblich mit der Dimension zusammen. Daher ist eine Reduktion der Dimension eine Effizienzsteigerung für viele Algorithmen. Wir reduzieren die Daten auf ihre wesentlichen Merkmale.

Was bedeutet Dimensionalitätsreduktion?
Wir versuchen einen niedrig-dimensionalen Unterraum zu finden, mit dem die wesentliche Struktur der Daten weiterhin als Linearkombination dargestellt werden kann. -> Hauptkomponentenanalyse / Principle Component Analysis (PCA)

Was ist die Projektion eines Vektors?
Was mach eine Reduktion gut?
Was sind die Hauptkomponenten in den Daten und wie ist die Beziehung zur Kovarianzmatrix?

## Hauptkomponentenanalyse (PCA)

![[Pasted image 20250310150730.png]]

- PCA projiziert die Daten in einen linearen Unterraum
- PCA maximiert die Varianz der Projektion
- PCA minimiert den Fehler der Rekonstruktion

Eigenwerte / Eigenvektoren der Kovarianzmatrix

- Der größte Eigenwert gibt uns die maximale Variant
- Der entsprechende Eigenvektor gibt uns die Richtung der maximalen Varianz

### Vorgehen

- Zentriere die Daten um den Mittelwert
  - Mittelwert berechnen und von Daten abziehen
- Berechne und zerlege die Kovarianzmatrix, wähle die ersten $M$ größten Eigenwerte und entsprechenden Eigenvektoren
- Die resultierende Eigenbasis ist Grundlage für die Darstellung der Daten
  - Projektion auf nieder-dimensional: $z_i = W^T(x_i - \mu)$
  - Re-Projektion auf hoch-dimensional: $\tilde{x} = \mu + W z_i$
  - mit $W = [u_1, \dots, u_M]$ und $\mu$ der Mittelpunkt

### Optimieren von $M$

Größere $M$ sind näher an der originalen Dimension $D$, und damit genauer. Wir wollen aber ein möglichst kleines $M$, ohne die Struktur der Daten zu verlieren.

- Wähle $M$ so klein, wie die Anwendung der Daten damit funktioniert
- Wähle $M$ so, dass die Eigenbasis einen bestimmten Teil der Varianz erfasst (z.B. $\eta = 0.9$)

### Anwendung

Eine der ersten Anwendungen von PCA, war Gesichtserkennung. Mittels PCA können Bilder von Gesichtern in ihre Merkmale zerlegt werden. Durch Rekonstruktion können auch die Merkmale von Bilder angepasst werden.

![[Pasted image 20250310152242.png]]

## Autoencoder (AE)

![[Pasted image 20250310152705.png]]
Autoencoder sind [[Neurales Netzwerk|Deep Neural Networks]] die darauf ausgelegt sind, ihre Eingabe, insbesondere Bilder, zu reproduzieren. Sie werden mittels [[Back Propagation]] trainiert.

Encoder komprimieren die Eingabe. Decoder rekonstruieren die Eingabe. Dabei versucht AE, dass die Rekonstruktion möglichst nah an der Eingabe liegt. Zwischen Encoder und Decoder entsteht ein Bottleneck, was das Netzwerk zwingt die Struktur der Daten zu lernen.

### Autoencoder vs PCA

- PCA kann nur linear Kombinationen
- PCA ist leicht und effizient zu berechnen
- AE kann nicht-lineare Abhängigkeiten lernen
- AE kann Faltschichten (Convolutions) anwenden
- Wenn nur eine lineare Schicht für Encoder und Decoder verwendet werden, sind AE und PCA sehr ähnlich

### Selbsüberwachtes Lernen

Da AE versucht seine Eingaben zu Rekonstruieren, kann AE sich selbst prüfen und verbessern.

### Anwendung

- Rauschunterdrückung
- Merkmale extrahieren
  - Als neue Eingabe für überwachten Algorithmus
- Bildsuche
  - Bilder können anhand ihrer komprimierten Darstellung besser verglichen werden.
- Imputation fehlender Werte
  - Fehlende Werte im Datensatz ausgleichen
- Bildeinfärbung
  - Schwarz-weiß Bilder wieder Farbe verleihen
- Entfernen von Wasserzeichen
- Erkennen von Anomalien
  - Wenn der Rekonstruktionsfehler groß ist, ist es ein außergewöhnliches Beispiel.

## Clustering

![[Pasted image 20250310153516.png]]Das Ziel von Clustering Algorithmen ist es eine Menge von Objekten so zu gruppieren, dass die zugewiesenen Klassen zueinander ähnlich sind.

Achtung: Clustering ist subjektiv! Daten können meist in verschiedene Klassen eingeordnet werden (z.B. Farbe, Distanz). Die "Richtige" Lösung ist meistens nicht bekannt -> Metriken geben Richtung vor

### Entfernunsmetrik

$d(x,y) = ||x-y|| = \sqrt{(\sum^{d}_{k=1} (x_k - y_k)^2)}$
Wenn die Einheiten unterschiedlich sind, müssen diese vorher normalisiert werden.

### K-Means-Clustering

Der K-Means-Algorithmus definiert Zentroide $C$ zu den Daten $D$, anhand dessen der globale Fehler $SSD$ der Daten berechnet werden kann. Jeder Datenpunkt wird mit seinem nächsten Zentroid verglichen. Die quadrierte Distanz wird auf den Fehler addiert. Es gilt diesen Fehler zu minieren.

$$
SSD(C,D) = \sum^{n}_{i=1} d(x_i,c(x_i))^2
$$

1. Wähle beliebige Clusterzentren
2. Jeder Datenpunkt dem nächstgelegenden Zentroid zuordnen
3. Anpassung der Zentoride an den Mittelwert der zugewiesenen Datenpunkte
4. Schritt 2 wiederholen bis keine Änderung mehr erfolgt

### Konvergiert K-Means?

Ja, aber nur lokal! Es wird kein globales Maximum gefunden. Die Lösung hängt von dem Startpunkt der Zentren ab!

### K-Means++

Alternativ können Zentren iterativ hinzugefügt werden, wobei die Distanz zu anderen Zentren maximiert wird.

1. Wähle zufälligen Datenpunkt als erstes Zentrum
2. Finde den Datenpunkt der von allen Zentren am weitesten entfernt ist
3. Wähle diesen Datenpunkt als neue Zentrum
4. Wiederhole Schritt 2 und 3 bis die gewünschte Anzahl der Zentren erreicht ist.

### Wie wähle ich $K$?

- Holdout Set / Cross Validation ist teuer
- Knee-finding, heuristisch, billig
  - $K$ langsam erhöhen bis $SSD$ nicht weiter sinkt

### Fazit

- Stärken
  - K-means konvergiert schnell
  - K-means++ findet eher ein globales Minimum
    - Alternativ mehrmals verschieden Initialisieren
- Schwächen
  - Mittelwert muss definiert sein
    - Was ist mit kategorischen Daten?
  - Verrauschte Daten nicht zu verarbeiten
  - Cluster sind immer konvex in der Form
