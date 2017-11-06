Lunghezza media delle parole
============================

Descrizione
-----------

Scrivete un programma che legga una frase (cioè, un’intera riga) e che calcoli
quante parole contiene e la loro lunghezza media. Per esempio, se consideriamo
la frase

    S’i’ fosse foco, arderei ’l mondo

la frase contiene 7 parole, con lunghezza media 3.43.

Esempio
-------

Avendo nel flusso di ingresso

    S’i’ fosse foco, arderei ’l mondo

il programma emette nel flusso di uscita

    La frase contiene 7 parole, con lunghezza media 3.43

mentre avendo nel flusso di ingresso

    mamma mia!

il programma emette nel flusso di uscita

    La frase contiene 2 parole, con lunghezza media 4.00

Suggerimenti
------------

Potete leggere l'input tramite

    String l = s.nextLine();

dove `s` è una variabile di tipo `Scanner` opportunamente inizializzata.

Per contare quante parole contiene una stringa potete controllare quanti sono i
caratteri alfabetici seguiti da caratteri non alfabetici; per vedere se un
carattere è alfabetico potete usare il metodo statico
`Character.isLetter(char)`.
Il metodo restituisce vero quando il suo argomento è alfabetico. Dovete
ovviamente stare attenti a quel che fate sull’ultimo carattere. Notate che la
lunghezza media è semplicemente il numero di caratteri alfabetici diviso per il
numero di parole.

Per stampare un numero double con un certo numero cifre decimali, anziché usare
`System.out.println()` potete usare `System.out.printf()`, che accetta una
stringa di formato. Per esempio,

    System.out.printf("La frase contiene %d parole, con lunghezza media %.2f\n", n, media);

assumendo che la variabile intera `n` contenga il numero di parole e che la
variable double `media` contenga la media.
