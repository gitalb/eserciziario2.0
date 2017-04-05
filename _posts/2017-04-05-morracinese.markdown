---
layout: post
title: "MorraCinese"
date: 2017-04-05 11:21:17 +0100
categories: [interactive,loop]
level: 14
---


Scrivi il gioco interattivo `MorraCinese`. Il programma chiede di inserire il *punteggio massimo*, poi il gioco comincia. Vince chi raggiunge prima il *punteggio massimo*.

1. Il programma chiede di inserire il *punteggio massimo*. Sono ammessi solo valori nel range [1;10]. 
2. Se l'utente inserisce un valore non valido, ricomincia dal punto 1.
3. Chiede all'utente di inserire la sua giocata (`1` per carta, `2` per sasso, `3` per forbice).
4. Se l'utente inserisce un valore non valido, ricomincia dal punto 3.
5. Il programma estrae a sorte la propria giocata (`1` per carta, `2` per sasso, `3` per forbice).
6. Il programma visualizza le due giocate e, se ve ne è uno, il vincitore della mano corrente (player o CPU) e il punteggio attuale dei due giocatori.
7. Se nessuno ha raggiunto il *punteggio massimo* il programma prosegue dal punto 3.
8. Se un giocatore ha raggiunto il *punteggio massimo* il programma stampa il *nome* del vincitore (player o CPU) e prosegue dal punto 9.
9. Il programma chiede se si vuole giocare di nuovo (`0` per continuare, `1` per terminare). 
10. Se l'utente inserisce un valore non valido, ricomincia dal punto 9.
11. Se l'utente inserisce `0`  il programma ricomincia dal punto 1.
11. Se l'utente inserisce `1`  il programma termina.

Esempio:

<video width="320" height="240" controls>
  <source src="{{ site.baseurl }}/assets/posts/MorraCineseMID.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>