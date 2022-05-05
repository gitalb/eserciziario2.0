---
layout: post
title: "BlackJack"
date: 2017-03-21 21:04:24 +0100
categories: [methods]
level: 11
---

Nel Blackjack vince il giocatore che totalizza un punteggio che:

- sia superiore a 0
- sia il più vicino possibile, ma non superi, il valore 21


Scrivi La classe `BlackJack` contenente il metodo: 

~~~java
public static int blackjackWinner(int score1, int score2)
~~~

che, dati due punteggi `score1` e `score2`, ritorna un numero intero secondo le seguenti regole:

- in caso di pareggio, ritorna `0`
- se vince `score1` ritorna `1`
- se vince `score2` ritorna `2`

Qualche esempio: 

- `blackjackWinner(16,19)` ritorna `2`
- `blackjackWinner(21,17)` ritorna `1`
- `blackjackWinner(22,17)` ritorna `2`
- `blackjackWinner(1,0)` ritorna `1`
- `blackjackWinner(0,23)` ritorna `0`