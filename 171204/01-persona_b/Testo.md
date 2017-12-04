Persona (2)
===========

Descrizione
-----------

Questo esercizio è un'estensione dell'esercizio “Persona”. Il formato di input è lo stesso.

Aggiungete alla classe `Persona` i seguenti metodi:

- un metodo che restituisca l'età (in anni) della persona (usando come riferimento l'anno in corso, che dovete memorizzare come costante statica della classe `Persona`);

- un metodo che determini se una persona è più vecchia di una persona data;

- un metodo che determini se una persona è nata nella stessa città di una persona data (le città sono due stringhe, e vanno considerate uguali se le due stringhe coincidono).

Sperimentate i metodi inseriti, per esempio modificando il programma
precedente in modo da stampare accanto a ogni persona anche la sua età, e
indicando quali sono le persone che sono non più vecchie della prima
inserita, e quali sono quelle che sono nate nella sua stessa città.
 
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
George Bush (Tordonia 1945), 59 anni
Michael Stipe (Athens 1959), 45 anni
Persone non più vecchie di George Bush (Tordonia 1945): George Bush (Tordonia 1945), Michael Stipe (Athens 1959)
Persone che sono nate dove è nato George Bush (Tordonia 1945): George Bush (Tordonia 1945)
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
