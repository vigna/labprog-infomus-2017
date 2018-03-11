Sequenza perfetta
=================

Descrizione
-----------

Data una sequenza di 27 di cifre intere comprese tra 1 e 9, essa è *quasi
perfetta* se ogni cifra tra 1 e 9 è ripetuta esattamente tre volte.
Una sequenza quasi perfetta in cui ogni cifra `i` è posizionata in modo che ci
siano esattamente `i` numeri tra le occorrenze successive di `i` è detta
*perfetta*.
Ad esempio, la sequenza

    1 5 1 9 1 2 5 2 2 6 4 9 6 4 7 9 6 7 4 7 3 8 3 8 3 8 5

è quasi perfetta. La sequenza

    1 9 1 2 1 8 2 4 6 2 7 9 4 5 8 6 3 4 7 5 3 9 6 8 3 5 7

è perfetta.

Dovete scrivere un programma che legge dal flusso di input 27 cifre intere
comprese tra 1 e 9 e stampa a video `perfetta` se la linea contiene una
sequenza perfetta, `quasi` se la linea contiene una sequenza quasi perfetta,
`no` altrimenti.

Vincoli
-------

La sequenza di cifre inserita dal flusso di input contiene solo cifre tra 1 e 9.
Non è necessario alcun controllo. Le cifre sono su una o più linee, separate da
spaziatura.

Esempio
-------

Eseguendo

    soluzione

e immettendo dal flusso di input la sequenza

    1 9 1 2 1 8 2 4 6 2 7 9 4 5 8 6 3 4 7 5 3 9 6 8 3 5 7

il programma emette
    
    perfetta
    
Alternativamente, se nel flusso di input fosse inserita la sequenza

    1 9 1 2 1 8 2 4 6 2 7 9 4 5 8 6 3 4 7 5 3 9 5 5 5 5 5

il programma emetterebbe

    no

Eseguendo

    soluzione

e immettendo dal flusso di input la sequenza

    1 1 1 2 2 2 3 3 3 4 4 4 5 5 5 6 6 6 7 7 7 8 8 8 9 9 9

il programma emette
    
    quasi
