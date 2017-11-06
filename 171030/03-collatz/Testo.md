Collatz
=======

Descrizione
-----------

Considerate la seguente regola: dato un numero intero positivo `n`, se `n` è
pari lo si divide per 2, se è dispari lo si moltiplica per 3 e si aggiunge
1 al risultato. Quando `n` è 1 ci si ferma. Questa semplice regola permette
di costruire delle sequenze: la sequenza che si costruisce a partire dal
numero `n` è detta sequenza di Collatz di `n`. Ad esempio, la sequenza di
Collatz di 7 è:

    7 22 11 34 17 52 26 13 40 20 10 5 16 8 4 2 1

È un noto problema aperto stabilire se ogni sequenza di Collatz termina
(cioè, se arriva a 1). Scrivete un programma che chiede all'utente un
numero e mostra la sequenza di Collatz del numero (con tanto di lunghezza).

Vincoli
-------

Il numero in ingresso è strettamente positivo. Il formato in uscita
è quello mostrato nell'esempio, e deve essere seguito strettamente.

Esempio
-------

Avendo nel flusso di ingresso

    7

il programma emette nel flusso di uscita

    sequenza: 7 22 11 34 17 52 26 13 40 20 10 5 16 8 4 2 1
    lunghezza: 17

mentre avendo nel flusso di ingresso

    8

il programma emette nel flusso di uscita

    sequenza: 8 4 2 1
    lunghezza: 4

Suggerimenti
------------

Potete leggere l'input tramite

    int n = s.nextInt();

dove `s` è una variabile di tipo `Scanner` opportunamente inizializzata.
