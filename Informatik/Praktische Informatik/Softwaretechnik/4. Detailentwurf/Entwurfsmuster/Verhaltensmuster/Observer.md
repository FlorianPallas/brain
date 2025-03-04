---
aliases: []
---

# Observer #card
## Zweck
Benachrichtige sogennante Observer über Zustandsänderungen die sich bei einer gegebenen Klasse zu Laufzeit an- und abmelden können.
## Motivation
Teilt man ein System in eine Menge von interagierenden Klassen auf, so muss die Konsistenz zwischen den miteinander in Beziehung stehenden Objekten aufrechterhalten werden. Eine enge Kopplung dieser Klassen ist nicht empfehlenswert, weil dies die individuelle Wiederverwendbarkeit einschränkt.
## Struktur
![[Pasted image 20220621175053.png]]
![[Pasted image 20220621175135.png]]
## Anwendbarkeit
- Wenn die Änderung eines Objekts die Änderung anderer Objekte verlangt und man nicht weiß, wie viele und welche Objekte geändert werden müssen.
- Wenn ein Objekt andere Objekte benachrichtigen muss, ohne Annahmen über diese Objekte zu treffen.
- Wenn eine Abstraktion zwei Aspekte besitzt, wobei einer von dem anderen abhängt. Die Kapselung dieser Aspekte in separaten Objekten ermöglicht unabhängige Wiederverwendbarkeit.
## Hinweis
Die Botschaft enthält keinen Hinweis was geändert wurde. Ein erweitertes Protokoll kann verwendet werden, um den Observern die konkrete Änderung mitzuteilen.
## Beispiele
![[Pasted image 20220621175208.png]]
^c-eEWOcl7cuJ
---
**Tags**: 