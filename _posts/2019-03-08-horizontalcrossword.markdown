---
layout: post
title: "HorizontalCrossword"
date: 2019-03-08 12:46:57 +0100
categories: [array,methods]
level: 12
---


Scrivi il programma `HorizontalCrossword` contenente i metodi utili per trovare delle *parole nascoste* nelle righe di una matrice.

La classe `HorizontalCrossword` deve contenere i metodi seguenti:

### `public static String reverse(String word)`

Ritorna la stringa `word` *rovesciata*, ad esempio per `"cane"` ritorna `"enac"`.

### `public static String getRowAsString(char[][] table, int row)`

Ritorna la stringa ottenuta concatenando tutti i caratteri presenti nella riga `row` della matrice `table`.


### `public static int searchInRows(char[][] table, String word)`

Ritorna l'indice della riga della matrice `table` che contiene la parola `word` (regolare o *rovesciata*, non sensibile al caso dei caratteri). Se `word` è presente in più righe, ritorna l'indice della prima ricorrenza. Se nessuna riga di `table` contiene `word`, ritorna `-1`.

Ad esempio per la parole "cane" e la matrice seguente il metodo ritorna `1`:

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
    <td class="tg-xldj">a</td>
    <td class="tg-xldj">c</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj"><b>c</b></td>
    <td class="tg-xldj"><b>A</b></td>
    <td class="tg-xldj"><b>n</b></td>
    <td class="tg-xldj"><b>E</b></td>
    <td class="tg-xldj">a</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj">o</td>
    <td class="tg-xldj">N</td>
    <td class="tg-xldj">i</td>
    <td class="tg-xldj">s</td>
    <td class="tg-xldj">N</td>
    <td class="tg-xldj">E</td>
  </tr>
  <tr>
    <td class="tg-xldj">b</td>
    <td class="tg-xldj">E</td>
    <td class="tg-xldj">e</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj">g</td>
    <td class="tg-xldj">a</td>
    <td class="tg-xldj">t</td>
    <td class="tg-xldj">t</td>
    <td class="tg-xldj">E</td>
    <td class="tg-0pky"></td>
  </tr>
</table>

Mentre per questa ritorna `3`:

<table class="tg">
  <tr>
    <td class="tg-xldj">t</td>
    <td class="tg-xldj">O</td>
    <td class="tg-xldj">p</td>
    <td class="tg-xldj">o</td>
    <td class="tg-xldj">C</td>
    <td class="tg-xldj">a</td>
    <td class="tg-xldj">N</td>
  </tr>
  <tr>
    <td class="tg-xldj">F</td>
    <td class="tg-xldj">r</td>
    <td class="tg-xldj">o</td>
    <td class="tg-xldj">g</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj">T</td>
    <td class="tg-xldj">a</td>
    <td class="tg-xldj">n</td>
    <td class="tg-xldj">A</td>
    <td class="tg-xldj">r</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj"><b>e</b></td>
    <td class="tg-xldj"><b>N</b></td>
    <td class="tg-xldj"><b>A</b></td>
    <td class="tg-xldj"><b>c</b></td>
    <td class="tg-xldj">i</td>
    <td class="tg-xldj">o</td>
    <td class="tg-xldj">S</td>
  </tr>
  <tr>
    <td class="tg-xldj">A</td>
    <td class="tg-xldj">g</td>
    <td class="tg-xldj">u</td>
    <td class="tg-xldj">L</td>
    <td class="tg-xldj">e</td>
    <td class="tg-xldj">B</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-xldj">B</td>
    <td class="tg-xldj">o</td>
    <td class="tg-xldj">V</td>
    <td class="tg-xldj">e</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
</table>




### `main`

Contiene il codice utile a verificare e dimostrare il buon funzionamento di tutti i metodi che hai scritto.


