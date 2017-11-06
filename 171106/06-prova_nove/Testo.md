La prova del nove
=================

Descrizione
-----------

La prova del nove è un meccanismo per il controllo dei calcoli basato
sull'aritmetica modulare. Sfrutta il fatto che dovendo controllare se `x * y =
z`, possiamo controllare se `x * y mod 9 = z mod 9`, dove `mod` è il resto
della divisione intera (in Java, `%`). Calcolare il resto della divisione per
nove è molto facile perché basta continuare a sommare le cifre del numero
finché non si ottiene il risultato: per esempio,

   7813 mod 9 = (7 + 8 + 1 + 3) mod 9 = 19 mod 9 = (1 + 9) mod 9 = 10 mod 9 = (1 + 0) mod 9 = 1.

Scrivete un programma che enumeri le terne di interi x, y, z minori di un
intero dato dall'utente e che stampi quelle per cui la prova del nove non
funziona (cioè `x * y != z` ma `(x * y) % 9 == z % 9`).

Vincoli
-------

Il numero in ingresso è strettamente positivo.

Esempio
-------

Avendo nel flusso di ingresso

    5

il programma emette nel flusso di uscita

    3 3 0
    3 4 3
    4 3 3

Suggerimenti
------------

Potete leggere l'input tramite

    int n = s.nextInt();

dove `s` è una variabile di tipo `Scanner` opportunamente inizializzata.

Per scrivere il programma occorrono tre cicli annidati.
