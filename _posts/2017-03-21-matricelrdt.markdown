---
layout: post
title: "MatriceLRDT"
date: 2017-03-21 19:52:56 +0100
categories: [array]
level: 13
---


Ora proviamo a *ribaltare verticalmente* la disposizione dei valori rispetto a quanto fatto nell'esercizio [`MatriceLRTD`]({{ site.baseurl }}{% link _posts/2017-03-21-matricelrtd.markdown %}). Scrivi un programma che:

2. Crea una matrice con le dimensioni definite dall'utente 
3. Riempie la matrice disponendo dei valori crescenti da sinistra a destra, dal basso verso l'alto
4. Stampa lo stato della matrice

Esempio, per una matrice di 5 x 5:

~~~text
20	21	22	23	24	
15	16	17	18	19	
10	11	12	13	14	
5	6	7	8	9	
0	1	2	3	4	
~~~

Il programma deve funzionare correttamente anche per matrici rettangolari. Esempio (7 x 2):

~~~text
12	13	
10	11	
8	9	
6	7	
4	5	
2	3	
0	1		
~~~