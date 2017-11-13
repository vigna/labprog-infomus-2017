Liste a rovescio
================

Descrizione
-----------

Dovete leggere una lista di interi dal flusso di ingresso
e stamparla in ordine inverso. Il primo numero in input è la lunghezza
`n` della lista di numeri. Seguono `n` numeri interi.

Esempio
-------

Avendo nel flusso di ingresso

    3
    17
    -1
    0

il programma emette nel flusso di uscita

    0
    -1
    17

Suggerimenti
------------

Potete leggere l'input usando il metodo `nextInt()` di `Scanner`.
Una volta letta la lunghezza della lista, dovete creare un array
di interi della lunghezza data, dove memorizzerete la lista stessa.
Alla fine, dovrete scorrere l'array al contrario e stamparlo.

Per questo programma è bene effettuare le prove utilizzando la
redirezione: create un file `input.txt` contenente le righe di prova, ed
eseguite la vostra soluzione aggiungendo `< input.txt` alla fine della
riga di comando. In questo modo l'input invece che da tastiera arriverà
dal file `input.txt`, facendovi risparmiare tempo e fatica.
