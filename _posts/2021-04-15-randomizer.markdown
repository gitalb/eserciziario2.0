---
layout: post
title: "Randomizer"
date: 2021-04-14 12:29:19 +0100
categories: [math, methods]
level: 10
---

Scrivi il programma `Randomizer` che, dati tre numeri interi passati come argomenti da linea di comando, genera una serie di numeri casuali (separata `','` e terminata da `'.'`). 

I primi due argomenti determinano il range dei valori casuali che verranno generati. Il valore più piccolo non sarà compreso nel range mentre il più grande si. 

Il terzo argomento determina il numero di valori da generare. 

Ad esempio:

```
$ java Randomizer 0 4 5

1, 3, 1, 2, 4.
```

Oppure:

```
$ java Randomizer 5 1 6

2, 4, 5, 3, 5, 2.
```

Se il numero di argomenti non è sufficiente il programma deve stampare un messaggio di errore e terminare:

```
$ java Randomizer 5 

Argomenti insufficienti
```

Se gli argomenti non sono validi il programma dovrà stampare un messaggio di errore indicando il primo valore errato e terminare:

```
$ java Randomizer 1 4 b 

Argomento non valido: b
```

Nota
: è vietato utilizzare la classe `java.util.Random`.


