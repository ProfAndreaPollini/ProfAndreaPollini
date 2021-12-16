# Esercizi di programmazione

Raccolta di esercizi di programmazione che possono essere risolti sia utilizzando un qualsiasi linguaggio di programmazione.


## Yellow Submarine

siamo in navigazione nel mar del caos. Vogliamo recuperare delle informazioni relative al fondale marino, e per far questo possiamo utilizzare il sonar sp01, installato nel nostro sommergibile. 

Il sonar misura la profondità di una "striscia" frontale rispetto alla nostra direzione e ci ritorna un array di 15 misurazioni di profondità, una per ogni metro.

realizzare un programma che consenta di effettuare le seguenti operazioni:

- effettuare una scansione con il sonar. (*)
- stampare se ci sono più tratti in discesa o in salita.
- stampare la profondità media
- stampare profondità minima e massima
- data una distanza, la pronfondità media dal sottomarino alla distanza selezionata
- fare un grafico approsimativo della profondità

(*) scansione:
  riempire l' array delle misurazioni con valori interi nell'intervallo (5-20)

Bonus:

- applicare una funzione di smooth ai dati letti.
- comandare il sottomarino utilizzando solo i tasti 'w' (per andare su di una cella) e 's' per andare giù di una cella, in modo tale da attraversare il campo misurato passando il più possibile vicino al fondale. il punteggio viene dato misurando per ogni mossa la profondità del sommergibile, ad ogni movimento in verticale corrisponde sempre un movimento a destra. Disegnare il sommergibile sulla mappa con il carattere '@'
  - roadmap:
    - [x] disegnare il sottomarino fermo
    - [ ] movimento in verticale
    - [ ] movimento sempre a destra
    - [ ] punteggio
    - [ ] gestione collisione con il fondale

## Soluzioni

- ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=C%2B%2B&logoColor=white): [codice fatto in classe](https://replit.com/@professorandrea/3di-sottomarino-1?v=1)


### Simulare la caduta di un granello di sabbia [TODO]

Data una griglia bidimensionale che rappresenta il terreno sopra l'aria


