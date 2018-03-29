---
layout: post
title: "CsvValidator"
date: 2018-03-29  8:58:36 +0100
categories: [files, loops]
level: 12
---
Scrivi la classe `CsvValidator` contenente il metodo:

~~~java
public static boolean isValid(Path csvFile)
~~~

Tale metodo verifica che il file in formato csv `csvFile` rispetti le seguenti regole:

- contiene solo numeri **interi** nel range **[1;100]** 
- i valori sono disposti in una *griglia* di dimensione N x N
- contiene lo **stesso numero** (N) di righe e colonne
- su ogni riga vi sono N valori separati dal carattere `';'`
- **non** contiene righe vuote

Se tutte le regole sono rispettate il metodo ritorna `true`, in qualsiasi altro caso il metodo ritorna `false`. Se il file non è accessibile il metodo ritorna `false`.

Esempio di file valido (3 x 3):

~~~text
1;2;3
4;5;6
7;8;9
~~~

