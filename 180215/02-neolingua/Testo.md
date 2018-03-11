Neolingua
=========

Descrizione
-----------

In Cortonia, il governo ha deciso di cominciare a utilizzare una neolingua
più pratica dell'italiano. In particolare, sono state individuate tre sorgenti
di ridondanza:

- Le parole che finiscono per `mente` potrebbero finire per `men`: per esempio,
  invece di `improvvisamente` si potrebbe dire `improvvisamen`.

- Le parole che contengono la sequenza `ntr` potrebbero invece contenere la sequenza
  `n`: per esempio, invece di `intrallazzo` si potrebbe dire `inalazzo`

- Ogni volta che compare una doppia, la si potrebbe sostituire con una
  lettera singola: per esempio, invece di `attaccatutto` si potrebbe
  dire `atacatuto`

Dovete scrivere un programma in grado di tradurre in neolingua una serie di frasi letta dal
flusso di input.

Vincoli
-------

Ogni riga del flusso di input è una frase in italiano da tradurre. Le frasi sono interamente in minuscolo
e possono contenere spaziatura e segni di interpunzione.

Esempio
-------

Eseguendo

    soluzione

e avendo nel flusso di ingresso

    assolutamente ciao
    un'intrallazzo 
    pazzo certamente
    mentecatto

il programma emette

    asolutamen ciao
    un'inalazo
    pazo certamen
    mentecato
