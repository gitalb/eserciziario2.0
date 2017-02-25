---
layout: post
title: "StringTool"
date: 2017-02-25 12:30:05 +0100
categories: [methods,switch,string]
level: 12
---

Scrivi la classe `StringTool` contenente i metodo seguenti:

### longest

~~~java
public static String longest(String a, String b)
~~~
Ritorna la stringa più lunga tra `a`, `b`. Ad esempio `longest("cane","gatto")` ritorna la stringa `gatto`, mentre `longest("abcdef","gatto")` ritorna `abcdef`.

### alternate

~~~java
public static String alternate(String a, String b, int times)
~~~

Ritorna una stringa di testo contenente le stringhe `a` e `b` alternate `times` volte. Ad esempio `alternate("*","-",5)` ritorna la stringa `*-*-*-*-*-`, mentre `alternate("va","Ja",2)` ritorna la stringa `vaJavaJa`.

### concatenate

~~~java
public static String concatenate(int a, int b, int c, char separator, char terminator)
~~~

Ritorna una stringa contenente l'elenco dei valori dei parametri `a`, `b` e `c`. I valori sono separati dal carattere `separator` e la lista è terminata dal carattere `terminator`. Ad esempio `concatenate(1,2,3,';','.')` ritorna la stringa `1;2;3.`, mentre `concatenate(10,20,30,'_','!')` ritorna la stringa `10_20_30!`.w