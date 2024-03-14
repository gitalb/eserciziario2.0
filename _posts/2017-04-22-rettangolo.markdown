---
layout: post
title: "Rettangolo"
date: 2017-04-22 09:05:10 +0100
categories: [class]
level: 13
---

Scrivi la classe `Rettangolo` che rappresenta il modello astratto di rettangolo. La classe deve possedere due attributi interi *privati* `latoA` e `latoB` utili per descrivere rispettivamente la dimensione orizzontale e verticale del rettangolo. 

Dovrai implementare pure i metodi *getter* e *setter* per entrambi gli attributi `latoA` e `latoB` applicando la regola seguente:

- `latoA` e `latoB` non possono mai essere pari a 0 o negativi.
 

La classe deve esportare due metodi *costruttori* e i *metodi di istanza*: 

- il *costruttore vuoto* che istanzia un `Rettangolo` con le *dimensioni di default* (10 x 5)
- un *costruttore personalizzato* `public Rettangolo(int latoA, int latoB)` che istanzia un rettangolo con le dimensioni fornite (se valide, altrimenti applica le *dimensioni di default*). 
- `public int getArea()`: ritorna l'area del rettangolo
- `public int getPerimetro()`: ritorna il perimetro del rettangolo
- `public void draw()`: disegna a terminale un rettangolo composto di asterischi, ad esempio per un rettangolo di 10 x 5 stampa:
	
	~~~text
	**********
	*        *
	*        *
	*        *
	**********
	~~~
- `public String toString()`: ritorna una descrizione testuale del rettangolo, ad esempio per un rettangolo di 10 x 5 ritorna: `"Rettangolo 10 x 5"`

Quando hai terminato scrivi il metodo `main` in cui dovrai istanziare 3 rettangoli di dimensioni differenti e verificare su ognuno il buon funzionamento dei metodi. 
