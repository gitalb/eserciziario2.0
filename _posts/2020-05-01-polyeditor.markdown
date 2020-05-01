---
layout: post
title: "PolyEditor"
date: 2020-05-01 08:23:58 +0100
categories: [gui]
level: 13
---



Il programma `PolyEditor` permette all'utente di disegnare e modificare un poligono. 

La dimensione e il colore dei pallini e il colore delle linee sono definiti dalle costanti `POINT_R` (default 4) e `POINTS_COLOR` (default nero).

## Aggiunta e rimozione

I vertici del poligono sono rappresentati da pallini e vengono aggiunti cliccando il tasto sinistro del mouse. È possibile rimuovere un pallino cliccandolo con il tasto destro.

Il programma supporta un numero massimo di punti, definito dalla costante `POLY_SIZE` (default `4`). 

Se l'utente aggiunge un vertice in più rispetto a quelli definiti da `POLY_SIZE` il primo vertice inserito viene rimosso.
La distanza minima consentita tra i vertici è pari al **diametro** di un pallino.

## Mouse over

Quando il puntatore del mouse si trova dentro alla superficie di un pallino, il pallino assume il colore definito dalla costante `OVER_COLOR` (default verde). 

## Spostamento

È possibile spostare un pallino trascinandolo con il mouse. Durante lo spostamento il colore assume il colore definito dalla costante `DRAG_COLOR` (default arancio).

Durante lo spostamento i pallini non si possono sovrapporre.
 
Se durante il trascinamento il puntatore esce dalla finestra, lo spostamento viene interrotto.


## Metodi

La classe deve esportare i seguenti metodi:

- il costruttore vuoto
- `public List<Point> getPointsIn(Point p, int distance)`: ritorna la lista di tutti i pallini che si trovano ad una distanza uguale o inferiore a `distance` dalla posizione `p`
- `public void addPoint(Point p)`: se possibile, aggiunge un nuovo pallino nella posizione `p`
- `public void removePoint(Point p)`: se ve ne è uno, rimove il pallino che si trova nei pressi della posizione `p`
- `public void movePoint(Point p, Point newPosition)`: se è possibile, sposta il pallino `p` nella posizione `newPosition`


## Demo

<video width="510" height="266" controls>
  <source src="{{ site.baseurl }}/assets/posts/PolyEditor.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video> 


