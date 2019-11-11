---
layout: post
title: "CifrarioDiCesare"
date: 2017-03-21 21:28:43 +0100
categories: [string,methods]
level: 12
---


Da [Wikipedia](https://it.m.wikipedia.org/wiki/Cifrario_di_Cesare):

> “Il cifrario di Cesare è uno dei più antichi algoritmi crittografici di cui si abbia traccia storica. È un cifrario a sostituzione monoalfabetica in cui ogni lettera del testo in chiaro è sostituita nel testo cifrato dalla lettera che si trova un certo numero di posizioni dopo nell'alfabeto. Questi tipi di cifrari sono detti anche cifrari a sostituzione o cifrari a scorrimento a causa del loro modo di operare: la sostituzione avviene lettera per lettera, scorrendo il testo dall'inizio alla fine.” ... ” In particolare, Cesare utilizzava uno spostamento di 3 posizioni (la chiave era dunque 3” ...

---

Ad esempio, applicando la chiave 3: `'a'` diventa `'d'`, `'b'` diventa `'e'`, `'c'` diventa `'f'` e via dicendo:


Carattere originale     |`'a'`|`'b'`|`'c'`|`'d'`|`'e'`|...|`'x'`|`'y'`|`'z'`|
------------------------|-----|-----|-----|-----|-----|---|-----|-----|-----|
Codifica con chiave 3   |`'d'`|`'e'`|`'f'`|`'g'`|`'h'`|...|`'a'`|`'b'`|`'c'`|

---

Applicando invece la chiave 5 `'a'` diventa `'f'`, `'b'` diventa `'g'`... eccetera:

Carattere originale     |`'a'`|`'b'`|`'c'`|`'d'`|`'e'`|...|`'x'`|`'y'`|`'z'`|
------------------------|-----|-----|-----|-----|-----|---|-----|-----|-----|
Codifica con chiave 5   |`'f'`|`'g'`|`'h'`|`'i'`|`'j'`|...|`'c'`|`'d'`|`'e'`|

---

Scrivi la classe Java `CifrarioDiCesare` che contenga due metodi utili rispettivamente per codificare e decodificare una stringa:

- `public static String codifica(String testo, int chiave)`
- `public static String decodifica(String codice, int chiave)`