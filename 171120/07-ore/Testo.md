Ore
===

Descrizione
-----------

Scrivete un programma che, data un’ora sotto forma di tre numeri
interi (ore, minuti, secondi) fornita sulla riga di comando, stampa la
rappresentazione testuale dell'ora indicata. Vanno stampate sempre tutte e
tre le componenti: le prime due vanno separate da una virgola, e la terza
da una “e”.

Esempio
-------

Avendo sulla riga di comando gli argomenti

    12 30 22

il programma stampa

    Ore dodici, trenta minuti e ventidue secondi

mentre avendo sulla riga di comando gli argomenti

    13 00 00

il programma stampa

    Ore tredici, zero minuti e zero secondi

Suggerimenti
------------

È importante strutturare bene il programma utilizzando dei metodi statici
di supporto. Un punto di partenza è creare un metodo in grado di stampare
la parte delle decine, cioè che su input `2` scriva “venti”, su input `3`
scriva “trenta” e così via (usate l’istruzione `switch`), e un metodo in
grado di stampare le unità. Sulla base di questi metodi è poi possibile
creare un metodo che stampi in maniera testuale un numero tra 0 e 59.
Attenti alle combinazioni contenenti “uno” e “otto”.

Assumendo che la vostra classe si chiami `Ore`, per eseguire il programma
secondo le istruzioni dovete dare il comando

    java Ore 12 30 22

e leggere tramite l'argomento del metodo `main()` le tre componenti
fornite.
