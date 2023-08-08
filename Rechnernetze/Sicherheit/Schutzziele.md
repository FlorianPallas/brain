Kategorisiert in CIA:
- Confidentiality (Vertraulichkeit)
- Integrity (Integrität)
- Availability (Verfügbarkeit)

Auch wichtig:
- Authentizität
- Privatsphäre
- (Nicht-)Abstreitbarkeit

## Vertraulichkeit
Ein System ist vertraulich wenn es keine unautorisierte Informationsgewinnung ermöglicht.

- Symmetrische oder asymetrische Verschlüsselung

![[Pasted image 20230808153332.png]]

## Integrität
Ein System bewahrt **starke** Integrität, wenn es **nicht** möglich ist Daten unautorisiert zu maipulieren.
Ein System bewahrt **schwache** Integrität, wenn unautorisierte Manipulationen
an Daten **nicht unbemerkt** möglich sind

- Message Authentication Codes (MAC)
- Im Internet nicht möglich -> [[Dolev Yao Angreifer]]

![[Pasted image 20230808153522.png]]

## Authentizität
Unter Authentizität versteht man die manipulationssichere **Identifikation von Instanzen**.
Der Vorgang zur Überprüfung der Authentizität wird als Authentifizierung bezeichnet

- Echtheit von Instanzen
	- Gesprächspartner, Server, Access Point
- Echtheit von Daten
	- Daten wirklich vom korrekt Sender
- Zertifikate, digitale Signatuen, gemeines Geheimnis