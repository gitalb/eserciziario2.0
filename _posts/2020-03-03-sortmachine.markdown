---
layout: post
title: "SortMachine"
date: 2020-03-03 15:18:13 +0100
categories: [sort, array, methods]
level: 13
---

Scrivi la classe `SortMachine` contenente i metodi descritti in seguito.

- ```public static int getRandomInt(int min, int max)```: ritorna un numero intero casuale nel range [`min`;`max`].
- ```public static void randomize(int[] a, int min, int max)```: riempie l'array `a` di numeri casuali nel range [`min`;`max`].
- ```public static void swap(int[] a, int i, int j)```: se esistenti, scambia i valori dei due elementi di `a` che si trovano in `i` e `j`.
- ```public static boolean isSorted(int[] a) ```: ritorna `true` se l'array `a` è ordinato (crescente), `false` altrimenti.
- ```public static void bubbleSort(int[] a)```: ordina gli elementi di `a` in modo crescente applicando l'algoritmo *bubble sort*.
- ```public static void selectionSort(int[] a)```: ordina gli elementi di `a` in modo crescente applicando l'algoritmo *selection sort*.

Poi verifica il buon funzionamento dei metodi e confronta le prestazioni di *bubble* e *selection sort* cronometrando quanto tempo impiegano per ordinare un array di 10000 elementi.

