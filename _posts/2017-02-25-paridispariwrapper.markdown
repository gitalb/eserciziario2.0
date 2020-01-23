---
layout: post
title: "PariDispariWrapper"
date: 2020-01-23 11:35:57 +0100
categories: [wrapper,exceptions]
level: 5
---

Scrivi la classe `PariDispariWrapper` che valuta il valore intero passato come primo argomento da linea di comando e, se il valore è pari stampa "PARI", altrimenti stampa "DISPARI". Nel caso che il valore passato non sia intero **è necessario** gestire l'eventuale errore in maniera appropriata. Qualche esempio:

~~~text
$ java PariDispariWrapper 3
DISPARI
~~~

~~~text
$ java PariDispariWrapper 6
PARI
~~~

~~~text
$ java PariDispariWrapper 8
PARI
~~~


Se non vengono passati argomenti il programma termina:

~~~text
$ java PariDispariWrapper
$
~~~

Se vengono passati argomenti non appropriati:

~~~text
$ java PariDispariWrapper "Testo"
ERRORE: il valore Testo non è accettabile
~~~

~~~text
$ java PariDispariWrapper 5.3
ERRORE: il valore 5.3 non è accettabile
~~~