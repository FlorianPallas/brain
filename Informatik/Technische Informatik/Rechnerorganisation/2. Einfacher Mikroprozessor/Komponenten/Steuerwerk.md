## Definition

- Holt die Befehlt eines Programms aus dem Speicher
- Dekodiert die Befehle
- Steuert ihre Ausführung in der verlangten Reihenfolge mittels Steuer- und Status-Signalen
  ![[CleanShot 2022-11-14 at 15.53.51@2x.png]]

## Bestandteile

### Taktgenerator

- Erzeugen des Taktsignals gemäß der Taktfrequenz
- Erzeugen eines mit dem Prozessortakt synchronisierten Rücksetzsignals (RESET) - Zurücksetzen / Initialisierung des Prozessors - Erzeugen eines definierten Anfangszustands

### Befehlsregister

- Enthält den gerade auszuführenden Befehl
- Kann aus mehreren Registern bestehen (z.B. Variables Befehlsformat: die Befehle sind unterschiedlich lang)

### Steuerung

#### Decoder

- Entnimmt den obersten vordecodierten Befehl aus dem Befehls-FIFO
- Ermittelt die Startadresse des zugehörigen Mikroprogramms

#### Mikrobefehls-Steuerung

- Synchrones Schaltwerk
- erzeugt die Steuersignale, interpretiert die Meldesignale

#### Zeit-Steuerung

- Synchronisiert die erzeugten Steuersignale mit dem Systemtakt

### Steuerregister

- Mit Hilfe des Steuerregisters kann die aktuelle Arbeitsweise des Steuerwerks beeinflusst werden
- Es können bestimmte Arbeitsmodi für den Prozessor festgelegt werden (User-Modus, Systemmodus)

## Mikroprogrammiertes Steuerwerk

- Jeder Maschinenbefehl wird durch ein Mikroprogramm implementiert
- Ein Mikroprogramm besteht aus einer Folge von Mikrobefehlen
- Jedes Mikroprogramm ist im Mikroprogrammspeicher abgelegt
- Jeder Mikrobefehl fasst die Mikrooperationen (Steuersignale) zusammen
  ![[CleanShot 2022-11-14 at 16.32.03@2x.png]]
