---
aliases: []
---

# Hauptraum #card
## Definition
Ist $q \leq n$ die kleinste natürliche Zahl mit $K_{q}=K_{q+1}$, so heißt
$$
H_{\lambda}:=K_{q}=\operatorname{Kern}\left(\left(f-\lambda \operatorname{id}_{V}\right)^{q}\right)
$$
Hauptraum (oder verallgemeinerter [[Eigenraum]]) von $f$ zum [[Eigenwert]] $\lambda$; $q$ heißt Index von $H_{\lambda}$. Hinweis: $K_q$ ist der [[j-te Kern|q-te Kern]] 
## Bemerkung
- Bemerkung 1.6. Für den Untervektorraum $H_{\lambda}$ von $V$ ist der Endomorphismus $g: H_{\lambda} \rightarrow H_{\lambda,} \quad v \mapsto\left(f-\lambda \mathrm{id}_{V}\right)(v)$ nilpotent, das heißt es gibt $m \in \mathbb{N}$ mit $g^{m}=0$.
- Der Hauptraum besitzt folgendes [[f invariant|f invariantes]] Komplement: $B_{\lambda}:=\operatorname{Bild}\left(\left(f-\lambda \mathrm{id}_{V}\right)^{q}\right)$. Somit gilt $V=H_{\lambda} \oplus B_{\lambda}.$
## Berechnung
Gegebenenfalls muss zuerst der [[Eigenwerte]] bestimmt werden. Dieser wird mit dem [[charakteristisches Polynom|charakteristischen Polynom]] bestimmt. Nach den Eigenschaften der [[j-te Kern|j-ten Kernen]] gilt: $K_q = K_n$. Somit kann für die Ermittlung des Hauptraums [[Lineares Gleichungssystem|LGS]], das direkt aus der Definition folgt gelöst werden: $$\operatorname{Kern}\left(\left(f-\lambda \operatorname{id}_{V}\right)^{n}\right)$$Dies ist aber sehr umständlich da die $n$-te Potenz der [[Matrix]] bestimmt werden muss. Folglich ist es angenehmer die Kerne $K_1=E_1, \quad K_2, \quad ... \quad$ sukzessive zu bestimmen, bis $K_{q+1}=K_q$ erfüllt ist.
^c-V8tCPcxpqs
---
**Tags**: #todo 