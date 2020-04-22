---
layout: post
title: "JKFlipFlop"
date: 2020-04-21  8:07:03 +0100
categories: [junit]
level: 14
---

Considera la classe `JKFlipFlop` che simula il funzionamento di un *flip-flop JK edge-triggered*. 

![JK FF]({{ site.baseurl }}/assets/posts/jkff.png)

L’interazione con gli ingressi `J` e `K` del flip-flop avviene tramite i metodi:

~~~java
public void setJ(boolean j)

public void setK(boolean k)
~~~


Il triggering del flip-flop è prodotto dal metodo che simula un impulso di clock:

~~~java
public void clock()
~~~

Lo stato del flip-flop è accessibile attraverso il metodo:

~~~java
public boolean getQ()
~~~

La logica di funzionamento del FF JK é riassunta nella seguente tabella:

| J    | K    |C     |Q     |      |
|:----:|:----:|:----:|:----:|:----:|
| 0 | 0 | &#8593; | Q<sub>0</sub> | NC |
| 0 | 1 | &#8593; | 0 | RESET |
| 1 | 0 | &#8593; | 1 | SET |
| 1 | 1 | &#8593; | !Q<sub>0</sub> | TOGGLE |


L’istanziazione dei flip-flop è possibile esclusivamente tramite il costruttore vuoto; inizialmente i flip-flop si trovano nello stato RESET (Q=0).


Dovrai:

- Definire i casi di test per la classe `JKFlipFlop`, per ognuno di essi dovrai fornire:
	- procedimento
	- risultati attesi
- Implementare la classe `JKFlipFlop` 
- Implementare i test per la classe `JKFlipFlop` utilizzando il framework `JUnit` in modo appropriato