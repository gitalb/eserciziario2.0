---
layout: post
title: "StringFormatter"
date: 2026-05-29  9:01:00 +0100
categories: [loops, string]
level: 12
---

Scrivi la classe `StringFormatter` contenente il metodo:

~~~java
public static String reformat(String text)
~~~

Tale ritorna la stringa `text` *formattandola* secondo le regole seguenti:

1. il carattere *a capo* non è ammesso
2. non ci sono *spazi* (`' '`) all'inizio e alla fine del testo
3. non ci sono *spazi multipli*
4. non ci sono *spazi* prima di un carattere di punteggiatura (`'.'`, `','`, `';'`, `':'`, `'!'`, `'?'`)
5. dopo un carattere di punteggiatura c'è sempre uno spazio, a meno che:
	- sia l'ultimo carattere del testo (regola 2.)
	- sia seguito da un altro carattere di punteggiatura (regola 4.)

Ad esempio per un file contenente il testo:

~~~text
  John,Malkovich?John   : Malkovich!!! !
     John     Malkovich   !? !?John;Malkovich .   .    .  
~~~

il metodo `reformat` ritorna la stringa:

~~~text
John, Malkovich? John: Malkovich!!!! John Malkovich!?!? John; Malkovich...
~~~
