Istogrammi di frequenza
=======================

Descrizione
-----------

Scrivete un programma che legge una frase (cioè, un’intera riga) 
e visualizza degli istogrammi che illustrano il numero di occorrenze di ciascun
carattere alfabetico. Il programma non deve fare distinzione fra maiuscole e minuscole, e non deve visualizzare gli
istogrammi delle lettere che non compaiono.

Esempio
-------

Avendo nel flusso di ingresso

    C’era un RAGAZZO che come ME amava i Beatles e I rolling StoneS

il programma emette nel flusso di uscita

    A *******
    B *
    C ***
    E ********
    G **
    H *
    I ***
    L ***
    M ***
    N ***
    O ****
    R ***
    S ***
    T **
    U *
    V *
    Z **


Suggerimenti
------------

Nella codifica ASCII, i caratteri alfabetici sono consecutivi, cioè “A” è
seguito da “B”, eccetera. Per questo motivo, se `c` è un carattere
alfabetico maiuscolo, l'espressione `c - ’A’` restituisce un valore
compreso fra 0 (per la lettera “A”) e 25 (per la lettera “Z”). È quindi
facile utilizzare un array di 26 interi per contare le occorrenze dei
caratteri nella stringa.

Alla fine, dato un numero `i` tra 0 e 25, potete ottenere il carattere
maiuscolo corrispondente utilizzando l'espressione `(char)('A' + i)`.
