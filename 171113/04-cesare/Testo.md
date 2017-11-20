Il cifrario di Cesare
=====================

Descrizione
-----------

Svetonio nella “Vita dei dodici Cesari” racconta che Giulio Cesare usava per
le sue corrispondenze riservate un codice di sostituzione molto semplice,
nel quale la lettera in chiaro veniva sostituita dalla lettera che la
segue di tre posti nell'alfabeto: la lettera `A` è sostituita dalla `D`,
la `B` dalla `E` e così via fino alle ultime lettere che sono cifrate con
le prime.

Più in generale si dice _codice di Cesare_ un codice nel quale la lettera
del messaggio chiaro viene spostata di un numero fisso `k` di posti, non
necessariamente tre.

Dovete scrivere un programma che chiede in input una stringa da cifrare e
il numero `k` (la chiave di cifratura), ed emette in output la stringa
cifrata; il programma deve cifrare solo le lettere dell'alfabeto,
mantenendo minuscole le minuscole, e maiuscole le maiuscole, mentre deve
lasciare inalterati gli altri simboli.

Vincoli
-------

Potete assumere che la stringa non contenga lettere accentate.

Esempio
-------

Avendo nel flusso di ingresso

    mamma li Turchi
    5

il programma emette nel flusso di uscita

    rfrrf qn Yzwhmn

mentre avendo nel flusso di ingresso

    rfrrf qn Yzwhmn
    21

il programma emette nel flusso di uscita

    mamma li Turchi

Suggerimenti
------------

Potete leggere l'input usando prima il metodo `nextLine()` di `Scanner`
per leggere la frase, e poi il metodo `nextInt()` per leggere la chiave.

Una volta letta la frase, può essere comodo convertirla in un array
di caratteri utilizzando il metodo `toCharArray()` della classe `String`.

Per “spostare” ciclicamente di `k` posti un carattere `c` potete usare l’espressione

    (char)( ( ( c - ’A’ ) + k ) % 26 + ’A’ )

nel caso c sia maiuscolo,

    (char)( ( ( c - ’a’ ) + k ) % 26 + ’a’ )

nel caso c sia minuscolo (perché?).

Per stabilire se un carattere è una lettera potete usare il metodo statico
`Character.isLetter(char)`, e per sapere se è maiuscola o minuscola
i metodi statici `Character.isUpperCase(char)` e `Character.isLowerCase(char)`.

Per provare se il programma funziona, cifrate un messaggio con una certa
chiave `k` e poi applicate al risultato una nuova cifratura con chiave 26
− `k`: il risultato dovrebbe essere la stringa originale.

Per questo programma è bene effettuare le prove utilizzando la
redirezione: create un file `input.txt` contenente le righe di prova, ed
eseguite la vostra soluzione aggiungendo `< input.txt` alla fine della
riga di comando. In questo modo l'input invece che da tastiera arriverà
dal file `input.txt`, facendovi risparmiare tempo e fatica.
