Bandiera
========

Descrizione
-----------

Scrivete un programma che, letto un numero intero `n`, emetta in output una
bandiera di `n` + 1 righe costituite ciascuna da `n` caratteri contenente il
motivo diagonale mostrato negli esempi.

Vincoli
-------

Il numero in ingresso è strettamente positivo.

Esempio
-------

Avendo nel flusso di ingresso

    4

il programma emette nel flusso di uscita

    ++++
    *+++
    **++
    ***+
    ****

mentre avendo nel flusso di ingresso

    5

il programma emette nel flusso di uscita

    +++++
    *++++
    **+++
    ***++
    ****+
    *****

Suggerimenti
------------

Potete leggere l'input tramite

    int n = s.nextInt();

dove `s` è una variabile di tipo `Scanner` opportunamente inizializzata.
