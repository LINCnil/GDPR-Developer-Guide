# Scheda n°10: Garantisci la qualità del codice e della documentazione

#### &Egrave; essenziale adottare il prima possibile buone tecniche di scrittura del codice. La leggibilità del codice riduce nel tempo gli sforzi di mantenimento e di correzione dei bug  per te e per i tuoi (magari futuri) collaboratori.

## Documenta il codice e l’architettura

* A volte durante lo sviluppo la documentazione viene trascurata, per mancanza di tempo o di visibilità del progetto. Però, è **cruciale per la manutenibilità del progetto**: ti permette di capire il modo in cui il codice funziona nel suo insieme, e di sapere quali parti di codice verranno affette da una modifica.

* **Documenta l’architettura, non solo il codice**: quando scrivi la documentazione devi essere in grado di tenere in mente la visione d’insieme e aiutare altri sviluppatori a capire come tutte le diverse componenti del codice lavorano insieme. Perciò, quando documenti il tuo progetto concentrati su diagrammi e spiegazioni chiare.

* **Aggiorna la documentazione assieme al codice**: il miglior modo per mantenere aggiornata la documentazione è di modificarla mano a mano che modifichi il codice.

* Se usi uno strumento di gestione del codice sorgente, in ciascun *commit* che modifica il sorgente puoi  includere anche le modifiche alla relativa documentazione (vedi in particolare la scheda ["Gestisci il codice sorgente”](#Scheda_n°4_:_Gestisci il codice sorgente)).

* **Nella documentazione, non scordare di trattare la parte relativa alla sicurezza**. In particolare, puoi documentare le differenti scelte di configurazione della tua applicazione, e spiegare quali regolazioni sono più sicure.

## Controlla la qualità del codice e della documentazione

* Un codice di qualità richiede **l’adozione di buone pratiche e convenzioni di scrittura**, applicate in modo consistente in tutta l’applicazione. &Egrave; anche opportuno fare riferimento a [convenzioni esistenti](https://github.com/Kristories/awesome-guidelines). Ecco alcuni esempi di buone pratiche:
    * **Usare nomi di variabile e di funzione espliciti** ende più semplice capire a colpo d’occhio cosa sta succedendo.
    * **Indentare correttamente il codice** ti permette di comprendere più velocemente la struttura del codice.
    * **Evitare la ridondanza del codice** riduce la necessità di replicare una modifica in più punti. Una svista si dimentica in fretta.

* **Esistono strumenti che possono aiutarti a controllare la qualità del codice**. Una volta che li hai configurati correttamente, ti eviteranno di rileggere il codice per assicurarti che le convenzioni di scrittura siano state rispettate. Alcuni esempi di questi strumenti sono:
* **Ambienti di sviluppo integrati ** ("_IDE–Integrated Development Environments_"), magari con l’aggiunta di plugin, che possono essere configurati per rispettare le regole di indentazione, le linee vuote fra diverse porzioni di codice o la posizione delle parentesi, graffe o di altro tipo.
    * **Software di misurazione della qualità del codice** possono segnalarti duplicazioni, adesione alle regole di programmazione e potenziali bug.
