---
layout: post
title: "Asciigator"
date: 2017-02-25 12:06:45 +0100
categories: [interactive,unicode,string,loop]
level: 9
---

Scrivere la classe `Asciigator` che chiede all'utente di digitare un stringa di testo e poi stampa ogni carattere contenuto nella stringa introdotta e il relativo codice Unicode (in decimale e in esadecimale). 

Ad esempio per `ABCDEF1234567890` il programma produce l'output seguente:

~~~text
Introdurre un testo:
ABCDEF1234567890

char:	'A'	'B'	'C'	'D'	'E'	'F'	'1'	'2'	'3'	'4'	'5'	'6'	'7'	'8'	'9'	'0'	
dec:	65	66	67	68	69	70	49	50	51	52	53	54	55	56	57	48	
hex:	41	42	43	44	45	46	31	32	33	34	35	36	37	38	39	30	

~~~

Mentre per `Hello world!`:

~~~text
Introdurre un testo:
Hello world!

char:	'H'	'e'	'l'	'l'	'o'	' '	'w'	'o'	'r'	'l'	'd'	'!'	
dec:	72	101	108	108	111	32	119	111	114	108	100	33	
hex:	48	65	6c	6c	6f	20	77	6f	72	6c	64	21

~~~