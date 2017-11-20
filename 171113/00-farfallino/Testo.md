Alfabeto farfallino
===================

Descrizione
-----------

Quando i vostri docenti di laboratorio di programmazione erano bambini,
usavano a volte, per comunicare con i loro simili, uno speciale alfabeto,
detto alfabeto farfallino. L'alfabeto farfallino consiste nel sostituire a
ciascuna vocale una sequenza di tre lettere della forma vocale-f-vocale.
Per esempio, alla lettera `a` viene sostituita la sequenza `afa`, alla
lettera `e` la sequenza `efe` e così via. Dovete scrivere un programma che
legge righe scritte dall'utente e ne stampa la traduzione in alfabeto
farfallino.

Vincoli
-------

Potete assumere che il testo in input non contenga lettere maiuscole.
Il programma si deve fermare quando viene premuto Control-D per chiudere il
flusso di ingresso.

Esempio
-------

Avendo nel flusso di ingresso

    mamma mia
    aiuola
    farfalla

il programma emette nel flusso di uscita

    mafammafa mifiafa
    afaifiufuofolafa
    fafarfafallafa

Suggerimenti
------------

Potete leggere l'input in un ciclo `while` controllato dal valore restituito
dal metodo `s.hasNextLine()` tramite l'istruzione

    String l = s.nextLine();

dove `s` è una variabile di tipo `Scanner` opportunamente inizializzata.

Utilizzate l’istruzione `switch` per scrivere un metodo statico che
accetti un carattere e restituisca una stringa che rappresenta la sua
trasformazione in farfallino. Chiamate poi il metodo all'interno di un
ciclo che scorre i caratteri della riga corrente.

Per questo programma è bene effettuare le prove utilizzando la
redirezione: create un file `input.txt` contenente le righe di prova, ed
eseguite la vostra soluzione aggiungendo `< input.txt` alla fine della
riga di comando. In questo modo l'input invece che da tastiera arriverà
dal file `input.txt`, facendovi risparmiare tempo e fatica.
