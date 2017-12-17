Orario
======

Descrizione
-----------

Implementate una classe di nome `Orario` che rappresenta un orario,
specificato come ore e minuti. Internamente, la classe deve mantenere un
singolo attributo intero (privato) che rappresenta i minuti trascorsi
dalla mezzanotte. (In realtà, per la realizzazione degli ultimi due
metodi indicati sarà necessario aggiungere altri attributi, il cui
tipo e significato sono soggetti a vostra valutazione) La classe deve
avere i seguenti costruttori e metodi:

- `Orario(int h, int m)`: costruisce l'orario `h:m` (`h` deve essere compreso fra 0 e 23, e `m` deve essere compreso fra 0 e 59; decidete
come comportarvi se queste condizioni non si verificano);

- `Orario(int h)`: costruisce l'orario `h:00`;

- `Orario()`: costruisce l'orario corrispondente all'ora attuale; per ottenere tale orario, tenete conto che:
    - l'ora attuale si può ottenere con l'istruzione `(new GregorianCalendar()).get(Calendar.HOUR_OF_DAY)`;
    - i minuti attuali si possono ottenere con l'istruzione `(new GregorianCalendar()).get(Calendar.MINUTE)`;

- `int getOre()`: restituisce le ore;

- `int getMinuti()`: restituisce i minuti;

- `void setOre(int h)`: cambia le ore, lasciando i minuti invariati;

- `void setMinuti(int m)`: cambia i minuti, lasciando le ore invariate

- `void setOreMinuti(int h, int m)`: cambia sia le ore che i minuti;

- `boolean equals(Orario x)`: restituisce true se l'orario su cui è invocato è uguale a `x`;

- `int compareTo(Orario x)`: restituisce un valore negativo se l'orario su cui è invocato viene prima di `x`, 0 se i due
orari sono uguali, e un valore maggiore di zero se l'orario su cui è invocato viene dopo;

- `int quantoManca(Orario x)`: restituisce il numero di minuti dall'orario target all'orario `x` (sarà un valore negativo
se `x` viene prima dell'orario attuale);

- `String toString()`: restituisce una stringa della forma h:m;

- `void setSeparatore(char separatore)`: permette di scegliere con che separatore stampare l'orario (da ora in
avanti verrà usato come separatore il carattere indicato, anziché `:` nel metodo `toString()`)

- `void setFormato(boolean formato24)`: permette di scegliere se stampare l'orario (da ora in poi) nel formato
24 ore, oppure nel formato 12 ore: in questo caso, il metodo `toString()` dovrà restituire ore della forma
`h:m AM` oppure `h:m PM` (al posto dei `:` ovviamente dovrete usare il separatore specificato).

Sperimentate la classe, realizzando un programma di test. 

Infine, aggiungete un metodo `toLiteral()` che restituisce l'ora e i
minuti in formato letterale: per esempio, se l'ora è 2:25 deve restituire
la stringa `due e venticinque`. 

Suggerimenti
------------

Per implementare `toLiteral()` è importante strutturare bene il programma
utilizzando dei metodi statici di supporto. Un punto di partenza è creare
un metodo in grado di stampare la parte delle decine, cioè che su input
`2` scriva “venti”, su input `3` scriva “trenta” e così via (usate
l’istruzione `switch`), e un metodo in grado di stampare le unità. Sulla
base di questi metodi è poi possibile creare un metodo che stampi in
maniera testuale un numero tra 0 e 59. Attenti alle combinazioni
contenenti “uno” e “otto”.

