---
layout: post
title: "ButterFyler"
date: 2020-04-19  7:33:31 +0100
categories: [String, Files]
level: 13
---

Scrivi il programma `ButterFyler` utile per codificare un file di testo (UTF-8) in *alfabeto farfallino* e salvarlo in un file di destinazione (se non conosci l'*alfabeto farfallino* vedi [wikipedia](https://it.wikipedia.org/wiki/Alfabeto_farfallino)). 

La classe deve contenere il metodo `encode` che codifica il file `source` e lo salva nel file `dest`:

~~~java
public static void encode(Path source, Path dest)
~~~

Per verificare il buon funzionamento del tuo programma prova a codificare la [Divina commedia]({{ site.baseurl }}/assets/posts/LA_DIVINA_COMMEDIA.txt) e a cronometrare il tempo impiegato per la codifica (usa `System.currentTimeMillis()` per misurare il tempo).




