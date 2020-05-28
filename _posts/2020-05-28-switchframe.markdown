---
layout: post
title: "SwitchFrame"
date: 2020-05-27  9:37:37 +0100
categories: [gui]
level: 16
---


Devi realizzare l'applicazione Swing `SwitchFrame` secondo le specifiche descritte in seguito. 

## Architettura

![]({{ site.baseurl }}/assets/posts/switchframe/switch.svg)


L'applicazione è costituita dalle classi e dalla *interface* rappresentate nel diagramma (che puoi completare aggiungendo metodi e attributi se lo reputi necessario):

- `SwitchFrame`: è il frame principale dell'applicazione.
- `Switch`: simula il comportamento di un interruttore.
- `SwitchListener`: è una `interface` che definisce l'interazione tra un interruttore (`Switch`) e i sui *ascoltatori* (`SwitchListener`).

## Classe `Switch`

La classe `Switch` rappresenta il modello astratto di un *interruttore*. Un interruttore è e rappresentato graficamente da un rettangolo (spessore bordo 10 pixel) e può essere acceso:

![]({{ site.baseurl }}/assets/posts/switchframe/on.png)


oppure spento:


![]({{ site.baseurl }}/assets/posts/switchframe/off.png)


La posizione e le dimensioni dell'interruttore sono definite dagli attributi `x`, `y`,`width` e `height`. La classe esporta pure il metodo `paint` che disegna l'interruttore e il metodo `contains` utile per determinare se un punto (`java.awt.Point`) si trova all'interno dell'area dell'interruttore.

### Eventi della classe `Switch`

Gli eventi generati da un interruttore sono definiti dalla *interface* `SwitchListener`.

#### Eventi `mouseEntered` e `mouseExited`
Il metodo `mouseEntered` viene invocato quando il puntatore del mouse **entra nella superficie dell'interruttore**. Quando ciò avviene, il bordo dell'interruttore diventa arancio.


Il metodo `mouseExited ` viene invocato quando il puntatore del mouse **esce dalla superficie dell'interruttore**. Quando ciò avviene, il bordo dell'interruttore ritorna nero.

<video controls="controls" width="200" name="Video Name" src="{{ site.baseurl }}/assets/posts/switchframe/over.mp4"></video>

#### Evento `switchToggled`
Il metodo `switchToggled` viene invocato quando lo stato di un interruttore cambia. Per accendere e spegnere un interruttore bisogna cliccare la superficie dell'interruttore con il **tasto destro** del mouse. Se l'interruttore è spento, la parte centrale dell'interruttore è di colore rosso, altrimenti verde:

<video controls="controls" width="200" name="Video Name" src="{{ site.baseurl }}/assets/posts/switchframe/onoff.mp4"></video>


## Classe `SwitchFrame`

È una semplice GUI che utilizza 9 istanze di `Switch`:

<video controls="controls" width="200" name="Video Name" src="{{ site.baseurl }}/assets/posts/switchframe/switchframe.mp4"></video>

Le 9 istanze sono disposte su di una *griglia* di 3 righe e 3 colonne (margine laterale e inferiore 20 pixel, superiore 40 pixel), hanno larghezza e altezza pari a 100 pixel e sono distanziate di 20 pixel le una dalle altre.

