---
layout: post
title: "ArithmeticProgression"
date: 2020-11-23 17:21:01 +0100
categories: [math, loop, interactive]
level: 8
---

Scrivi il programma `ArithmeticProgression` utile per calcolare i termini di una progressione aritmetica. Il programma deve funzionare nel modo seguente:

1. Chiede di inserire il valore del primo termine ($a_1$)
2. Se il valore inserito non è un numero intero stampa il messaggio:
	
		Valore a1 non valido "<valore>" 
	e ricomincia dal punto 1.
3. Chiede di inserire la *ragione* ($r$)
4. Se il valore inserito non è un numero intero stampa: 

		Valore r non valido "<valore>" 
	e ricomincia dal punto 3.
5. Chiede di inserire il numero di termini da stampare (`N`)
6. Se il valore inserito non è un numero intero stampa:
		
		Valore N non valido "<valore>" 
	e ricomincia dal punto 5.
7. Se il valore inserito è inferiore a 1 stampa: 

		Il numero di termini deve essere maggiore di 0 
	e ricomincia dal punto 5.
8. Stampa i primi `N` termini della progressione aritmetica

Esempio 1:

~~~
Inserire primo termine (a1): 1
Inserire ragione (r): 2
Inserire numero di termini (N): 10
1, 3, 5, 7, 9, 11, 13, 15, 17, 19.
~~~

Esempio 2:

~~~
Inserire primo termine (a1): bau
Valore a1 non valido "bau"
Inserire primo termine (a1): 1
Inserire ragione (r): miao
Valore r non valido "miao"
Inserire ragione (r): 2
Inserire numero di termini (N): muhh
Valore N non valido "muhh"
Inserire numero di termini (N): 0
Il numero di termini deve essere maggiore di 0
Inserire numero di termini (N): 5
1, 3, 5, 7, 9.
~~~
