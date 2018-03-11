Ordine ciclico
==============

Descrizione
-----------

Una sequenza di <var>n</var> numeri si trova in *ordine <var>k</var>-ciclico* se quando esaminiamo 
gli elementi in posizione 0, <var>k</var> mod <var>n</var> , 2
<var>k</var> mod <var>n</var>, ..., (<var>n</var> – 1)<var>k</var> mod <var>n</var> 
questi sono in ordine crescente. Per esempio, la sequenza

    0 5 2 7 3 9 4

non è in ordine 1-ciclico, dato che 2 è più piccolo di 5, però è in ordine 2-ciclico,
perché 0 ≤ 2 ≤ 3 ≤ 4 ≤ 5 ≤ 7 ≤ 9.

Dovete scrivere un programma che legge una sequenza di interi e trova, se
esiste, il più piccolo <var>k</var> strettamente positivo per cui la
sequenza è ciclica e lo stampa. Se non esiste nessun <var>k</var> con
questa proprietà, dovete stampare 0.

Vincoli
-------

I numeri della sequenza compaiono nel flusso di ingresso, su una o più righe,
separati da spaziatura, e sono tutti distinti.

Esempio
-------

Eseguendo

	soluzione

e avendo nel flusso di ingresso

    0 5 2
    7 3
    9

il programma emette

	2

Avendo invece nel flusso di ingresso

    0 2 3 4 5 1

il programma emette

    0

e avendo nel flusso di ingresso

    0 3 2 1

il programma emette

    3

