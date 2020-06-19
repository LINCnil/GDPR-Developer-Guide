# Scheda n°8: Gestisci i profili utente

#### La gestione dei profili dello staff e degli utenti deve essere valutata a monte dello sviluppo. Si tratta di definire profili di accesso e autorizzazione differenti in modo che ciascuna persona possa accedere solo ai dati di cui ha effettiva necessità.

## Buone pratiche per la gestione degli utenti

* Il punto di partenza è l’**uso di identificativi unici e individuali**, tanto per gli utenti dell’applicazione che per il team di sviluppo.
* Assicurati di richiedere l’autenticazione prima di qualunque accesso a dati personali, in linea con le [raccomandazioni di CNIL](https://www.cnil.fr/en/passwords-minimum-security-recommendations-businesses-and-citizens).
* Per assicurarti che ogni persona (utente o staff) possa accedere solo **ai dati di cui ha effettiva necessità**, il tuo sistema deve fornire **politiche differenziare di gestione degli accessi ai dati** (lettura, scrittura, cancellazione, ecc.) a seconda delle persone e delle loro necessità. Un meccanismo generale di gestione dei profili utente ti permetterà di raggruppare diritti diversi a seconda del ruolo svolto da un gruppo di utenti all’interno dell’applicazione.
* La gestione dei profili utente si può accompagnare a **sistemi di log che consentano di tracciare le attività e individuare anomalie o eventi legati alla sicurezza**, come accessi fraudolenti o abuso di dati personali. Questi sistemi non devono essere usati per altro scopo che non sia garantire un utilizzo corretto dei sistemi informatici. Inoltre, i log non possono essere conservati più di quanto sia necessario. In generale, si considera adeguata una conservazione per sei mesi.
* Considera anche di pianificare audit del codice o *penetration testing* per il tuo ambiente di sviluppo per **garantire la robustezza del tuo sistema di gestione dei profili utente**.

## Semplifica la gestione dei profili di sicurezza

* Pianifica di **documentare o automatizzare gli spostamenti dello staff**. Per esempio, dovresti definire procedure che prescrivono cosa fare nel momento in cui una persona non è più autorizzata ad accedere a un locale o a una risorsa IT, o al termine del contratto.
* Gestire staff e utenti implica **una revisione periodica dei permessi** sulla base dell’evoluzione delle necessità e della mobilità organizzativa all’interno del progetto. L’uso di servizi di directory come ad esempio *Lightweight Directory Access Protocol*, ti aiuterà a tenere sotto controllo questi cambiamenti e ti permetterà di affinare le tue strategie di accesso, per esempio definendo ruoli sulla base dei profili di utilizzo delle risorse. Questo ti permetterà di rispettare al meglio il principio del minimo privilegio.
* L’uso di account “superutente” (come *root*, *Administrator*, ecc.) deve essere evitato per le operazioni quotidiane e di routine, perché costituiscono le fondamenta del tuo sistema e allo stesso tempo un bersaglio di elezione per un possibile attaccante esterno. In particolare per questi account ti raccomandiamo di adottare una politica di password forti (da 10 a 20 caratteri, oppure multi-fattore) e di limitare al massimo il numero di persone che la conoscono.
* **Favorisci l’utilizzo di un password manager all’interno del progetto** e, ogjni volta che sia possibile, la transizione all’autenticazione forte. Evita account generici condivisi fra più persone.
