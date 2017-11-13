Il crivello di Eratostene
=========================

Descrizione
-----------

Il crivello di Eratostene è un algoritmo antico per determinare i numeri
primi fino a un dato intero `n`. L’algoritmo utilizza un array di
variabili booleane (inizializzate a `true`) che nella posizione `i`
conterrà alla fine il valore di verità “`i` è primo”.

L’algoritmo itera sugli elementi dell'array a partire dalla posizione 2, e
ogni volta che trova in posizione `p` il valore vero (cioè il numero `p` è
fino a quel punto stimato primo) imposta a falso i valori dell'array in
posizioni multiple di `p`, cioè `2p`, `3p`, eccetera (fino al limite `n`).
Alla fine, si scandisce l'array a partire dalla posizione due e si
stampano tutte le posizioni il cui valore è vero.

Dovete scrivere un programma che legge il limite `n` dal flusso di ingresso
e stampa i numeri primi fino a `n`, separati da uno spazio.

Esempio
-------

Avendo nel flusso di ingresso

    10

il programma emette nel flusso di uscita

    2 3 5 7

mentre avendo nel flusso di ingresso

    100

il programma emette nel flusso di uscita

    2 3 5 7 11 13 17 19 23 29 31 37 41 43 47 53 59 61 67 71 73 79 83 89 97

Suggerimenti
------------

Il programma richiede due cicli annidati: il primo scandisce le posizioni
del vettore alla ricerca di quelle impostate a vero; il secondo mette a
falso le posizioni multiple di quelle trovate.
