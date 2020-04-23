---
layout: post
title: "PolyFrame"
date: 2020-04-22  9:49:12 +0100
categories: [gui]
level: 12
---


Il programma `PolyFrame ` permette all'utente di disegnare un poligono. I vertici del poligono sono rappresentati da pallini e vengono aggiunti cliccando il tasto sinistro del mouse. 

![]({{ site.baseurl }}/assets/posts/poly1.png)

Il programma supporta un numero massimo di punti, definito dalla costante `POLY_SIZE` (default `4`). 

![]({{ site.baseurl }}/assets/posts/poly2.png)
![]({{ site.baseurl }}/assets/posts/poly3.png)
![]({{ site.baseurl }}/assets/posts/poly4.png)

Se l'utente aggiunge un vertice in più rispetto a quelli definiti da `POLY_SIZE` il primo vertice inserito viene rimosso.![]({{ site.baseurl }}/assets/posts/poly5.png)
La dimensione e il colore dei pallini e il colore delle linee sono definiti dalle costanti `POINT_R` e `POINTS_COLOR`.

La distanza minima consentita tra i vertici è pari al **diametro** di un pallino.




