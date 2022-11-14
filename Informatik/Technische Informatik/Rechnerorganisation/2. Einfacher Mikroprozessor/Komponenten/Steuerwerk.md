## Definition #card
- Holt die Befehlt eines Programms aus dem Speicher
- Dekodiert die Befehle
- Steuert ihre Ausführung in der verlangten Reihenfolge mittels Steuer- und Status-Signalen
![[CleanShot 2022-11-14 at 15.53.51@2x.png]]
^c-ZJyrMw8mqC

## Bestandteile
### Taktgenerator #card 
- Erzeugen des Taktsignals gemäß der Taktfrequenz
- Erzeugen eines mit dem Prozessortakt synchronisierten Rücksetzsignals (RESET) - Zurücksetzen / Initialisierung des Prozessors - Erzeugen eines definierten Anfangszustands
^c-fQ9ckS8c6w
### Befehlsregister #card 
- Enthält den gerade auszuführenden Befehl
- Kann aus mehreren Registern bestehen (z.B. Variables Befehlsformat: die Befehle sind unterschiedlich lang)
^c-O6tdAGENui
### Steuerung #card 
#### Decoder
- Entnimmt den obersten vordecodierten Befehl aus dem Befehls-FIFO
- Ermittelt die Startadresse des zugehörigen Mikroprogramms
#### Mikrobefehls-Steuerung
- Synchrones Schaltwerk
- erzeugt die Steuersignale, interpretiert die Meldesignale
#### Zeit-Steuerung
- Synchronisiert die erzeugten Steuersignale mit dem Systemtakt
^c-pjyTOQk6zD
### Steuerregister #card 
- Mit Hilfe des Steuerregisters kann die aktuelle Arbeitsweise des Steuerwerks beeinflusst werden 
- Es können bestimmte Arbeitsmodi für den Prozessor festgelegt werden (User-Modus, Systemmodus)
^c-xsu9BHxBzz