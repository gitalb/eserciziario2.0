---
layout: post
title: "MatriceRLTD"
date: 2017-03-21 19:48:39 +0100
categories: [array]
level: 13
---

Ora proviamo a *ribaltare orizzontalmente* la disposizione dei valori rispetto a quanto fatto nell'esercizio [`MatriceLRTD`]({{ site.baseurl }}{% link _posts/2017-03-21-matricelrtd.markdown %}). Scrivi un programma che:

1. Chiede all'utente di introdurre il numero di righe e il numero di colonne di una matrice
2. Crea una matrice con le dimensioni definite dall'utente 
3. Riempie la matrice disponendo dei valori crescenti da destra a sinistra, dall'alto verso il basso.
4. Stampa lo stato della matrice

Esempio, per una matrice di 5 x 5:

~~~text
Inserire numero di righe: 5
Inserire numero di colonne: 5

4	3	2	1	0	
9	8	7	6	5	
14	13	12	11	10	
19	18	17	16	15	
24	23	22	21	20	
~~~

Il programma deve funzionare correttamente anche per matrici rettangolari. Esempio:

~~~text
Inserire numero di righe: 7
Inserire numero di colonne: 2

1	0	
3	2	
5	4	
7	6	
9	8	
11	10	
13	12	
~~~