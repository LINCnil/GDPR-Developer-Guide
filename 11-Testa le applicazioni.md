# Scheda n°11: Testa le applicazioni

#### Testare i tuoi prodotti ti permette di controllare che funzionino correttamente, che l’esperienza utente sia buona e di trovare e prevenire difetti prima che il codice vada in produzione. I test riducono anche i rischi di violazioni dei dati personali.

## Automatizza i test

* I **test di sviluppo** (unit, funzionali, ecc.) verificheranno la corrispondenza fra le specifiche e il funzionamento del prodotto. I **test di sicurezza** (test con dati casuali anche detti *“fuzzying”*, scansione delle vulnerabilità, ecc.) verificheranno che il prodotto continui a funzionare in modo accettabile anche al di fuori dell’utilizzo normale, e che non presenti vulnerabilità che permetterebbero a terze parti di comprometterne la sicurezza. Entrambi i tipi di test sono importanti per il corretto funzionamento della tua applicazione.

* Appronta un **sistema di integrazione continua** per eseguire i test in automatico dopo ogni modifica al codice sorgente.

## Integra i test nella tua strategia di business

* Aggiungi l’implementazione dell’ambiente di test alla strategia di business. Le **metriche accettabili** devono essere definite congiuntamente da tutte le parti in causa prima dello sviluppo..

* Le metriche che puoi considerare sono per esempio:

    * Il **tasso di copertura dei test** e il loro tipo;
    * il **tasso di duplicazione** nel codice;
    * il **numeri di vulnerabilità** (come definite dagli strumenti) e il loro tipo, ecc.

## Fai attenzione ai dati di test!

* Non si dovrebbero usare dati "veri” di produzione nelle fasi di sviluppo e di test. Usare dati personali per fare dei test dal tuo database di produzione equivale a **distoglierlo dal suo scopo originario**.
* Se usi dati personali al di fuori della produzione, occorre ricordare che i **rischi di sicurezza aumentano**: accesso ai dati da parte di persone che non ne hanno necessità, molteplici posizioni di archiviazione, ecc.
* Per questo motivi devi costituire un **dataset fittizio** che assomigli ai dati che verranno effettivamente trattati dalla tua applicazione. Un dataset fittizio garantirà che la comunicazione di questi dati non abbia alcun impatto sulle persone.
* Se devi **importare configurazioni esistenti** dalla produzione nei tuoi test, considera l’**anonimizzazione dei dati** che siano presenti.

