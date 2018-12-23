---
layout: post
title: "ActionableIsbnChecker"
date: 2018-12-23  8:49:25 +0100
categories: [string,math]
level: 10
---


L'ISBN-13 *azionabile* è un codice composto secondo il modello:

		ISBN A 10.###.#######/###

Ad esempio:

		ISBN A 10.978.8889637/418

Dove la sequenza di `#` rappresenta 13 cifre (12 cifre di *codice* + 1 *cifra di controllo*). 


La *cifra di controllo* si calcola in base al valore delle 12 cifre precedenti con il seguente algoritmo numerico:

1. si moltiplica ogni cifra per un peso che assume in modo alternato i valori 1 e 3, partendo dalla prima cifra a sinistra che ha peso 1
2. si sommano i risultati
3. si divide la somma per 10 e si prende il resto della divisione
4. si sottrae il risultato da 10: questa cifra è la *cifra di controllo*; se quest'ultimo risultato fosse proprio 10, lo si sostituirà con 0.

Ad esempio per il codice `ISBN A 10.978.8843025/34`:

~~~
9 * 1 + 7 * 3 + 8 * 1 + 8 * 3 + 8 * 1 + 4 * 3 + 3 * 1 + ... + 4 * 3 = 117

117 diviso 10 da resto 7

10 - 7 = 3 
~~~

la cifra di controllo sarebbe **3** (quindi il codice completo sarebbe `ISBN A 10.978.8843025/343`). 


Scrivi il programma `ActionableIsbnChecker` che chiede all'utente di inserire un *codice ISBN-13 azionabile* e ne verifica la correttezza.

I prefissi `ISBN`, `A` e `10`, i punti, lo slash e gli spazi (`'.'`, `'/'` e `'' `) sono opzionali, se vengono omessi il programma esegue comunque la verifica. 

Il *codice* e la *cifra di controllo* devono essere presenti e validi, altrimenti il programma stampa un messaggio di errore. 

Se il codice non è valido, il messaggio stampato è `Codice non valido`. Se la *cifra di controllo* non è valida (`[1;10]`) il messaggio di errore è `Cifra di controllo non valida`.

Se l'utente inserisce un *codice* con il formato ammesso, il programma ne verifica la bontà controllando la corrispondenza tra *codice* e *cifra di controllo*. Se corrispondono il programma termina stampando il messaggio `Codice verificato!`, altrimenti stampa `Codice errato`.

