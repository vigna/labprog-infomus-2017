Stessa lettera
==============

Descrizione
-----------

Dopo una piacevole serata, un folto gruppo di amici si pone la seguente
domanda: quante persone presenti hanno il nome che inizia come il mio?

Per semplificargli la vita, dovete scrivere un programma che legge i nomi
dei partecipanti alla serata e stampa una riga per ogni partecipante. La
riga contiene il nome del partecipante, seguito dai nomi dei partecipanti
il cui nome comincia con la stessa iniziale, separati da uno spazio.

Vincoli
-------

Potete assumere che i nomi siano in minuscolo. L'ordine di output deve
essere uguale all'ordine di input. Su ogni riga, l'ordine dei nomi degli
amici con la stessa iniziale deve essere uguale all'ordine di input.

Esempio
-------

Avendo nel flusso di ingresso

    6
    angelo
    maria
    davide
    marco
    adalgiso
    mattone

il programma emette nel flusso di uscita

    angelo adalgiso
    maria marco mattone
    davide
    marco maria mattone
    adalgiso angelo
    mattone maria marco

Suggerimenti
------------

Potete leggere il primo input (la lunghezza della lista) usando il metodo
`nextInt()` di `Scanner`, e proseguire con il metodo `next()`. Una volta
letta la lunghezza della lista, dovete creare un array di stringhe della
lunghezza data, dove memorizzerete la lista stessa. Utilizzando l'array
è facile ottenere il risultato richiesto.

Per questo programma è bene effettuare le prove utilizzando la
redirezione: create un file `input.txt` contenente le righe di prova, ed
eseguite la vostra soluzione aggiungendo `< input.txt` alla fine della
riga di comando. In questo modo l'input invece che da tastiera arriverà
dal file `input.txt`, facendovi risparmiare tempo e fatica.
