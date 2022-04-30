# Turingmaschine

Eine **Turingmaschine** $T=(Z,z_0,X,f,g,m)$ ist definiert durch die **Zustandsmenge** $Z$, einem **Anfangszustand** $z_0 \in Z$, dem **Bandalphabet** $X$, der partiellen **Zustandsübergangsfunktion** $f: Z \times X \to Z$, der partiellen **Ausgabefunktion** $g: Z \times X \to X$ und der partiellen **Bewegungsfunktion** $m: Z \times X \to \{-1,0,1\}$.

Die **Konfiguration** $c$ einer Turingmaschine ist ihr eindeutiger Gesamtzustand. Dieser beinhaltet den momentanen Zustand, die Beschriftung des Bands, sowie die Position des Lesekopfes. $c_n(w)$ ist die Konfiguration nach $n$ Schritten mit dem Wort $w$ als Eingabe.

Das **Band** der Turingmaschine ist unendlich lang und ist zunächst mit **Blanksymbolen** gefüllt. Die **Bandbeschriftung** kann als Abbildung $b: \mathbb{Z} \to X$ formalisiert werden.

