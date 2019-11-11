---
layout: post
title: "PariDispari"
date: 2017-02-25 11:35:57 +0100
categories: [wrapper,exceptions]
level: 5
---

Scrivi la classe `PariDispari` che valuta il valore intero passato come primo argomento da linea di comando e, se il valore è pari stampa "PARI", altrimenti stampa "DISPARI". Nel caso che il valore passato non sia intero **è necessario** gestire l'eventuale errore in maniera appropriata. Qualche esempio:

~~~text
$ java PariDispari 3
DISPARI
~~~

~~~text
$ java PariDispari 6
PARI
~~~

~~~text
$ java PariDispari 8
PARI
~~~


Se non vengono passati argomenti il programma termina:

~~~text
$ java PariDispari
$
~~~

Se vengono passati argomenti non appropriati:

~~~text
$ java PariDispari "Testo"
ERRORE: il valore Testo non è accettabile
~~~

~~~text
$ java PariDispari 5.3
ERRORE: il valore 5.3 non è accettabile
~~~