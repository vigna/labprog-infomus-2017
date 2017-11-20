Liste a rovescio (lunghezza ignota)
===================================

Descrizione
-----------

Dovete leggere una lista di interi dal flusso di ingresso
e stamparla in ordine inverso.

Vincoli
-------

La lunghezza della lista non è nota. Dovete leggere tutti gli
interi disponibili dal flusso di input.

Esempio
-------

Avendo nel flusso di ingresso

    17
    -1
    0

il programma emette nel flusso di uscita

    0
    -1
    17

Suggerimenti
------------

Potete leggere l'input usando i metodi `hasNextInt()` e
`nextInt()` di `Scanner`. Dato che non sapete in anticipo
quanti interi leggerete, occorre utilizzare un'istanza
di `ArrayList` contenente oggetti involucro di tipo `Integer`.

Per questo programma è bene effettuare le prove utilizzando la
redirezione: create un file `input.txt` contenente le righe di prova, ed
eseguite la vostra soluzione aggiungendo `< input.txt` alla fine della
riga di comando. In questo modo l'input invece che da tastiera arriverà
dal file `input.txt`, facendovi risparmiare tempo e fatica.
