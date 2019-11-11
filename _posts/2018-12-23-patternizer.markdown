---
layout: post
title: "Patternizer"
date: 2018-12-23  8:47:26 +0100
categories: [loop,interactive]
level: 13
---


Scrivi la classe `Patternizer` che chiede all'utente di inserire un *pattern* che servirà da modello per disegnare una figura bidimensionale. L'utente introduce la sequenza di caratteri da stampare su di una sola riga utilizzando il carattere `'g'` per indicare i punti in cui andare *a capo*. 

Ad esempio la sequenza `" /\g/  \g|__|"` produce il disegno seguente:

~~~
 /\
/  \
|__|
~~~

Il programma stampa il disegno in uno spazio cartesiano in cui devono comparire le coordinate orizzontali e verticali come mostrato negli esempi seguenti:

~~~
Inserire pattern (g per new line):
****g*  *g*  *g****
 0123
0****
1*  *
2*  *
3****
~~~

Oppure:

~~~
Inserire pattern (g per new line):
*********g.*.....*.g..*...*..g...*.*...g....*....
 012345678
0*********
1.*.....*.
2..*...*..
3...*.*...
4....*....
~~~

La figura contenuta nel pattern deve avere una larghezza massima di 10 caratteri. Se il pattern fornito non rispetta questa regola, il programma stampa il messaggio `Riga <riga> troppo lunga (max 10 char)`, indicando il numero della riga non valida e poi ripete la richiesta iniziale. Esempio:

~~~
Inserire pattern (g per new line):
*.*.*.*.*.*g***g---*g
Riga 0 troppo lunga (max 10 char)
Inserire pattern (g per new line):
/\/\/\g\/\/\/
 012345
0/\/\/\
1\/\/\/
~~~

