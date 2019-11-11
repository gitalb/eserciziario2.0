---
layout: post
title: "Butterflyzer"
date: 2017-04-04  9:49:26 +0100
categories: [string,loop,interactive]
level: 13
---

Scrivi il programma interattivo `Butterflyzer` che permetta di codificare e decodificare messaggi in *alfabeto farfallino*. 

1. Inizialmente il programma propone di scegliere la funzione (`'c'` per codificare, `'d'` per decodificare, `'q'` per terminare), 
2. Se la scelta digitata non è valida ricomincia dal punto 1.
3. Se la scelta è `'q'` il programma termina.
4. Se la scelta è `'c'`, chiede all'utente di digitare una stringa di testo da codificare e poi stampa il messaggio codificato.
5. Se la scelta è `'d'`, chiede all'utente di digitare il messagio da decodificare e poi stampa il testo decodificato.
6. Il programma ricomincia dal punto 1.

Esempio:

~~~
$ java Butterflyzer
Codificatore/decodificatore alfabeto Farfallino
Premi 'c' per codificare un messaggio
Premi 'd' per decodificare un messaggio
Premi 'q' per uscire
Scelta: x
Scelta non valida 'x'

Codificatore/decodificatore alfabeto Farfallino
Premi 'c' per codificare un messaggio
Premi 'd' per decodificare un messaggio
Premi 'q' per uscire
Scelta: c
Inserire testo da codificare: Tanto va la gatta al lardo
Messaggio codificato: Tafantofo vafa lafa gafattafa afal lafardofo

Codificatore/decodificatore alfabeto Farfallino
Premi 'c' per codificare un messaggio
Premi 'd' per decodificare un messaggio
Premi 'q' per uscire
Scelta: d
Messaggio da decodificare: Lefe frafagofolefe sofonofo mafatufurefe
Testo decodificato: Le fragole sono mature

Codificatore/decodificatore alfabeto Farfallino
Premi 'c' per codificare un messaggio
Premi 'd' per decodificare un messaggio
Premi 'q' per uscire
Scelta: q
$
~~~