---
layout: post
title: "Calcolatrice3"
date: 2019-02-20  6:55:37 +0100
categories: [exceptions]
level: 12
---

Scrivi la classe `Calcolatrice3` contenente il metodo:

~~~java
public static int calcola(String[] espressione)
~~~

Tale metodo valuta le stringhe contenute nell'array `espressione` che rappresentano le parti di un'espressione aritmetica e ne calcola il valore. 

Ad esempio per `{"1", "+", "2"}` il metodo ritorna `3`; mentre per `{"3", "*", "3"}` ritorna `9`.

Gli operatori ammessi sono `'+'`, `'-'`, `'*'`, `'/'`. Gli operandi devono essere dei numeri interi.  

Se l'espressione da valutare contiene un operatore o degli operandi non validi, il metodo ritorna 0.
