---
layout: post
title: "HelloPeople"
date: 2024-09-09 10:26:15 +0100
categories: [primipassi, args, loop, switch, string, draw]
level: 5
---

Scrivi il programma `HelloPeople` che riceve `N` nomi come argomenti da linea di comando e poi stampa altrettanti omini stilizzati. Sotto ogni omino compare il relativo nome.

Ad esempio per `"Luigi Michele"` il programma stampa due omini:

```text
\o/     \o/     
 |       |      
/ \     / \     
Luigi   Michele
```

Invece per `"Simone Luigi Pincopallino  Michele Joe"`:

```text
\o/          \o/          \o/          \o/          \o/          
 |            |            |            |            |           
/ \          / \          / \          / \          / \          
Simone       Luigi        Pincopallino Michele      Joe
```

Se non vengono forniti argomenti, il programma termina senza stampare niente.