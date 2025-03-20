# Variablenbasierte Modelle
In manchen Anwendungen gibt es keine Aktionen und die Reihenfolge ist nicht wichtig. Dies als Suchproblem darzustellen ist sehr ineffizient.
z.B. Sudoku, Zustandsschätzung

# Bayes'sche Netzwerke
Probleme mit probabilistischen Abhängigkeiten
z.B. Sensordaten -> Position eines Autos

## Vorteile
- Framework für probabilistisches Schlussfolgern
- Umgang mit heterogen fehlenden Informationen
- Einbeziehung von Vorwissen (z.B. physikalische Gesetze)
- Kann die Variablen aller Zeitschritte interpretieren

## Bayes Regel
$$
p(A|B) = \frac{p(B|A)p(A)}{p(B)}
$$
- Umkehrung der bedingten Wahrscheinlichkeit

### Mit Hintergrund $x$
$$
p(z|y,x) = \frac{p(y|z,x)p(z|x)}{p(y|x)}
$$

## Netze
- DAG, häufig Grafisch dargestellt
- Elternknoten durch Kanten angezeigt
- Beobachtete Variablen grau
- Wahrscheinlichkeit eines Knoten, ist das Produkt der bedingten Wahrscheinlichkeiten der Eltern

![[Pasted image 20250317133618.png]]
Gemeinsame Verteilung: $$p(E,B,A) = p(E)p(B)p(A|B,E)$$

# Hidden Markov Modell (HMM)
- Anfangsverteilung $p(z_0)$
- Transitionsmodell $p(z_{t+1}|z_t)$
- Beobachtungsmodell $p(y_t|z_t)$
Bei kontinuierlichen Zuständen auch Zustandsraummodell genannt.