---
layout: post
title: "TableParser"
date: 2018-03-29  8:20:43 +0100
categories: [files, loops]
level: 12
---

Scrivi la classe `TableParser` contenente il metodo:

~~~java
public static void convertTable(Path htmlFile, Path csvFile)
~~~

Tale metodo legge il file in formato HTML `htmlFile`. Se nel file HTML è contenuta almeno una tabella, il metodo converte il contenuto della prima tabella contenuta nel file in formato CSV e lo salva nel file `csvFile`.

La conversione avviene secondo le regole seguenti:

- i commenti html vengono ignorati (`<!---`,`--->`)
- solo la prima tabella viene esportata
- la tabella è delimitata dai tag html `<table>` e `</table>`
- ogni riga è delimitata dai tag html `<tr>` e `</tr>`
- ogni colonna è delimitata dai tag html `<td>` e `</td>`
- le tabelle non hanno header (non sono presenti tag `<th>` e `</th>`)
- se il file HTML non è accessibile, se non contiene nessuna tabella, se la tabella non contiene righe o colonne, non viene generato nessun file csv.

Ad esempio per un file html contenente:

~~~html
...
<h1>Tabella di test</h1>
<p>Prova a convertire la seguente tablella:</p>
<!-- Questo è un commento -->
<table><!-- Qui inizia la tabella -->
    <tr><!-- Prima riga -->
        <td>A</td><td>B</td><td>C</td><td>D</td>
    </tr>
    <tr><!-- Prima riga -->
        <td>1</td><td>1234</td><td>cane<!--- BAU!!! --->
        </td><td>gatto</td>
    </tr>
</table><!-- Qui termina la tabella -->
...
~~~

Verrà prodotto il seguente file CSV:

~~~text
A;B;C;D;
1;1234;cane;gatto;
~~~

