Persona
=======

Descrizione
-----------

Implementate una classe di nome `Persona` che rappresenta una persona. Una
persona è caratterizzata dai seguenti dati: un nome, un cognome, un anno
di nascita e un luogo di nascita. Implementate la classe decidendo quale
sia il costruttore, e decidendo di quali metodi dotarla. Dovete
necessariamente sovrascrivere il metodo `toString()` restituendo una stringa
opportuna (p.es. `Sebastiano Vigna (Milano 1967)`).

Realizzate quindi una
classe di test, in cui dichiarate un array e consentite a un utente di
inserire i dati di un certo numero di persone, creando ogni volta un
oggetto istanza di `Persona` e inserendolo nell'array. Alla fine, stampate
le persone inserite.

Esempio
-------

Ecco un esempio di come potrebbe funzionare il programma (in grassetto le parti inserite dall'utente):

<pre>
Quante persone? <b>2</b>
Nome: <b>George</b>
Cognome: <b>Bush</b>
Luogo di nascita: <b>Tordonia</b>
Anno di nascita: <b>1945</b>
Nome: <b>Michael</b>
Cognome: <b>Stipe</b>
Luogo di nascita: <b>Athens</b>
Anno di nascita: <b>1959</b>
George Bush (Tordonia 1945)
Michael Stipe (Athens 1959)
</pre>

Suggerimenti
------------

Se utilizzate `Scanner.nextInt()` per leggere un intero su una riga (come il primo input), 
dovete poi dare uno `Scanner.nextLine()` a vuoto per passare alla riga successiva. 

Per questo programma è bene effettuare le prove utilizzando la
redirezione: create un file `input.txt` contenente le righe di prova, ed
eseguite la vostra soluzione aggiungendo `< input.txt` alla fine della
riga di comando. In questo modo l'input invece che da tastiera arriverà
dal file `input.txt`, facendovi risparmiare tempo e fatica.
