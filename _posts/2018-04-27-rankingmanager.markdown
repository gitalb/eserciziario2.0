---
layout: post
title: "RankingManager"
date: 2018-04-27 12:13:40 +0100
categories: [class, files]
level: 14
---


# `Record` e `RankingManager`

## `Record`

La classe `Record` è  utilizzata per rappresentare i dati di un *record* nella classifica di un videogioco. La classe è molto semplice; possiede solo i due attributi privati `name` (il nome del giocatore che ha fatto il record) e `points` (i punti totalizzati). Entrambi gli attributi sono accessibili in sola lettura. 

La classe `Record` esporta pure il *costruttore personalizzato* che permette di inizializzare `name` e `points` (in questo ordine). 

Inoltre `Record` esporta e il metodo `String toString()` che ne ritorna la rappresentazione testuale nel formato:

~~~
<name>: <points>
~~~

Esempio:

~~~
Luigi: 10000
~~~

## `RankingManager`

Serve per caricare i record salvati in un file CSV e per trovare il giocatore con il punteggio più alto. 

I record sono memorizzati nella *lista di Record* `records` (attributo privato `List<Record>`).

La classe `RankingManager` esporta i seguenti metodi:

### Costruttore

~~~java
public RankingManager(Path csvPath)
~~~

Il costruttore personalizzato permette di definire il percorso del file CSV. 

### `loadRanking`

~~~java
public void loadRanking()
~~~

Carica i dati dal file CSV. Se non è possibile accedere o leggere il file, solleva una `IOException`. Le righe del file CSV che contengono dati non validi non vengono importate. 

### `getRecords`

~~~java
public List<Record> getRecords
~~~

Ritorna la lista (`records`) dei record caricati dal file CSV.

### `getWinner`

~~~java
public Record getWinner()
~~~

Ritorna il `Record` con il punteggio più alto in `records`. Se la lista è vuota ritorna `null`. 

## Formato del file CSV

Su ogni riga del file CSV deve essere registrato un record nel formato:

~~~
<name>,<points>
~~~

Dove:

- `<name>`: stringa *non vuota*, deve contenere almeno un carattere diverso da ' ' (blank) 
- `<points>`: numero intero

Tutte le righe che non rispettano questo formato sono considerate non valide e vengono ignorate dal metodo `loadRanking`.

Ad esempio un file CSV valido potrebbe contenere i dati seguenti:

~~~
Mario,50
Alb,-200
Luigi,10000
Zorro,0
Pippo,400
~~~

