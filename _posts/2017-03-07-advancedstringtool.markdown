---
layout: post
title: "AdvancedStringTool"
date: 2017-03-07  8:01:14 +0100
categories: [string,methods,switch,loop]
level: 13
---


Scrivi la classe `AdvancedStringTool` contenente i metodi desctitti in seguito:

### isLetter

~~~java
public static boolean isLetter(char c)
~~~

Ritorna `true` se il carattere `c` è una lettera, mentre ritorna `false` In caso contrario.

### isConsonant
~~~java
public static boolean isConsonant(char c)
~~~

Ritorna `true` se il carattere `c` è una consonante, `false` altrimenti.

### isVowel
~~~java
public static boolean isVowel(char c)
~~~

Ritorna `true` se `c` è una vocale, mentre ritorna `false` in tutti gli altri casi.

### countVowels

~~~java
public static int countVowels(String text)
~~~

Ritorna il numero di vocali presenti nella stringa `text`. Ad esempio `countVowels("NOOOOOO")` ritorna 6.

### countConsonants
~~~java
public static int countConsonants(String text)
~~~

Tale metodo ritorna il numero di consonanti presenti nella stringa `text`. Ad esempio `countConsonants("NOOOOOO")` ritorna 1.

### vowelize

~~~java
public static String vowelize(String text)
~~~

Ritorna una stringa contenente solamente le vocali della stringa `text`. Ad esempio `vowelize("casa")` ritorna `"aa"`, mentre `vowelize("lunotto")` ritorna `"uoo"`.

### isAlternative

~~~java
public static boolean isAlternative(String s)
~~~

Tale metodo ritorna true se la stringa `s` contiene consonanti e vocali alternate (es. `isAlternative("patata")` ritorna `true`).

### countInString

~~~java
public static int countInString(String text, char c)
~~~

Tale metodo conta quante volte il carattere `c` è presente nella stringa `text`.


### isAnagram

~~~java
public static boolean isAnagram(String firstWord, String secondWord)
~~~

Ritorna `true` se `firstWord` è un anagramma di `secondWord`, altrimenti ritorna `false`. Esempio `isAnagram("calendario","locandiera")` ritorna `true`.
