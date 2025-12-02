---
layout: post
title:  "ArrayManager"
date:   2025-12-02 10:47:01 +0100
categories: [array, loop]
level: 12
---


Scrivi il programma `ArrayManager` che permette di aggiungere e togliere dei numeri interi ad un array. Inizialmente l'array è vuoto. Il programma chiede ripetutamente di inserire un numero intero (`N`) e:

- se `N` è positivo lo inserisce nell'array, l'inserimento avviene in modo che i valori nell'array siano sempre in ordine crescente
- se `N` è negativo e il suo valore assoluto è presente nell'array, viene rimosso dall'array
- se `N` è 0, il programma termina
- ad ogni *ciclo* il contenuto dell'array viene stampato
  
Esempio:

~~~text
Insert a number (0 to quit): 10
10 
Insert a number (0 to quit): 20
10 20 
Insert a number (0 to quit): 30
10 20 30 
Insert a number (0 to quit): 15
10 15 20 30 
Insert a number (0 to quit): 25
10 15 20 25 30 
Insert a number (0 to quit): 20
10 15 20 20 25 30 
Insert a number (0 to quit): 20
10 15 20 20 20 25 30 
Insert a number (0 to quit): 20
10 15 20 20 20 20 25 30 
Insert a number (0 to quit): -5
10 15 20 20 20 20 25 30 
Insert a number (0 to quit): -15
10 20 20 20 20 25 30 
Insert a number (0 to quit): -20
10 25 30 
Insert a number (0 to quit): -25
10 30 
Insert a number (0 to quit): 0
10 30 
~~~
