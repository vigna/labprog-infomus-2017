Primi gemelli
=============

Descrizione
-----------

Due primi `p` e `q` sono gemelli se `q` = `p` + 2. Scrivete un programma che
stampi i primi gemelli minori di un intero fornito dall'utente.

Vincoli
-------

Il numero in ingresso è strettamente positivo.

Esempio
-------

Avendo nel flusso di ingresso

    10

il programma emette nel flusso di uscita

    3 5
    5 7

mentre avendo nel flusso di ingresso

    100

il programma emette nel flusso di uscita

    3 5
    5 7
    11 13
    17 19
    29 31
    41 43
    59 61
    71 73

Suggerimenti
------------

Potete leggere l'input tramite

    int n = s.nextInt();

dove `s` è una variabile di tipo `Scanner` opportunamente inizializzata.

Notate che vi occorre sapere se un numero è primo _due volte_: scrivete prima
un metodo statico che prende un numero e restituisce vero o falso a seconda che
il suo argomento sia primo. Poi, chiamate il metodo due volte all'interno di un
ciclo. È anche possibile, con un po' di attenzione, fare in modo di chiamare il
metodo una sola volta all'interno del ciclo (come?).
