Modellierung des Datenbank Schemas in Tabellen für jede Relation. Beziehungen sind durch Fremdschlüssel abgebildet.

## Ableiten vom [[ER Modell]]
- Relation für jede Identität aus dem Modell erstellen mit den entsprechenden Attributen und primären Schlüsseln.
- Relationen umwandeln
	- 1:1
		- Bei muss-muss Relationen verschmelzen
		- Ansonsten (is-a) Primärschlüssel duplizieren und in beiden Relationen verwenden
		![[Pasted image 20230813164635.png]]
	- 1:n
		- Fremdschlüssel auf n Seite
	- n:m
		- Zwischenrelation einführen, beide Fremschlüssel sind auch Primärschlüssel