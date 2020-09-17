---
layout: post
title: "ArrayDecoder"
date: 2020-03-27 10:14:08 +0100
categories: [array,methods]
level: 12
---

Scrivi la classe `ArrayDecoder` contenente i metodi seguenti:

## `public static boolean sizeDiffer(char[] a, char[] b)`

Ritorna `true` se la dimensione degli array `a` e `b` è differente, `false` altrimenti.

## `public static int indexOfUnique(char[] a, char c)`

Se il carattere `c` è presente una sola volta nell'array `a`, il metodo ritorna l'indice di `c` in `a`. Altrimenti ritorna `-1`.

## `public static boolean isPermutation(char[] a, char[] b)`

Ritorna `true` solo se l’array `b` è una permutazione valida dell’array `a`, ossia se ogni carattere di `b` è presente una sola volta in `a` (anche in posizioni diverse).

## `public static int[] decode(char[] a, char[] b)`

Ritorna un array che contiene l'indice in cui ogni carattere di `a` è presente dentro a `b`. Ad esempio:
	
-  se `a` contiene `'a'`, `'b'`, `'c'`
-  e `b` contiene `'b'`, `'a'`, `'c'`
-  ritorna un array contenente `1`, `0`, `2`

Se le dimensioni di `a` e `b` sono diverse, solleva una `IllegalArgumentException` con il messaggio: 
	
		"Lunghezze diverse"
	
Se `b` non è una permutazione valida di `a` solleva una `IllegalArgumentException` con il messaggio: 
	
		"Array b non valido"
	
