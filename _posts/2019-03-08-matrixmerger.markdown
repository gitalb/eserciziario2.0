---
layout: post
title: "MatrixMerger"
date: 2019-03-08 12:32:22 +0100
categories: [array,methods]
level: 12
---


Scrivi il programma `MatrixMerger` contenente i metodi utili per *combinare tra loro* due matrici di interi. 

La classe `MatrixMerger` deve contenere i metodi seguenti:

### `public static int getRowWidth(int[][] m, int row)`

Ritorna la larghezza (*il numero di colonne*) della riga `row` nella matrice `m`. Se la riga specificata è vuota oppure non è valida, ritorna `0`.


### `public static int getMaxWidth(int[][] a, int[][] b)`

Ritorna la *dimensione* della riga più larga che si otterrebbe combinando ogni riga di `a` con la rispettiva riga di `b`. Ossia, calcola la somma tra la dimensione di ogni riga della matrice `a` con la rispettiva riga della matrice `b` e ritorna il valore massimo.




### `public static int[][] merge(int[][] a, int[][] b)`


Ritorna una matrice rettangolare ottenuta combinando le matrici `a` e `b`. La combinazione avviene concatenando ogni riga di `a` con la rispettiva riga di `b`. La nuova matrice avrà un numero di righe pari a quello della matrice *più alta* tra `a` e `b` ed un numero di colonne pari a quella della riga più larga prodotta dalla concatenazione (*larghezza massima* di `a` e `b`). Ad esempio:


<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;margin:0px auto;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:0px;overflow:hidden;word-break:normal;}
.tg .tg-xldj{border-color:inherit;text-align:left;border-style:solid;border-width:1px}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top;border-style:solid;border-width:0px}
</style>
<table class="tg">
  <tr>
    <td class="tg-xldj">1</td>
    <td class="tg-xldj">2</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-xldj">3</td>
    <td class="tg-xldj">4</td>
    <td class="tg-xldj">5</td>
    <td class="tg-xldj">6</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-xldj">1</td>
    <td class="tg-xldj">2</td>
    <td class="tg-xldj">3</td>
    <td class="tg-xldj">4</td>
    <td class="tg-xldj">5</td>
    <td class="tg-xldj">6</td>
  </tr>
  <tr>
    <td class="tg-xldj">1</td>
    <td class="tg-xldj">2</td>
    <td class="tg-xldj">3</td>
    <td class="tg-xldj">4</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">+</td>
    <td class="tg-0pky"></td>
    <td class="tg-xldj">5</td>
    <td class="tg-xldj">6</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">=</td>
    <td class="tg-0pky"></td>
    <td class="tg-xldj">1</td>
    <td class="tg-xldj">2</td>
    <td class="tg-xldj">3</td>
    <td class="tg-xldj">4</td>
    <td class="tg-xldj">5</td>
    <td class="tg-xldj">6</td>
  </tr>
  <tr>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-xldj">1</td>
    <td class="tg-xldj">2</td>
    <td class="tg-xldj">3</td>
    <td class="tg-xldj">4</td>
    <td class="tg-xldj">5</td>
    <td class="tg-xldj">6</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-xldj">1</td>
    <td class="tg-xldj">2</td>
    <td class="tg-xldj">3</td>
    <td class="tg-xldj">4</td>
    <td class="tg-xldj">5</td>
    <td class="tg-xldj">6</td>
  </tr>
</table>



Se presenti, le celle *in eccesso* di ogni riga conterranno il valore `0`, ad esempio:



<table class="tg">
  <tr>
    <td class="tg-xldj">1</td>
    <td class="tg-xldj">1</td>
    <td class="tg-xldj">1</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-xldj">5</td>
    <td class="tg-xldj">5</td>
    <td class="tg-xldj">5</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-xldj">1</td>
    <td class="tg-xldj">1</td>
    <td class="tg-xldj">1</td>
    <td class="tg-xldj">5</td>
    <td class="tg-xldj">5</td>
    <td class="tg-xldj">5</td>
  </tr>
  <tr>
    <td class="tg-xldj">2</td>
    <td class="tg-xldj">2</td>
    <td class="tg-xldj">2</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">+</td>
    <td class="tg-0pky"></td>
    <td class="tg-xldj">6</td>
    <td class="tg-xldj">6</td>
    <td class="tg-xldj">6</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">=</td>
    <td class="tg-0pky"></td>
    <td class="tg-xldj">2</td>
    <td class="tg-xldj">2</td>
    <td class="tg-xldj">2</td>
    <td class="tg-xldj">6</td>
    <td class="tg-xldj">6</td>
    <td class="tg-xldj">6</td>
  </tr>
  <tr>
    <td class="tg-xldj">3</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-xldj">7</td>
    <td class="tg-xldj">7</td>
    <td class="tg-xldj">7</td>
    <td class="tg-xldj">7</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-xldj">3</td>
    <td class="tg-xldj">7</td>
    <td class="tg-xldj">7</td>
    <td class="tg-xldj">7</td>
    <td class="tg-xldj">7</td>
    <td class="tg-xldj"><b>0</b></td>
  </tr>
  <tr>
    <td class="tg-xldj">4</td>
    <td class="tg-xldj">4</td>
    <td class="tg-xldj">4</td>
    <td class="tg-xldj">4</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-xldj">4</td>
    <td class="tg-xldj">4</td>
    <td class="tg-xldj">4</td>
    <td class="tg-xldj">4</td>
    <td class="tg-xldj"><b>0</b></td>
    <td class="tg-xldj"><b>0</b></td>
  </tr>
</table>


### `main`

Contiene il codice utile a verificare e dimostrare il buon funzionamento di tutti i metodi che hai scritto.

