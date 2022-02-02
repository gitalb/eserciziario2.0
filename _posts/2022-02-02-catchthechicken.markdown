---
layout: post
title: "CatchTheChicken"
date: 2022-02-02 12:29:44 +0100
categories: [wrapper,args,switch]
level: 9
---

Devi aiutare il fattore John a catturare la sua gallina. Il fattore e la gallina si trovano in un campo di 3 righe e tre colonne.

Il tuo programma riceve 4 numeri interi come argomenti da linea di comando, nell'ordine:

- la coordinata della riga in cui si trova il fattore
- la coordinata della colonna in cui si trova il fattore
- la coordinata della riga in cui si trova la gallina
- la coordinata della colonna in cui si trova la gallina

La cella in alto a sinistra si trova alla riga `0` e alla colonna `0`:

```
👷🍃🍃
🍃🍃🍃
🍃🍃🍃
```

La cella in basso a sinistra si trova alla riga `2` e alla colonna `0`:

```
🍃🍃🍃
🍃🍃🍃
👷🍃🍃
```
La cella in basso a destra si trova alla riga `2` e alla colonna `2`:

```
🍃🍃🍃
🍃🍃🍃
🍃🍃👷
```

Il tuo programma deve stampare la direzione in cui il fattore si deve spostare per prendere la gallina:

- `\"N\"`: NORD, il fattore si sposta verso l'alto
- `\"S\"`: SUD, il fattore si sposta verso il basso
- `\"W\"`: WEST, il fattore si sposta verso sinistra
- `\"E\"`: EAST, il fattore si sposta verso destra

## Esempio

Se gli argomenti forniti sono `[1,1,0,1]` significa che il fattore si trova al centro del campo (riga `1`, colonna `1`) e la gallina si trova nella riga in alto (`0`) e nella colonna centrale (`1`):

```
🍃🐔🍃
🍃👷🍃
🍃🍃🍃
```

La gallina si trova sopra al fattore, per catturarla il fattore dovrà spostarsi verso NORD, quindi il tuo programma deve stampare `\"N\"`.

