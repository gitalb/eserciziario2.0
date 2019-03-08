---
layout: post
title: "VerticalCrossword"
date: 2019-03-08 12:59:00 +0100
categories: [array,methods]
level: 12
---


Scrivi il programma `VerticalCrossword` contenente i metodi utili per trovare delle *parole nascoste* nelle colonne di una matrice.

La classe `VerticalCrossword` deve contenere i metodi seguenti:


### `public static int getMaxWidth(char[][] table)`

Ritorna la dimensione della *riga più larga* (con il maggior numero di colonne) contenuta nella matrice `table`.


### `public static String getColAsString(char[][] table, int col)`

Ritorna la stringa ottenuta concatenando tutti i caratteri presenti nella colonna `col` della matrice `table`. Le righe troppo corte per possedere un carattere nella colonna specificata da `col` vengono ignorate. Ad esempio, per la matrice seguente e per `col` pari a `3`, il metodo ritorna la stringa `"CaNe"`:


<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;margin:0px auto;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:0px;overflow:hidden;word-break:normal;}
.tg .tg-xldj{border-color:inherit;text-align:left;border-style:solid;border-width:1px}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top;border-style:solid;border-width:0px}
</style>
<table class="tg">
  <tr>
    <td class="tg-xldj">c</td>
    <td class="tg-xldj">C</td>
    <td class="tg-xldj">e</td>
    <td class="tg-xldj"><b>C</b></td>
    <td class="tg-xldj">c</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj">c</td>
    <td class="tg-xldj">a</td>
    <td class="tg-xldj">n</td>
    <td class="tg-xldj"><b>a</b></td>
    <td class="tg-xldj">a</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj">c</td>
    <td class="tg-xldj">p</td>
    <td class="tg-xldj">a</td>
    <td class="tg-xldj"><b>N</b></td>
    <td class="tg-xldj">n</td>
    <td class="tg-xldj">E</td>
  </tr>
  <tr>
    <td class="tg-xldj">a</td>
    <td class="tg-xldj">e</td>
    <td class="tg-xldj">e</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj">a</td>
    <td class="tg-xldj">b</td>
    <td class="tg-xldj">c</td>
    <td class="tg-xldj"><b>e</b></td>
    <td class="tg-xldj">e</td>
    <td class="tg-0pky"></td>
  </tr>
</table>

### `public static int searchInCols(char[][] table, String word)`

Ritorna l'indice della colonna della matrice `table` che contiene la parola `word` (non sensibile al caso dei caratteri). Se `word` è presente in più colonne, ritorna l'indice della prima ricorrenza. Se nessuna colonna di `table` contiene `word`, ritorna `-1`.

Ad esempio per la parola `"cane"` e la matrice seguente il metodo ritorna `3`:



<table class="tg">
  <tr>
    <td class="tg-xldj">c</td>
    <td class="tg-xldj">C</td>
    <td class="tg-xldj">e</td>
    <td class="tg-xldj"><b>C</b></td>
    <td class="tg-xldj">c</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj">c</td>
    <td class="tg-xldj">a</td>
    <td class="tg-xldj">n</td>
    <td class="tg-xldj"><b>a</b></td>
    <td class="tg-xldj">a</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj">c</td>
    <td class="tg-xldj">p</td>
    <td class="tg-xldj">a</td>
    <td class="tg-xldj"><b>N</b></td>
    <td class="tg-xldj">n</td>
    <td class="tg-xldj">E</td>
  </tr>
  <tr>
    <td class="tg-xldj">a</td>
    <td class="tg-xldj">e</td>
    <td class="tg-xldj">e</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj">a</td>
    <td class="tg-xldj">b</td>
    <td class="tg-xldj">c</td>
    <td class="tg-xldj"><b>e</b></td>
    <td class="tg-xldj">e</td>
    <td class="tg-0pky"></td>
  </tr>
</table>

Mentre per questa matrice e `"BAU"` ritorna `1`:

<table class="tg">
  <tr>
    <td class="tg-xldj">G</td>
    <td class="tg-xldj">a</td>
    <td class="tg-xldj">t</td>
    <td class="tg-xldj">t</td>
    <td class="tg-xldj">o</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj">r</td>
    <td class="tg-xldj"><b>b</b></td>
    <td class="tg-xldj">a</td>
    <td class="tg-xldj">u</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj">R</td>
    <td class="tg-xldj"><b>A</b></td>
    <td class="tg-xldj">p</td>
    <td class="tg-xldj">U</td>
    <td class="tg-xldj">n</td>
    <td class="tg-xldj">Z</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj">r</td>
    <td class="tg-xldj"><b>u</b></td>
    <td class="tg-xldj">p</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
</table>


### `main`

Contiene il codice utile a verificare e dimostrare il buon funzionamento di tutti i metodi che hai scritto.

