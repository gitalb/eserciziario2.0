---
layout: post
title: "HashGenerator"
date: 2022-10-23 10:52:51 +0100
categories: [string]
level: 3
---

Un sistema di gestione del personale deve generare una sigla associata ad ogni dipendente secondo un formato standardizzato. Il formato prevede che la sigla di ogni persona sia composta da 4 caratteri e un numero intero:

1. Il primo carattere del cognome in **maiuscolo**,
2. l'ultimo carattere del cognome in **minuscolo**,
3. il primo carattere del nome in **maiuscolo**,
4. l'ultimo carattere del nome in **minuscolo**,
5. il numero totale di caratteri che compongono nome e cognome, espresso in base 10.

Scrivi la classe Java `HashGenerator` che, dati nome e cognome memorizzati in due **costanti**, stampi a terminale la relativa sigla. Il formato dell'output deve rispettare rigorosamente quello proposto nei seguenti esempi:

Per un impiegato di nome "HAiEiE" e cognome "bRaZorF":

~~~
	Nome:    HAiEiE
	Cognome: bRaZorF
	Sigla:   BfHe13
~~~

Per un impiegato di nome "Mickey" e cognome "Mouse":

~~~
	Nome:    Mickey
	Cognome: Mouse
	Sigla:   MeMy11
~~~

Per un impiegato di nome "vladimir" e cognome "harkonnen":

~~~
	Nome:    vladimir
	Cognome: harkonnen
	Sigla:   HnVr17
~~~


