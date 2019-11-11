---
layout: post
title: "TimeConverter"
date: 2018-04-10 11:28:58 +0100
categories: [exceptions]
level: 12
---

Scrivi la classe `TimeConverter` che converte un tempo espresso in ore, minuti e secondi (forniti come argomenti da linea di comando) in secondi. 

## `convertInt`
Per convertire i 3 argomenti da `String` a `int` devi creare il metodo:

~~~java
public static int convertInt(String s) throws NumberFormatException 
~~~

Se la stringa `s` non può essere convertita in un numero intero, il metodo solleva una `NumberFormatException`.

## `main`
Il metodo `main` cattura i 3 argomenti, usa il metodo `convertInt` per ricavarne i valori interi e poi stampa a terminale il risultato della conversione.

Ad esempio - per 1 ora, 2 minuti e 3 secondi - il programma stampa `3723`:

~~~
java TimeConverter 1 2 3
1:2:3 corrispondono a 3723 secondi.
~~~

Se il numero di argomenti fornito non è sufficiente, il programma termina stampando:

~~~
Utilizzo: java TimeConverter <h> <m> <s>
~~~

Se il valore fornito per le `ore` non è appropriato il programma stampa:

~~~
ore: valore non valido <valore>
~~~


Se il valore fornito per i `minuti` non è appropriato il programma stampa:

~~~
minuti: valore non valido <valore>
~~~

Se il valore fornito per i `secondi` non è appropriato il programma stampa:

~~~
secondi: valore non valido <valore>
~~~