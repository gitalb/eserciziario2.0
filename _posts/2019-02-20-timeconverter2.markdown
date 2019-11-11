---
layout: post
title: "TimeConverter2"
date: 2019-02-20  7:05:35 +0100
categories: [exceptions]
level: 12
---


Scrivi la classe `TimeConverter2` che converte un tempo espresso in ore, minuti e secondi in secondi. 

## `convertInt`
Per convertire i 3 argomenti da `String` a `int` devi creare il metodo:

~~~java
public static int convertInt(String s) throws NumberFormatException 
~~~

Se la stringa `s` non può essere convertita in un numero intero, il metodo solleva una `NumberFormatException`.

## `main`
Il metodo `main` deve:

1. Chiedere all'utente di inserire 3 valori interi che cattura con il metodo `next()` della classe `Scanner` (**non è permesso** utilizzare `nextInt()`). 
2. Usa il metodo `convertInt` per ricavarne i valori interi.
3. Stampa a terminale il risultato della conversione.

Ad esempio - per 1 ora, 2 minuti e 3 secondi - il programma stampa `3723`:

~~~
1:2:3 corrispondono a 3723 secondi.
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