---
layout: post
title: "Coordinator"
date: 2018-12-23  8:40:49 +0100
categories: [loop, interactive]
level: 13
---


Scrivi la class `Coordinator` che:

1. Chiede all'utente di inserire la *coordinata di riga* (intero, valore minimo `0`, valore massimo `4`).

2. Se il valore non è valido stampa un messaggio di errore e ricomincia dal punto 1.

3. Chiede di inserire la *coordinata di colonna* (intero, valore minimo `0`, valore massimo `4`).

4. Se il valore non è valido stampa un messaggio di errore e ricomincia dal punto 3.

5. Stampa a terminale un piano cartesiano (dimensione 5 x 5) con una `X` alla coordinata immessa (vedi esempi).

I messaggi di errore da stampare (ai punti 2. e 4.) sono i seguenti:

- Se il valore immesso è troppo basso: `"Valore troppo piccolo <valore>"`
- Se il valore immesso è troppo alto: `"Valore troppo grande <valore>"`
- Se il valore non è un numero: `"Inserire solo numeri interi"`

Esempio di output:

~~~
Inserire coordinata riga [0;4]: 2
Inserire coordinata colonna [0;4]: 2
 01234
0     
1     
2  X  
3     
4             
~~~

Oppure:

~~~
Inserire coordinata riga [0;4]: -1
Valore troppo piccolo -1
Inserire coordinata riga [0;4]: 0
Inserire coordinata colonna [0;4]: 100
Valore troppo grande 100
Inserire coordinata colonna [0;4]: zero
Inserire solo numeri interi
Inserire coordinata colonna [0;4]: 0
 01234
0X    
1     
2     
3     
4 
~~~
