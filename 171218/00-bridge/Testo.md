Bridge
======

Descrizione
-----------


Implementate una classe di nome `Carta` che rappresenta una carta da gioco. 
Internamente, la classe deve mantenere un attributo di tipo intero che contiene il seme (0=cuori, 1=quadri, 2=fiori, 3=picche)
e un attributo di tipo intero che contiene il valore (1=asso, 2=due, eccetera).
La classe deve avere i seguenti costruttori e metodi:

- `Carta(int seme, int valore)`: costruisce la carta corrispondente.
- `boolean equals(Object x)`: restituisce true se valore e seme sono uguali.
- `String toString()`: restituisce una stringa di due caratteri formata da valore e seme, dove il seme deve essere
una singola lettera maiuscola (conviene scrivere un metodo statico contenente uno switch che, dato l'indice di un seme, restituisce la stringa corretta)
e il valore deve essere numerico per tutte le carte ad eccezione
di asso, jack, queen e king, che vanno denotati con l'iniziale
maiuscola (conviene scrivere un metodo statico contenente uno
switch che, dato l'indice di un valore, restituisce la lettera
corretta).
- __Extra__: se ci riuscite, utilizzate i caratteri Unicode estesi ♥, ♦, ♣ e ♠ invece delle iniziali.

Sperimentate la classe, realizzando un programma di test che permette di
inserire carte immettendo seme e valore. Per leggere seme e valore
utilizzate `Scanner.nextToken()` e `Scanner.nextInt()` in un ciclo che
termina quando `Scanner.hasNext()` restituisce false.

Implementate poi una classe di nome `Giocatore` che rappresenta un
giocatore. Internamente, la classe deve mantenere un attributo di tipo
stringa che contiene il nome del giocatore, e una lista di carte che
rappresenta le carte correntemente in mano al giocatore.

La classe deve avere i seguenti costruttori e metodi:

- `Giocatore(String nome)`: costruisce un giocatore con nome dato.
- `void prendi(Carta carta)`: aggiunge la carta argomento a quelle in mano al giocatore.
- `String toString()`: restituisce stringa contenente il nome del giocatore seguito dalle carte in suo possesso, stampate separandole con uno spazio.
- __Extra__: se ci riuscite,
stampate le carte dell'ordine standard per seme (<em>come quando fuori piove</em>) e poi per valore.
- __Exxtra__: se ci riuscite, oltre a stampare le carte in ordine inserite due spazi tra due carte se hanno seme diverso.

Infine, implementate una classe di nome `Smazzata` contenente un metodo 
`main()` che genera una permutazione aleatoria di un mazzo completo, e distribuisce
le carte del mazzo a quattro giocatori inseriti dall'utente. La classe deve stampare i
quattro giocatori (in modo che si possa vedere la smazzata).

Per ottenere una permutazione aleatoria procedete come segue:

- Costruite utilizzando due cicli annidati un vettore `mazzo` di 52 carte contenente un mazzo ordinato.
- Permutate il vettore utilizzando un generatore di numeri pseudocasuali:

    Collections.shuffle( Arrays.asList( mazzo ), new Random() );

Il metodo statico `Collection.shuffle()` permuta in maniera aleatoria una lista,
dato un generatore di numeri pseudocasuali (`new Random()`). Il metodo
`Arrays.asList()` restituisce una classe lista involucro basata
sull'array argomento.

- A questo punto, create quattro giocatori utilizzando nomi letti da riga di comando (cioè dal vettore argomento del `main()`), e assegnate a ciascun
giocatore 13 carte come farebbe un mazziere: al primo giocatore le carte di indice 0, 4, 8, ecc.. Al secondo
giocatore le carte di indice 1, 5, 9, etc. E così via.

Per finire, stampate i giocatori, in modo da poter controllare che le loro smazzate siano corrette e stampate nell'ordine corretto.

Esempio
-------

Ecco un esempio di come potrebbe funzionare il programma (in grassetto le parti inserite dall'utente):

<pre>
<b>java Smazzata Marco Mario Marta Maria</b>
Marco 8♥ Q♥ A♥  6♦ J♦ K♦ A♦  2♣ 5♣ 8♣ K♣ A♣  9♠
Mario 2♥ 4♥ 5♥ 10♥ J♥ K♥  2♦ 8♦ 9♦  9♣  5♠ 6♠ A♠
Marta 3♥ 6♥  4♦ 10♦  3♣ 4♣ 6♣ 7♣ J♣  2♠ 7♠ 8♠ 10♠
Maria 7♥ 9♥  3♦ 5♦ 7♦ Q♦  10♣ Q♣  3♠ 4♠ J♠ Q♠ K♠
<b>java Smazzata Marco Mario Marta Maria</b>
Marco 3♥ 4♥ 7♥  5♦ 8♦ 10♦  7♣ 9♣ Q♣  2♠ 4♠ 8♠ A♠
Mario 9♥ A♥  2♦ 3♦ 6♦ 7♦  2♣ 3♣ 4♣ A♣  3♠ 6♠ K♠
Marta 2♥ Q♥  4♦ Q♦ A♦  6♣ 8♣ J♣ K♣  5♠ 7♠ 10♠ J♠
Maria 5♥ 6♥ 8♥ 10♥ J♥ K♥  9♦ J♦ K♦  5♣ 10♣  9♠ Q♠
<b>java Smazzata Marco Mario Marta Maria</b>
Marco 9♥ Q♥ K♥  7♦ 9♦ A♦  10♣  3♠ 4♠ 5♠ 6♠ 7♠ 10♠
Mario 6♥ J♥ A♥  3♦ 6♦ J♦ Q♦  3♣ 4♣ 8♣ J♣  Q♠ K♠
Marta 4♥ 7♥ 10♥  5♦ 8♦ K♦  5♣ 6♣ 9♣  2♠ 8♠ 9♠ J♠
Maria 2♥ 3♥ 5♥ 8♥  2♦ 4♦ 10♦  2♣ 7♣ Q♣ K♣ A♣  A♠
</pre>
