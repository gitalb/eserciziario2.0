---
layout: post
title: "SimpleInterest"
date: 2020-11-23 17:23:34 +0100
categories: [loop, math, interactive]
level: 8
---

Scrivi il programma `SimpleInterest` utile per calcolare l'interesse semplice di un prestito. Il programma deve funzionare nel modo seguente:

1. Chiede di inserire il capitale iniziale (<math><mi>C</mi><mo>=</mo><msub><mi>M</mi><mn>0</mn></msub></math>)
2. Se il valore inserito non è un numero valido stampa il messaggio:
	
		Valore C non valido "<valore>" 
	e ricomincia dal punto 1.
3. Se il valore inserito è inferiore a 1 stampa: 

		C deve essere maggiore di 0 
	e ricomincia dal punto 1.
4. Chiede di inserire il tasso di interesse (<math><mi>i</mi></math>)
5. Se il valore inserito non è un numero stampa: 

		Valore i non valido "<valore>" 
	e ricomincia dal punto 4.
6. Chiede di inserire il periodo (<math><mi>n</mi></math>)
7. Se il valore inserito non è un numero intero stampa:
		
		Valore n non valido "<valore>" 
	e ricomincia dal punto 6.
8. Se il valore inserito è inferiore a 0 stampa: 

		Il periodo deve deve essere positivo
	e ricomincia dal punto 6.
9. Stampa il montante (<math><msub><mi>M</mi><mi>n</mi></msub></math>) del prestito

Esempio 1:

~~~
Inserire il capitale iniziale (C): 1000
Inserire il tasso di interesse (i): 5
Inserire il periodo (n): 2
M2 = 1100.0
~~~

Esempio 2:

~~~
Inserire il capitale iniziale (C): -1
Il capitale deve essere maggiore di 0
Inserire il capitale iniziale (C): bau
Valore C non valido "bau"
Inserire il capitale iniziale (C): 1000
Inserire il tasso di interesse (i): miao
Valore i non valido "miao"
Inserire il tasso di interesse (i): 7
Inserire il periodo (n): -1
Il periodo deve essere positivo
Inserire il periodo (n): cucu
Valore n non valido "cucu"
Inserire il periodo (n): 5
M5 = 1350.0
~~~
