---
layout: post
title: "SumArgsHex"
date: 2017-02-25 11:45:31 +0100
categories: [wrapper]
level: 7
---


Scrivi la classe `SumArgsHex` che stampa a terminale la somma dei due valori interi passati come argomenti da linea di comando in formato esadecimale. Nel caso che i valori passati non siano valori interi **è necessario** gestire l'eventuale errore in maniera appropriata. Esempio:

~~~text
$ java SumArgsHex 5 5
5 + 5 = a
~~~

~~~text
$ java SumArgsHex A 5
a + 5 = f
~~~

~~~text
$ java SumArgsHex FF FF
ff + ff = 1fe
~~~

Se vengono passati argomenti non appropriati:

~~~text
$ java SumArgsHex FF "Cinque"
ERRORE: uno o più valori passati non sono accettabili
~~~

~~~text
$ java SumArgsHex 5.3 FF
ERRORE: uno o più valori passati non sono accettabili
~~~
