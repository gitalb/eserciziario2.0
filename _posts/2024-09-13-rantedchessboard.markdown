---
layout: post
title: "RantedChessBoard"
date: 2024-09-13 09:00:00 +0100
categories: [args, array, loops]
level: 6
---


Scrivi il programma `RantedChessBoard` che riceve `N` interi come argomenti da linea di comando e crea una matrice *ranted* contenente `N` righe. Ogni riga possiede la lunghezza definita dal rispettivo argomento. La matrice va poi riempita *a scacchiera*, ossia con  un'alternanza di `0` e `1`.

Ad esempio gli argomenti `"1 3 2"` producono una matrice di 3 righe in cui la prima ha dimensione 1, la seconda 3 e la terza 2:

~~~text
0 
1 0 1 
0 1 
~~~

Per `"7 5 4 3 2 8"` si ottiene invece:

~~~text
0 1 0 1 0 1 0 
1 0 1 0 1 
0 1 0 1 
1 0 1 
0 1 
1 0 1 0 1 0 1 0 
~~~

E per `"1 2 3 4 5 6 7 2 2 2"`:

~~~text
0 
1 0 
0 1 0 
1 0 1 0 
0 1 0 1 0 
1 0 1 0 1 0 
0 1 0 1 0 1 0 
1 0 
0 1 
1 0 
~~~