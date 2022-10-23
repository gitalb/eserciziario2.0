---
layout: post
title: "HashBuilder"
date: 2022-10-23 13:45:06 +0100
categories: [string]
level: 3
---


Un sistema di gestione del personale deve generare una sigla associata ad ogni dipendente secondo un formato standardizzato. Il formato prevede che la sigla di ogni persona sia composta da 6 caratteri:


1. Il primo carattere del nome in **maiuscolo**,
2. il secondo carattere del nome in **minuscolo**,
3. l'ultimo carattere del nome in **minuscolo**,
4. il primo carattere del cognome in **minuscolo**,
5. il penultimo carattere del cognome in **minuscolo**,
6. l'ultimo carattere del cognome in **maiuscolo**.


Scrivi la classe Java `HashBuilder` che, dati nome e cognome memorizzati in due **costanti**, stampi a terminale la relativa sigla. Il formato dell'output deve rispettare rigorosamente quello proposto nel seguente esempio:

Per un impiegato di nome "HAiEiE" e cognome "braZoRf":

~~~
	Cognome: braZoRf
	Nome:    HAiEiE
	Sigla:   HaebrF
~~~
