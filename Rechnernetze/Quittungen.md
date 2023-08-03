---
alias: ['Quittung']
---

## Problem
Woher weiß der Sender dass ein Paket nicht (oder fehlerhaft) beim Empfänger angekommen ist?

## Lösung
Der Empfänger sendet Quittungen um den Sender über den Empfang zu informieren.

## Varianten
- Positive Quittungen (ACK): Der Empfänger quittiert den Empfang
- Negative Quittungen (NACK): Der Empfänger meldet ein nicht-erhalten eines Pakets (z.B. wenn er ein nachfolgendes Paket erhält)
- Selektive Quittungen: Quittung signalisiert den Empfang oder Verlust eines einzelnen Pakets
- Kumulative Quittungen: Quittung signalisiert den Empfang oder Verlust mehrerer Pakete (meist alle Pakete bis zu einem bestimmte Sequenznummer)