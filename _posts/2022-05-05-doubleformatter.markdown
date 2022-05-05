---
layout: post
title: "DoubleFormatter"
date: 2022-05-05 09:50:06 +0100
categories: [interactive format]
level: 8
---



Scrivi il programma `DoubleFormatter` che chiede all’utente di inserire:

- Un numero double (`double n`)
- Quanti caratteri riservare alla stampa (`int w`)
- Quante cifre dopo la virgola stampare (`int p`)
- Se stampare allineando a destra o a sinistra (`String a`, `"DX"`: destra, `"SX"`: sinistra)

Dopodiché il programma stampa il numero (`n`) applicando la formattazione definita dai valori di `w`, `p` e `a`. Ad esempio:

~~~
Inserire un numero double: 1.23456789
Inserire ampiezza: 10
Inserire precisione: 5
Inserire allineamento (dx/sx): dx
'   1.23457'
~~~

Oppure:

~~~
Inserire un numero double: 1.23456789
Inserire ampiezza: 10
Inserire precisione: 4
Inserire allineamento (dx/sx): sx
'1.2346    '
~~~

