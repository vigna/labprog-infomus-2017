Numeri amichevoli
=================

Descrizione
-----------

Due numeri interi `x` e `y` sono detti _amichevoli_ se la somma dei divisori
propri di ciascuno è uguale all'altro (fra i divisori è compreso l’1 ed escluso
il numero stesso). Ad esempio (220, 284) è una coppia di amichevoli, essendo

    284 = 1 + 2 + 4 + 5 + 10 + 11 + 20 + 22 + 44 + 55 + 110

che sono i divisori di 220, e

    220 = 1 + 2 + 4 + 71 + 142

che sono i divisori di 284.

Gli antichi greci ritenevano che le coppie di numeri amichevoli avessero certe
proprietà mistiche.
Scrivete un programma che, dato un numero `n` inserito dall'utente, stampi
tutte le coppie di numeri amichevoli
`x` e `y` con `x` ≤ `y` ≤ `n`. Un numero può essere anche amico di se stesso,
nel qual caso è detto _perfetto_.

Vincoli
-------

Il numero in ingresso è strettamente positivo.

Esempio
-------

Avendo nel flusso di ingresso

    500

il programma emette nel flusso di uscita

    6 6
    28 28
    220 284

Suggerimenti
------------

Potete leggere l'input tramite

    int n = s.nextInt();

dove `s` è una variabile di tipo `Scanner` opportunamente inizializzata.

Notate che vi occorre sapere la somma dei divisori di un numero _due volte_:
scrivete prima un metodo statico che prende un numero e restituisce la somma
dei suoi divisori propri. Poi, chiamate il metodo due volte all'interno di un
ciclo.
