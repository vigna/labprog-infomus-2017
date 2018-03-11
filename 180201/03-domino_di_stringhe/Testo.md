Domino di stringhe
==================

Descrizione
-----------

Dovete scrivere un programma che crea un domino tra stringhe.

Il programma legge una lista di stringhe, una per riga, scartando quelle
contenenti meno di tre caratteri. A questo punto scandisce la lista
delle stringhe rimanenti, e crea un domino in cui ogni stringa è
collegata alla successiva dal fatto che i suoi ultimi due caratteri
sono uguali ai primi due della successive.

L'algoritmo comincia inserendo nel domino la prima stringa (tra quelle lunghe
almeno tre caratteri). A questo punto cerca la prima stringa dopo la prima le
cui due iniziali sono uguali alle ultime due lettere della prima. Procede poi
cercando una stringa successiva con lo stesso criterio, e così via.
Durante la ricerca, se viene raggiunta la fine della lista si riparte
dall'inizio della lista. La ricerca termina quando non si riesce più a trovare
una stringa da agganciare.

Notate che ogni stringa che è stata inserita nella lista delle parole
agganciate non va più considerata.

Al termine il programma stampa le stringhe agganciate, una per riga. Ogni
stringa viene stampata con il primo carattere maiuscolo e gli altri minuscoli.

Ad esempio, se in input fosse fornita la seguente lista di stringhe:

    CASA
    tornate
    sasso
	reno
    Calamari
    NATANTE
    Io
    Teca
    No
    rinascere
    notare
    sospetto
    renna

Le stringhe `Io` e `No` sarebbero scartate perché contengono meno di tre caratteri.

La lista rimanente sarebbe quindi 

    CASA
    tornate
    sasso
    reno
    Calamari
    NATANTE
    Teca
    rinascere
    notare
    sospetto
    renna

E produrrebbe il seguente output:

    Casa
    Sasso
    Sospetto
    Tornate
    Teca
    Calamari
    Rinascere
    Renna
    Natante

Notate che alla stringa `Rinascere` viene attaccata la stringa `Renna` (non la
stringa `Reno`) poiché la ricerca della stringa da attaccare deve partire dalle
posizioni successive a `Rinascere`. 


Suggerimenti
------------

Notate che secondo le regole suddette:

- se la lista di stringhe fornita in input non contiene stringhe con più di due
  caratteri il programma non stampa nulla;
- se la lista di stringhe contiene solo una stringa o se nessuna stringa si
  aggancia alla prima, il programma stampa comunque la prima stringa.

Esempio
-------

Eseguendo

    soluzione

e inserendo dal flusso di input 

    amo
    piace
    tutto
    tris
    otto

il programma stampa

    Amo

Eseguendo

    soluzione

e inserendo dal flusso di input 

    io
    tu
    NO
    ma
    
il programma non stampa nulla

Eseguendo
    
    soluzione

e inserendo dal flusso di input
    
    abcd
    aaab
    cccd
    abcde
    cdeeef
    cdaa
    efffgcc
    
il programma stampa

    Abcd
    Cdeeef
    Efffgcc
    Cccd
    Cdaa
    Aaab
    Abcde
