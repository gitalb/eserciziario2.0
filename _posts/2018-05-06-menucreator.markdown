---
layout: post
title: "MenuCreator"
date: 2018-05-06 11:11:44 +0100
categories: [class, interactive, draw]
level: 12
---

# `MenuCreator`

Devi realizzare un'applicazione utile per redigere il menu di un ristorante. Un *menu* è costituito dall'elenco delle *pietanze* servite. Per ogni *pietanza* viene indicato il *nome* e il *prezzo*.

![]({{ site.baseurl }}/assets/posts/menu.png){:width="300"}


Per realizzare l'applicazione devi procedere in 2 fasi.

## `Food`
Creare la classe `Food`, che rappresenta il modello di *pietanza*. La classe `Food` deve possedere due attributi privati utili per la memorizzazione del nome e del prezzo della pietanza (e i relativi metodi getter e setter). Il nome è costituito da una stringa (valore di default `"NO NAME"`), mentre il prezzo è un numero reale a precisione doppia (valore di default `5.0`). Inoltre la classe deve esportare il costruttore vuoto e un costruttore personalizzato che permetta di inizializzare entrambi gli attributi della pietanza.

## `MenuCreator`
Realizzare l'applicazione `MenuCreator`. È una semplice applicazione che serve a generare il *menu* (*la carta delle pietanze*) di un ristorante. Quando viene eseguita, propone all'utente 2 possibilità: `Aggiungi pietanza` e `Esci`. 

Scegliendo `Aggiungi pietanza`, l'utente può aggiungere una pietanza fornendone il nome ed il prezzo. Il nome della pietanza non può essere vuoto o nullo e deve avere una lunghezza massima di 50 caratteri. Il prezzo fornito deve essere un numero positivo. 

~~~
[1 Aggiungi pietanza | 2 Esci] Scelta: 1

Aggiungi pietanza
-----------------
Nome pietanza: Insalata verde
Prezzo pietanza: 6.50
Aggiunto Insalata verde, CHF 6.50
---------------------------~~ MENU ~~---------------------------
| Insalata verde                                     CHF  6.50 |
----------------------------------------------------------------
[1 Aggiungi pietanza | 2 Esci] Scelta:
~~~


Se un valore fornito dall'utente non è accettabile, il programma stampa un messaggio e ripropone la richiesta come mostrato nell'esempio seguente:

~~~
[1 Aggiungi pietanza | 2 Esci] Scelta: 1

Aggiungi pietanza
-----------------
Nome pietanza: Specialità della casa con il nome trooooppo lunghissimo
Nome non valido Specialità della casa con il nome trooooppo lunghissimo
Nome pietanza: Sorbetto
Prezzo pietanza: -12
Prezzo non valido -12.0
Prezzo pietanza: 6
Aggiunto Sorbetto, CHF 6.00
---------------------------~~ MENU ~~---------------------------
| Insalata verde                                     CHF  5.50 |
| Insalata mista                                     CHF  6.50 |
| Spaghetti aglio olio e peperoncino                 CHF  9.00 |
| Spaghetti alla carbonara                           CHF 12.50 |
| Lasagne fatte in casa                              CHF 14.00 |
| Bistecca di manzo con contorno                     CHF 23.25 |
| Polenta e brasato                                  CHF 22.00 |
| Torta della nonna                                  CHF  6.40 |
| Gelato                                             CHF  2.40 |
| Sorbetto                                           CHF  6.00 |
----------------------------------------------------------------
[1 Aggiungi pietanza | 2 Esci] Scelta: 
~~~

Dopo aver aggiunto una pietanza all'elenco il programma stampa un messaggio di conferma (es. `Aggiunto Sorbetto, CHF 9.00`) e il menu formattato correttamente. Poi propone nuovamente la possibilità di aggiungere una pietanza o di terminare il programma.

