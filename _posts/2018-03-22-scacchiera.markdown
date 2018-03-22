---
layout: post
title: "Scacchiera (non interattivo)"
date: 2018-03-22  6:23:49 +0100
categories: [array, loops]
level: 10
---

Scrivi il programma `Scacchiera` che, dati due numeri interi forniti come argomenti da linea di comando che rappresentano il numero di righe e il numero di colonne di una matrice:

1. Crea una matrice con le dimensioni definite dall'utente 
2. Riempie la matrice disponendo i valori `1` e `0` altrenati come su una scacchiera.

Esempio, per una matrice 5 x 5:

~~~text
java Scacchiera 5 5
0 1 0 1 0 
1 0 1 0 1 
0 1 0 1 0 
1 0 1 0 1 
0 1 0 1 0
~~~

Il programma deve funzionare correttamente anche per matrici rettangolari. Esempio:

~~~text
java Scacchiera 6 8
0 1 0 1 0 1 0 1 
1 0 1 0 1 0 1 0 
0 1 0 1 0 1 0 1 
1 0 1 0 1 0 1 0 
0 1 0 1 0 1 0 1 
1 0 1 0 1 0 1 0
~~~