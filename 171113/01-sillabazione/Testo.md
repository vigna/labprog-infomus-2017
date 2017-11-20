La strana sillabazione
======================

Descrizione
-----------

Il professor Precisini, dell'Accademia della crusca, sostenendo che le
regole di sillabazione della lingua italiana sono troppo complesse e piene
di eccezioni, propone un nuovo e originale metodo di sillabazione. Il
metodo consiste in questo: una sillaba è una sequenza massimale di
caratteri consecutivi che rispettano l’ordine alfabetico. Per esempio, la
parola ambire viene sillabata come am-bir-e: infatti la lettera a precede
la lettera m, e le lettere b, i e r rispettano anch'esse l'ordine.
Analogamente, la parola sotterfugio viene sillabata come s-ott-er-fu-gio.

Dovete scrivere un programma che legge righe scritte dall'utente e ne
stampa la versione sillabata.

Vincoli
-------

Potete assumere che il testo in input in input non contenga lettere
maiuscole. Il programma si deve fermare quando viene premuto Control-D per
chiudere il flusso di ingresso.

Esempio
-------

Avendo nel flusso di ingresso

    amore
    medicina
    scafroglia

il programma emette nel flusso di uscita

    amor-e
    m-e-di-cin-a
    s-c-afr-o-gl-i-a

Suggerimenti
------------

Potete leggere l'input in un ciclo `while` controllato dal valore restituito
dal metodo `s.hasNextLine()` tramite l'istruzione

    String l = s.nextLine();

dove `s` è una variabile di tipo `Scanner` opportunamente inizializzata.

Per questo programma è bene effettuare le prove utilizzando la
redirezione: create un file `input.txt` contenente le righe di prova, ed
eseguite la vostra soluzione aggiungendo `< input.txt` alla fine della
riga di comando. In questo modo l'input invece che da tastiera arriverà
dal file `input.txt`, facendovi risparmiare tempo e fatica.
