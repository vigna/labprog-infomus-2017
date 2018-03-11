Più e meno
==========

Descrizione
-----------

Una stringa piùmeno è formata da una serie di simboli
più o meno ciascuno seguito da un numero formato da una
sola cifra. Il numero rappresentato dalla stringa si trova
partendo dal valore zero ed effettuando le operazioni
descritte nella stringa. Per esempio, la stringa

     +2-1-1-1+4

rappresenta il numero 3 = 0 + 2 - 1 - 1 - 1 + 4. Dovete scrivere un programma che legge
dal flusso di input una serie di stringhe piùmeno, una per riga, e stampa 
per ciascuna stringa `+`, `0` o `-`
a seconda che il valore della stringa sia strettamente positivo,
nullo o negativo.

Vincoli
-------

Ogni riga del flusso di input è una stringa piùmeno.

Esempio
-------

Eseguendo

    soluzione

e avendo nel flusso di ingresso

    +0+0
    -1+3-4
    +2-5+9

il programma emette

    0
    -
    +
