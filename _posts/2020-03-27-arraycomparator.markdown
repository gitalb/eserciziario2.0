---
layout: post
title: "ArrayComparator"
date: 2020-03-27 10:15:05 +0100
categories: [array,methods]
level: 12
---

Scrivi la classe `ArrayComparator` contenente i metodi seguenti:

## `public static boolean isLonger(char[] a, char[] b)`

Ritorna `true` se la dimensione dell' array `a` è superiore a quella di `b`, `false` altrimenti.

## `public static char[] append(char c, char[] a)`

Aggiunge  il carattere `c` in coda ad `a` e ritorna l'array risultante.

## `public static boolean onlyContainsVowels(char[] a)`

Ritorna `true` se l'array `a` contiene esclusivamente vocali, altrimenti ritorna `false`.

## `public static char[] compare(char[] a, char[] b)`

Ritorna un array contenente l'elenco di vocali di `a` che si trovano nella stessa posizione dentro a `b`:
	
-  se `a` contiene `'i'`, `'u'`, `'A'`
-  e `b` contiene `'i'`, `'a'`, `'a'`, `'u'`
-  ritorna un array contenente `'i'`, `'A'`

Se `a` contiene caratteri non validi, solleva una `IllegalArgumentException` con il messaggio: 
	
		"Array a non valido"

Se `b` contiene caratteri non validi, solleva una `IllegalArgumentException` con il messaggio: 
	
		"Array b non valido"
		
Se `b` è più piccolo di `a`, solleva una `IllegalArgumentException` con il messaggio: 
	
		"Array b troppo piccolo"	

