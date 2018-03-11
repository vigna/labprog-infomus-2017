Stampa numeri a zig-zag
=======================

Descrizione
-----------

Scrivete un programma che legge da linea di comando due numeri interi `r` e `c`
strettamente positivi e stampa una matrice di numeri con `r` righe e `c`
colonne.
Gli elementi della matrice sono i numeri da 1 a `r*c` disposti nel verso della
antidiagonale della matrice.
La scansione è effettuata alternativamente dall'alto verso il basso, e quindi
dal basso verso l'alto, come negli esempi sottostanti.

Vincoli
-------

Nella stampa del risultato gli elementi della matrice devono essere separati
dal carattere di tabulazione `\t`.

Esempio
-------

Eseguendo

    soluzione 3 7


il programma stampa 

    1       3       4       9       10      15      16
    2       5       8       11      14      17      20
    6       7       12      13      18      19      21


Eseguendo 

    soluzione 9 11
    
il programma stampa 
    
    1       3       4       10      11      21      22      36      37      54      55
    2       5       9       12      20      23      35      38      53      56      71
    6       8       13      19      24      34      39      52      57      70      72
    7       14      18      25      33      40      51      58      69      73      84
    15      17      26      32      41      50      59      68      74      83      85
    16      27      31      42      49      60      67      75      82      86      93
    28      30      43      48      61      66      76      81      87      92      94
    29      44      47      62      65      77      80      88      91      95      98
    45      46      63      64      78      79      89      90      96      97      99

Eseguendo 

    soluzione 11 7
    
il programma stampa

    1       3       4       10      11      21      22
    2       5       9       12      20      23      35
    6       8       13      19      24      34      36
    7       14      18      25      33      37      49
    15      17      26      32      38      48      50
    16      27      31      39      47      51      62
    28      30      40      46      52      61      63
    29      41      45      53      60      64      71
    42      44      54      59      65      70      72
    43      55      58      66      69      73      76
    56      57      67      68      74      75      77

Eseguendo 

    soluzione 4 1
    
il programma stampa

    1
    2
    3
    4
