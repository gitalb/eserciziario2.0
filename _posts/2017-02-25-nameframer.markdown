---
layout: post
title: "NameFramer"
date: 2017-02-25 12:36:50 +0100
categories: [methods,loop,string,draw]
level: 13
---


Scrivi la classe `NameFramer` contenente il metodo:

~~~java
pubic static String frameName(String name, char c, int width)
~~~

che ritorna una stringa contenente la stringa `name` incorniciata nel carattere `c` utilizzato con uno spessore `width`.

Ad esempio `frameName("Piero",'*',2)` ritorna la stringa:

~~~text
*********
*********
**Piero**
*********
*********
~~~


mentre `frameName("Andrea",'$',1)` ritorna la stringa:

~~~text
$$$$$$$$
$Andrea$
$$$$$$$$
~~~