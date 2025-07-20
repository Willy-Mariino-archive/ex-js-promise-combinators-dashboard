# Esercizi sui Promise Combinators in JavaScript - Modulo 1, JavaScript avanzato - lezione 5, Promise combinators

Questa repository contiene una serie di esercizi svolti relativi all'utilizzo dei Promise combinators in JavaScript vanilla, con particolare attenzione a: 
- Promise.all()
- Gestione asincrona di chiamate HTTP
- Aggregazione di dati da fonti multiple

Descrizione dell'esercizio

Dashboard asincrona con Promise.all()
L'obiettivo dell'esercizio è creare una funzione asincrona che recupera e aggrega dati da diverse API simulando una dashboard informativa per una città. Utilizzando Promise.all(), la funzione effettua in parallelo tre richieste HTTP per ottenere:

- Il nome completo della città e il paese da `/destinations?search=[query]`
- Il meteo attuale da `/weathers?search=[query]`
- Il nome dell’aeroporto principale da `/airports?search=[query]`

La funzione aggrega i dati ricevuti in un unico oggetto, estraendo il primo risultato da ciascun array restituito dalle API. I dati vengono poi stampati in console in un messaggio formattato.

Struttura della soluzione
- Definizione della funzione `getDashboardData(query)` che esegue le chiamate HTTP in parallelo e aggrega i dati.
- Test della funzione con la query "London".
- Gestione degli errori e stampa del risultato in console.

