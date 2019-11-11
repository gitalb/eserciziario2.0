---
layout: post
title: "CalcolatoreMedia"
date: 2019-03-05 13:54:33 +0100
categories: [wrapper, loop]
level: 8
---

Scrivi il programma `CalcolatoreMedia` che calcola la media di tutte le note valide passate come argomenti da linea di comando (scarta quelle non valide) e la stampa arrotondandola al decimo di punto più vicino.

```text
java CalcolatoreMedia 1.72 4.21 5 -2 cane 6

Nota 1:     1.72
Nota 2:     4.21
Nota 3:     5.0
Nota 4:     6.0
----------------
Media:      4.2   
```
Opzione: Stampare anche gli elementi scartati separati da virgole (`','`). Esempio:

```text
java CalcolatoreMedia 1.72 4.21 5 -2 cane 6

Nota 1:     1.72
Nota 2:     4.21
Nota 3:     5.0
Nota 4:     6.0
----------------
Media:      4.2   

Argomenti scartati: -2, cane
```
