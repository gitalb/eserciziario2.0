---
layout: post
title: "MailParser"
date: 2022-10-23 11:05:36 +0100
categories: [string]
level: 3
---


Il sistema di messaggistica scolastico deve ricavare il nome e il cognome dei docenti a partire dall'indirizzo email. Ogni indirizzo di posta elettronica è composto dal nome e dal cognome del docente separati da un punto e dal domino nel formato: 

	
		<nome>.<cognome>@edu.ti.ch


Scrivi la classe Java `MailParser` che, dato l'indirizzo di posta elettronica del docente memorizzato in una **costante**, stampi a terminale i relativi nome e cognome. Il formato dell'output deve rispettare rigorosamente quello proposto nei seguenti esempi:

Per "HAiEiE.braZoRf@edu.ti.ch" il programma stampa:

~~~
	Email: HAiEiE.braZoRf@edu.ti.ch
	Nome: Haieie
	Cognome: Brazorf
~~~

Per "Mickey.Mouse@edu.ti.ch":

~~~
	Email: Mickey.Mouse@edu.ti.ch
	Nome: Mickey
	Cognome: Mouse
~~~

Per "vladimir.harkonnen@edu.ti.ch":

~~~
	Email: vladimir.harkonnen@edu.ti.ch
	Nome: Vladimir
	Cognome: Harkonnen
~~~