---
layout: post
title: "ArrayEncoder"
date: 2020-03-27 10:12:36 +0100
categories: [array,methods]
level: 12
---


Scrivi la classe `ArrayEncoder` contenente i metodi seguenti:

## `public static boolean sizeEquals(char[] c, int[] p)`

Ritorna `true` se la dimensione degli array `c` e `p` equivale, `false` altrimenti.

## `public static boolean contains(int[] p, int value)`

Ritorna `true` se l'array `p` contiene il valore `value`, `false` altrimenti.

## `public static boolean isValid(int[] p)`

Ritorna `true` solo se l'array `p` contiene tutti i numeri compresi nell'intervallo `[0;p.length[`.

## `public static char[] encode(char[] c, int[] p)`

Ritorna un array in cui ogni carattere di `c` si trova nella posizione specificata dal rispettivo valore in `p`. Ad esempio:
	
-  se `c` contiene `'a'`, `'b'`, `'c'`
-  e `p` contiene `2`, `0`, `1`
-  ritorna un array contenente `'b'`, `'c'`, `'a'`

Se le dimensioni di `c` e `p` non sono uguali, solleva una `IllegalArgumentException` con il messaggio: 
	
		"Dimensione diversa"
	
Se `p` contiene dei valori non validi, solleva una `IllegalArgumentException` con il messaggio: 
	
		"Indici non validi"
	
