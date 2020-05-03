---
layout: post
title: "PerfectFinder"
date: 2020-05-02  7:40:17 +0100
categories: [collections]
level: 11
---

Scrivi la classe `PerfectFinder` utile per individuare i *numeri perfetti*. La classe deve esportare i metodi seguenti:

- `public static boolean isPerfect(int n)`: ritorna `true` se `n` è un numero perfetto, `false` altrimenti 

- `public static boolean isDefective(int n)`: ritorna `true` se `n` è un numero difettivo, `false` altrimenti 

- `public static List<Integer> getDividers(int n)`: ritorna l'elenco dei divisori propri di `n`

- `public static long getDividersSum(List<Integer> dividers)`: ritorna la somma dei numeri con tenuti nella lista `dividers`

- `public static List<Integer> getPerfectNumbers(int min, int max)`: ritorna l'elenco dei numeri perfetti presenti nell'intervallo [`min`, `max`]

## Numeri perfetti

Un numero `N` è detto *perfetto* se la somma dei suoi divisori propri (positivi, `N` escluso)  è pari ad `N`. Ad esempio `28` è un numero perfetto perché sommando i suoi divisori propri (`1, 2, 4, 7 e 14`) si ottiene `28`.

Invece se la somma dei divisori di `N` è inferiore al suo valore, `N` è un numero *difettivo*, mentre se le somma dei divisori è superiore, `N` è un numero *abbondante*.

