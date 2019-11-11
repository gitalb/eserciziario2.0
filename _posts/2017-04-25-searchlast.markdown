---
layout: post
title: "SearchLast"
date: 2017-04-25 11:59:23 +0100
categories: [search,array]
level: 12
---

Scrivi la classe `SearchLast` che applica una ricerca sequenziale per trovare l'ultima ricorrenza di `args[0]` in `args[1;N]` e ne stampa l'indice (partendo da 0). Ad esempio:

~~~text
$ java SearchLast 3 1 7 5 9 67 4 7 3 7 9
7
~~~

Oppure:

~~~text
$ java SearchLast 1 1 2 1 3 1 4 
4
~~~

Se il valore cercato non è presente il programma stampa il messaggio `"Valore non trovato"`.
