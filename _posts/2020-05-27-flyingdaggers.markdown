---
layout: post
title: "FlyingDaggers"
date: 2020-05-26 20:40:11 +0100
categories: [anim1D]
level: 14
---

Scrivi il video gioco 1D `FlyingDaggers`. Il gioco consiste nel lancio di un pugnale che deve colpire un bersaglio. 

Il giocatore ha a disposizione un numero limitato di pugnali (default 6) che vengono lanciati in sequenza. Il pugnale parte dalla posizione orizzontale (`-`) e procede ruotando in senso orario verso il bersaglio (`O`). 

<video width="574" height="144" controls>
  <source src="{{ site.baseurl }}/assets/posts/FlyingDaggers.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

Se, quando colpisce il bersaglio ,il pugnale è in posizione orizzontale, il bersaglio esplode (`*`) e il giocatore guadagna un punto:

![]({{ site.baseurl }}/assets/posts/FlyingDaggersHit.png)

Il gioco termina quando la riserva di pugnali è esaurita.

Ad ogni lancio il bersaglio si sposta ad una distanza casuale (minino 10, massimo 30). 

Durante la partita l'interfaccia rappresenta la riserva di pugnali e il punteggio attuale:

![]({{ site.baseurl }}/assets/posts/FlyingDaggers.png)


