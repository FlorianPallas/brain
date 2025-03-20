## Motivation
Das menschliche Gehirn erkennt Bilder auch, indem es das Bild zunächst in Features unterteilt. Das können Kanten, Formen, Objekte, oder Gesichter sein. CNNs ahmen dies nach.

## Datentypen
- 1D
	- Audio
	- Spektral
- 2D
	- Bilddaten, Graustufen
- 2D + Kanäle
	- Farbige Bilder
- 3D+
	- Volumetrische Daten
	- Videodateien
	- ...

## Anwendung
- Krebserkennung Medizin
- Bildklassifizierung

## Vorgehen
- Neuronale Netz, entwickelt für Daten auf Grids (1D, 2D, 3D, ...)
- Eingabe wird mit Kernel abgetastet, was eine neue Ausgabe erzeugt
- Elementweises Produkt von Eingabe und Kernel

## Padding
Beim Falten reduziert sich die Größe. Padding füllt den Input mit 0en auf, damit die Größe gleich bleibt. Stellt auch sicher, dass Randpixel korrekt vom Filter erfasst werden.

### 1D
Padding mit $k+1$, da $Output = m - k + 1$

## Hyperparameter
- Width der Kernels
- Stride: Wie viele Pixel bewegt sich der Kernel
- Pooling Funktion
- Zahl der Layer
- ...

## Pooling
Kombination der Informationen von mehreren Pixel zu einem einzigen.
- Max Pooling: Maximum der Pixel
- Average Pooling: Average
- L2 Pooling: L2 Norm
z.B. zum Downsampling

![[Pasted image 20250316144433.png]]

## Convolutional Layer
Ein Layer der mehrere Operationen verbindet
- Convolution
- Nichtlinearität (Detector)
- Pooling

## CNN Model
Kombination aus
- Convolution Layers
	- Mehrere Filter
	- Nichtlineare Transformationen
	- Pooling
- NN Layers
	- Vektorisierung
	- Dense Layers
	- Softmax (Mehrklassen Klassifizierung)

## Residual Learning
![[Pasted image 20250316145318.png]]
- Korrektur der Eingaben Lernen (anstatt Transformation)
- Informationen werden weitergegeben
- Gelernte Änderungen werden addiert
- Backpropagation: Direkter Pfad von Loss zu jeder Schicht
	- Schnelles Training, trotz Tiefe
- Ermöglicht extreme Tiefe (z.B. 1000 Schichten)

## Transfer Learning
- Erster Schritt: Trainieren mit tiefen CNNs und großen Datenmengen
- Zweiter Schritt: Nur Output Schicht ersetzen, neu trainieren mit neuen Daten
- -> Transfer von Lernen auf neuen Output, mit weniger Daten

## Data Augmentation
Daten werden verformt, skaliert, verschoben, rotiert, gespiegelt, damit das CNN invariant gegenüber diesen Transformation operiert.

## Computer Vision Tasks
![[Pasted image 20250316145717.png]]

## Semantische Segmentierung
Input: Bild
Output: Label pro Pixel

- Pixel einzeln Klassifizieren
	- teilweise unmöglich
- Pixel mit Umgebung
	- immernoch schwer
	- Ineffizient
- Convolutional Layers
	- Konstante Größe, sehr teuer
- Convolutional Layers
	- Downsampling, dann Upsampling
	- Upsampling -> Reverse Convolution, UNet

## Objekterkennung
CNN generiert Vektor
Fully Connected auf 1000 -> Softmax
Fully Connected auf 4 -> Box-Koordinaten

## Fragen
**Was ist ein CNN? Was sind die Komponenten und wie ist es aufgebaut?**
Ein NN das die Daten vorverarbeite um Features aus den Daten zu lesen. Transformationen können als Sparesly Connected Layers gesehen werden.
- Convolutional Layers
- Pooling Layers
- Nicht Lineare Transformationen
- NN Layers

**Wie viele Parameter hat ein convolutional layer mit gegebenen Spezifikationen?**
Convolution: Höhe x Breite x Tiefe x Kernel Anzahl
Pooling: 0
Fully Connected: Inputs x Outputs

**Warum funktionieren fully connected layers für Bild-Tasks nicht?**
Weil einzelne Pixel keinen direkten Einfluss auf den Inhalt des Bildes haben. Bilddaten erfordern das Lernen von Features.

**Welche Hyperparameter hat ein CNN?**
Kernel Größe, Stride, Poolingfunktion, etc.

**Was sind residual connections und wofür werden sie verwendet?**
Zwischen CNN Schichten, werden Verbindungen gezogen. Somit ist jeder Layer direkt mit dem Loss verbunden. So können deutlich tiefere CNNs trainiert werden.

**Was ist Transfer Learning?**
Es wird zunächst ein tiefes CNN mit viele Daten trainiert. Danach wird der Output Layer ersetzt, und nur dieser mit neuen Daten trainiert. So kann auch mit wenig Daten, der Lerneffekt des großen Datensatzes auf eine neue Aufgabe übertragen werden. 

**Was ist data augmentation? Was sind Invarianten in diesem Kontext?**
CNN Input Daten werden skaliert, rotiert, gespiegelt, etc. um den Datensatz diverser zu machen. So kann das CNN auch mit nicht-perfekten Daten umgehen.

**Was sind mögliche Computer Vision Tasks?**
Objekterkennung, Klassifikation, Semantische Segmentierung,  Instanz Segmentierung

**Was ist semantische Segmentierung?**
Ein Bild wird in seine Elemente zerlegt. z.B. Hintergrund, See, Eisbär, Pinguin.

**Was ist das U-Net und wofür wird es verwendet?**
U-Net wird für Upsampling Tasks verwendet z.B. zur Segmentierung. Upsampling ist dabei quasi "reverse convolution".

**Wie funktioniert Objekterkennung?**
Der Output eines CNN wird mit einem Fully Connected Layer entweder auf einen Vektor für Softmax, oder zu Box-Koordinaten gemapped.