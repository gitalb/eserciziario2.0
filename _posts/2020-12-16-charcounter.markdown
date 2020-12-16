---
layout: post
title: "CharCounter"
date: 2020-12-16 10:03:58 +0100
categories: [string, files]
level: 13
---

Scrivi il programma `CharCounter` che calcola la frequenza dei caratteri alfabetici contenuti in un file di testo. Il percorso del file è fornito come primo argomento da linea di comando. Il programma legge il contenuto del file e stampa il conteggio dei caratteri (*case insensitive*) e il tempo impiegato. Ad esempio, per un file contenente il testo seguente:

~~~
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
~~~

il programma stampa:

~~~
'a: 29
'b: 3
'c: 16
'd: 19
'e: 38
'f: 3
'g: 3
'h: 1
'i: 42
'j: 0
'k: 0
'l: 22
'm: 17
'n: 24
'o: 29
'p: 11
'q: 5
'r: 22
's: 18
't: 32
'u: 29
'v: 3
'w: 0
'x: 3
'y: 0
'z: 0

Parse time: 5ms
~~~

Se il percorso fornito come primo argomento non è valido (non esiste, non è leggibile), il programma stampa il messaggio `"Error reading <file>"` e termina.

Se non vengono forniti argomenti il programma stampa il messaggio `"Usage: java CharCounter <file>"`.


Per verificare il buon funzionamento del tuo programma puoi usare la [Divina commedia]({{ site.baseurl }}/assets/posts/LA_DIVINA_COMMEDIA.txt) e cronometrare il tempo impiegato (usa `System.currentTimeMillis()` per misurare il tempo).



