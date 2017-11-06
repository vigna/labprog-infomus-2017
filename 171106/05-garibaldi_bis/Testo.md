Garibaldi fu ferito (la vendetta)
=================================

Descrizione
-----------

Scrivete un programma che legga delle righe in input e le stampi dopo aver
sostituito tutte le vocali con la prima vocale che compare in ogni riga.  Il
programma si deve fermare quando viene premuto
Control-D per chiudere il flusso di ingresso.

Esempio
-------

Avendo nel flusso di ingresso

    mamma mia
    bella aiuola
    Garibaldi fu ferito
    Addio, monti SORGENTI

il programma emette nel flusso di uscita

    mamma maa
    belle eeeele
    Garabalda fa farata
    Addaa, manta SARGANTA

Suggerimenti
------------

Potete leggere l'input in un ciclo `while` controllato dal valore
restituito dal metodo `s.hasNextLine()`, tramite l'istruzione

    String l = s.nextLine();

dove `s` è una variabile di tipo `Scanner` opportunamente inizializzata.

Utilizzate l’istruzione `switch` per scrivere un metodo statico che
accetti un carattere arbitrario e un carattere di sostituzione,
e restituisca il primo carattere trasformato opportunamente.

Per questo programma è bene effettuare le prove utilizzando la
redirezione: create un file `input.txt` contenente le righe
di prova, ed eseguite la vostra soluzione aggiungendo `< input.txt`
alla fine della riga di comando. In questo modo l'input invece
che da tastiera arriverà dal file `input.txt`, facendovi risparmiare
tempo e fatica.
