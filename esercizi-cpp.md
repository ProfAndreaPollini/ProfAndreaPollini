# Esercizi di programmazione

Raccolta di esercizi di programmazione che possono essere risolti sia utilizzando un qualsiasi linguaggio di programmazione.


## [1] Yellow Submarine

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

### Soluzioni

- ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=C%2B%2B&logoColor=white): [codice fatto in classe](https://replit.com/@professorandrea/3di-sottomarino-1?v=1)

## [2] Valutazione studenti

La facoltá Pincopallis ti ha affidato il compito di creare una applicazione per valutare gli studenti. In input verranno inseriti il voto (in decimi, anche non interi) e un intero che indica il numero di progetti realizzati dallo studente.

Il voto finale va calcolato in questo modo:

- voto maggiore o uguale a 9 e almeno cinque progetti realizzati -> voto finale = 10
- voto maggiore o uguale a 8 e almeno tre progetti realizzati -> voto finale = 8
- voto maggiore o uguale a 6 e almeno due progetti realizzati -> voto finale = 6
- ogni altro caso: voto finale = 4
 
Il voto finale verrá stampato a video.

## [3] Congettura di Collatz

La [Congettura di Collatz](https://it.wikipedia.org/wiki/Congettura_di_Collatz) é una congettura matematica tuttora irrisolta ma parecchio interessante.

La congettura riguarda il seguente algoritmo:

- Si prenda un intero positivo n.
- Se n = 1, l'algoritmo termina.
- Se n è pari, si divida per due; altrimenti si moltiplichi per 3 e si aggiunga 1.

Scrivere un programma che implementi l'algoritmo della congettura di collatz in una funzione `collatz(...)` e che, chiesto in input un numero intero di partenza, applichi la funzione fino al termine dell'algoritmo. Stampare a video la sequenza di numeri che l'algoritmo produce e quanti sono i passi che portano al termine dello stesso.

## [4] DISHWASH / postazione automatica di lavaggio piatti

ci è  stato chiesto di Simulare una postazione  automatica di lavaggio piatti. ogni piatto è  rappresentato da un  numero positivo che indica quanti cicli di lavaggio sono necessari per pulirlo. la capienza massima della macchina è  di dieci piatti. 

all'avvio la macchina è  vuota. utilizzare un array per gestire la lista di piatti. ad ogni ciclo la macchina mostra all'operatore le statistiche di funzionamento: quanti piatti ha lavato, quanti ne ha in attesa e se vi è ancora spazio per caricarne uno. nel caso chiede all'utente se vuole aggiungere uno. se l'utente dice di sì viene generato e aggiunto all'array un intero compreso tra 1 e 5 che indica il grado di sporcizia sul piatto. se l'utente decide di spegnere la macchina, questa stampi a video quanti piatti ha lavato.

## [5] DISHWASH 2/ postazione automatica di lavaggio piatti

data la dishwash dell'esercizio precedente consentire di selezionare il programma di funzionamento tra normale (ogni ciclo pulisce di 2 il piatto corrente) e ultra (ogni ciclo pulisce 4). tuttavia se il piatto corrente ha grando di luridume 2 e lo puoiamo con il programma ultra, perderemo due unita di detergente. il detergente che dovesse avanzare non può  essere utilizzato per un ulteriore piatto. allo spegnimento mostrare a video quante unità di detergente sono state sprecate.

## [6] DISHWASH 3 / postazione automatica di lavaggio piatti

estendere la dishwash in modo tale che possa riutilizzare le unità di detergente che avanzano durante la pulizia di un piatto per il successivo.

## [7] scambio valori con il passaggio per riferimento

scrivere una funziona `scambio` che consenta di scambiare i valori passati come parametro. se la funzione viene chiamata sulle variabili a e b che valgono rispettivamente 2 e 3, dopo la chiamata `scambia(a,b)` sia avrà che `a` varrà  3 e `b` varrà 2.

## [8] Buffer circolare

84un buffer circolare è  una struttura dati semplice rappresentative con un array di lunghezza fissata. all'inizio l'array è  vuoto e man mano che viene aggiunto un valore, 

l'aggiunta viene fatta nella prima posizione libera (salvare la prima posizione libera in una variabile). una volta inserito un elemento nell'ultima posizione dell'array  la successiva posizione libera sarà la prima (0), e al prossimo inserimento verrà quindi sovrascritto l'elemento  in posizione 0, poi 1 e così via.

la struttura  deve stampare gli elementi in essa contenuti dal più vecchio al più recente e anche dal 0iu recente al più vecchio

## [9] percorsi a L

Generare una matrice NxN con N=6. Riempirla di numeri casuali da 0 a 9. Ogni numero definisce
L'altezza di una zona di terreno che la matrice rappresenta. Fare inserire all'utente riga e colonna di partenza e di arrivo.

Definito come percorso a L un percorso che svolta una sola volta, stampare a video i numeri dei due percorsi ad L che rappresentano i cammini tra partenza e arrivo.
Stampare anche quale è il percorso con la somma delle altezze più breve e la somma totale delle quote dei due percorsi.

## [10] gestione di una lista dinamica

Implementare utilizzando un Array un set per interi i cui elementi sono sempre maggiori o uguali a  zero.
Il set  ha dimensione massima 5. Deve essere possibile inserire un elemento (se il set non è pieno), cercare se un elemento è presente, cancellare un elemento dandone il valore e 
Dire se il set è pieno oppure no. Nel caso di inserimento di un valore già presente, l'inserimento non viene effettuato e l'utente viene avvisato (nei set non vi sono mai elementi duplicati) 

## lunghezza di una stringa

Creare una funziona che, data una stringa C style come parametro, ne ritorni la lunghezza. 

## ricerca della prima occorrenza di un carattere in una stringa

scrivere una funzione che, assegnata una stringa come parametro, ritorni la posizione di un carattere nella stringa, ritornando -1 se il carattere non dovesse essere presente nella stringa.

## concatenare due stringhe

date due stringhe c style come parametro di una funzione e una terza stringa sempre C style, concatenare le due stringhe e ritornare il risultato nella terza stringa

## concatenare due stringhe /2

date due stringhe (std::string) come parametro di una funzione e una terza stringa ( sempre std::string), concatenare le due stringhe e ritornare il risultato nella terza stringa

## codifica pinco latin

definire una funzione `char[] pincoLatin(const char[])` che effettui la codifica pinco latin della stringa passata come parametro e la ritorna. La lunghezza massima della stringa passata come parametro è 20. La codifica pinco latin è definita come segue:

* una parola è una sequenza consecutiva di lettere (a-z, A-Z) o apostrofi. Puoi assumere che l'input della funzione `pincoLatin` è una singola parola.
* Se una parola inizia per vocale, viene lasciata come è e viene aggiunta alla sua finale la seguqenza di caratteri "pinco". Quindi "amico" diventerà "amicopinco"
* Se una parola inizia con una consonante, ogni suo carattere fino alla prima vocale esclusa verrà trasferito alla fine della parola e verrà aggiunto "co" alla fine della stringa risultante. Ad esempio "ciao" diventerà "iaocco".
* Se il primo carattere della stringa è maiuscolo, anche quello della stringa risultante dovrà esserlo. ad esempio "Ciao" -> "Iaocco"

## dungeon /1

Assegnato un dungeon come il seguente (per gestirlo utilizza un array bidimensionale come struttura dati): 

```
. . . . . . . . . .
. @ . . . . . . . .
. . . . . . T . . .
. . . . . . . . . .
. . . . T . . . . .
. . . . . . T . . .
. . . . . . . . . X
```

fai in modo che l'utente (il carattere `@`) possa muoversi nelle quattro direzioni, utilizzando i tasti `WASD`. Il gioco termina quando si raggiunge il carattere `X` oppure quando il giocatore muore dopo aver toccato una trappola `T`. Il giocatore non può uscire dalla mappa.

## dungeon/2

Definire in modo casuale la posizione delle trappole sulla mappa e far ripartire il gioco con una nuova disposizione di trappole ogni volta che si raggiunge la `X`.

## dungeon/3

Aggiungere un punteggio che incrementa ogni volta che si fa una mossa nella mappa e che continua ad incrementarsi ad ogni mappa completata, fino alla morte del personaggio, quando invece deve essere riazzerato.

## dungeon/4

Aggiungere un orco `O` che si muove in modo casuale sulla mappa. Aggiungere altre creature o pozioni a piacere. Pubblicare su steam ;)

## tic tac toe

creare un gioco del tris che mostri la tavola di gioco e che chieda ad aogni giocatore di fare la propria giocata, scrivendo chi ha eventualmente vinto.

## gioco reale di Ur

Implementare il gioco reale di Ur, utilizzando le informazioni presenti nella pagina di [wikipedia dedicata](https://it.wikipedia.org/wiki/Gioco_reale_di_Ur).

