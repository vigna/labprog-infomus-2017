Garibaldi fu ferito
===================

Descrizione
-----------

Scrivete un programma che legga delle righe in input e le stampi dopo aver
sostituito tutte le vocali con delle “u”. Il programma si deve fermare quando
viene premuto Control-D  per chiudere il flusso di ingresso.

Esempio
-------

Avendo nel flusso di ingresso

    mamma mia
    bella aiuola
    Garibaldi fu ferito
    Addio, monti SORGENTI

il programma emette nel flusso di uscita

    mummu muu
    bullu uuuulu
    Gurubuldu fu furutu
    Udduu, muntu SURGUNTU

Suggerimenti
------------

Potete leggere l'input in un ciclo `while` controllato dal valore restituito
dal metodo `s.hasNextLine()` tramite l'istruzione

    String l = s.nextLine();

dove `s` è una variabile di tipo `Scanner` opportunamente inizializzata.

Utilizzate l’istruzione `switch` per scrivere un metodo statico che accetti un
carattere e lo restituisca trasformato opportunamente, e chiamate il metodo
all'interno di un ciclo che scorre i caratteri della riga corrente.

Per questo programma è bene effettuare le prove utilizzando la
redirezione: create un file `input.txt` contenente le righe
di prova, ed eseguite la vostra soluzione aggiungendo `< input.txt`
alla fine della riga di comando. In questo modo l'input invece
che da tastiera arriverà dal file `input.txt`, facendovi risparmiare
tempo e fatica.
