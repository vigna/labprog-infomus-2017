Numeri perfetti
===============

Descrizione
-----------

Un numero è _perfetto_ se è uguale alla somma dei suoi divisori propri. Per
esempio, 6 = 1 + 2 + 3 è perfetto.
Scrivete un programma che, dato un intero in input, scriva i numeri perfetti
minori dell'intero dato.

Vincoli
-------

Il numero in ingresso è strettamente positivo.

Esempio
-------

Avendo nel flusso di ingresso

    10

il programma emette nel flusso di uscita

    6

mentre avendo nel flusso di ingresso

    100

il programma emette nel flusso di uscita

    6
    28

Suggerimenti
------------

Potete leggere l'input tramite

    int n = s.nextInt();

dove `s` è una variabile di tipo `Scanner` opportunamente inizializzata.

Notate che vi occorrono due cicli: uno per scandire i numeri fino a `n`, e uno
annidato per sommare i divisori. Ancora meglio: scrivete prima un metodo
statico che prende un numero e restituisce la somma dei suoi divisori.
Poi, chiamate il metodo all'interno di un ciclo.
