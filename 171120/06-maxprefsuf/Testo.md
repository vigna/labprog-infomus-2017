Massimo prefisso/suffisso comune
================================

Descrizione
-----------

Date due stringhe fornite sulla riga di comando, dovete stamparne il
massimo _prefisso_ e il massimo _suffisso_ comune.

Il _massimo prefisso comune_ di due stringhe
<var>s</var><sub>0</sub><var>s</var><sub>1</sub>···<var>s</var><sub><var>m</var>&minus;1</sub>
e
<var>t</var><sub>0</sub><var>t</var><sub>1</sub>···<var>t</var><sub><var>n</var>&minus;1</sub>
è la sequenza
<var>s</var><sub>0</sub><var>s</var><sub>1</sub>···<var>s</var><sub><var>j</var>&minus;1</sub>
di massima lunghezza (cioè di massimo <var>j</var>) tale che
<var>s</var><sub>0</sub> =  <var>t</var><sub>0</sub>,
<var>s</var><sub>1</sub> = <var>t</var><sub>1</sub>, … ,
<var>s</var><sub><var>j</var>&minus;1</sub> =
<var>t</var><sub><var>j</var>&minus;1</sub>. Analogamente viene definito il
_massimo suffisso comune_.

Esempio
-------

Avendo sulla riga di comando le stringhe

    mamma madre

il programma stampa

    ma
     

(la seconda riga è vuota), mentre avendo sulla riga di comando le stringhe

    pippo pappo

il programma stampa

    p
    ppo

Suggerimenti
------------

Assumendo che la vostra classe si chiami `PrefSuff`, per eseguire il programma
secondo le istruzioni dovete dare il comando

    java PrefSuf mamma madre

e leggere tramite l'argomento del metodo `main()` le due stringhe fornite.
