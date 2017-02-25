---
layout: post
title: "Calcolatrice"
date: 2017-02-25 12:27:16 +0100
categories: [methods,math]
level: 11
---

Scrivi la classe `Calcolatrice` contenente il metodo:

~~~java
public static int calcola(int a, int b, char operatore)`
~~~

Tale metodo esegue un'operazione matematica di base sui due numeri `a` e `b`. Il valore `operatore` (`'+'`, `'-'`, `'*'`, `'/'`) definisce l'operazione da eseguire. 

Ad esempio l'invocazione `calcola(5,2,'+')` ritornerà `7` (`5+2`) mentre l'invocazione `calcola(5,2,'*')` ritornerà `10` (`5*2`). Se il parametro `operatore` contiene un carattere non valido, il metodo ritorna 0.