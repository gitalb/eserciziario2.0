---
layout: post
title: "EmployeeManager"
date: 2018-04-27 11:41:36 +0100
categories: [class, files]
level: 14
---


# `Employee` e `EmployeeManager`

## `Employee` 

La classe `Employee` è  utilizzata per rappresentare i dati di un impiegato aziendale e il suo stipendio. La classe è molto semplice; possiede solo i due attributi privati `name` (il nome dell'impiegato) e `salary` (lo stipendio dell'impiegato [`double`]). Entrambi gli attributi sono accessibili in sola lettura. 

La classe `Employee ` esporta pure il costruttore personalizzato che permette di inizializzare `name` e `salary` (in questo ordine). 

Inoltre `Employee` esporta e il metodo `boolean equals(Employee e)` che ritorna `true` se i due impiegati confrontati posseggono lo stesso nome (ignora maiuscole e minuscole) e lo stesso stipendio.


## `EmployeeManager`

Serve per caricare i dati riguardanti gli impiegati da un file CSV e per trovare la media degli stipendi.

I dati sono memorizzati nella *lista di Employee* `employees` (attributo privato `List<Employee>`).

La classe `EmployeeManager` esporta i seguenti metodi:

### Costruttore

~~~java
public EmployeeManager(String csvPath)
~~~

Il costruttore personalizzato permette di definire il percorso del file CSV.

### `loadEmployees`

~~~java
public void loadEmployees()
~~~

Carica i dati dal file CSV. Se non è possibile accedere o leggere il file, solleva una `IOException`. Le righe del file CSV che contengono dati non validi non vengono importate. 

### `getEmployees`

~~~java
public List<Employee> getEmployees()
~~~

Ritorna la lista (`employees `) degli impiegati.

### `getAverageSalary`

~~~java
public double getAverageSalary()
~~~

Ritorna lo stipendio medio (tra tutti quelli contenuti in `employees`). Se la lista è vuota ritorna `-1.0`. 

## Formato del file CSV

Su ogni riga del file CSV deve essere registrato un impiegato nel formato:

~~~
<salary>;<name>
~~~

Dove:

- `<salary>`: numero `double`
- `<name>`: stringa *non vuota*, deve contenere almeno un carattere diverso da `' '` (blank) 

Tutte le righe che non rispettano questo formato sono considerate come non valide e vengono ignorate dal metodo `loadEmployees`.

Ad esempio un file CSV valido potrebbe contenere i dati seguenti:

~~~
1250.5;Mario
200;Alb
1000.5;Luigi
8230.25;Zorro
400;Pippo

~~~

