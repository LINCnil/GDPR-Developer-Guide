# Scheda n°5: Fai scelte architetturali informate

#### Quando progetti l’architettura della tua applicazione, devi identificare i dati personali che verranno raccolti, e definire un percorso e un ciclo di vita per ciascuno di essi. La scelta degli asset di supporto (storage locale, server servizi in cloud) è un momento cruciale, che deve essere adeguato ai tuoi bisogni ma anche alla tua conoscenza tecnica. Il registro dei trattamenti e la conduzione di un Privacy Impact Assessment ti possono assistere in questa scelta.

## Esaminare il ciclo di vita di dati e processi, dalla raccolta alla cancellazione.

* Descrivi e rappresenta il modo in cui funziona il tuo prodotto prima di avviare il progetto, usando diagrammi di tipo *data flow* e fornendo una descrizione dettagliata dei processi.
* Quando i dati sono **registrati solo sul terminale dell’utente** (storage locale) o **rimangono confinati a reti sotto il controllo dell’utente** (ad es. Wi-Fi o altra rete locale), la sicurezza dei dati è il principale punto di attenzione. Il  periodo di conservazione dei dati e la loro cancellazione dovrebbero essere determinati dai singoli utenti.
* **quando i dati viaggiano attraverso servizi online**, devi scegliere se a  avvalerti di un servizio di hosting o usare un fornitore di servizi sulla base delle tue competenze di sicurezza e della qualità che ci si aspetta dal servizio. I fornitori cloud più noti possono offrire livelli di sicurezza più elevati, ma generano nuovi rischi che devono essere tenuti sotto controllo. Queste [Raccomandazioni per le aziende che desiderano avvalersi di servizi di cloud computing ](https://www.cnil.fr/sites/default/files/typo/document/Recommendations_for_companies_planning_to_use_Cloud_computing_services.pdf) possono guidarti durante questo stadio di scelta.


## Nel caso si usi un hosting esterno

* **Scegli un fornitore di servizi che ti assicuri misure adeguate di sicurezza e confidenzialità e sia sufficientemente trasparente**. 
* **Assicurati di conoscere la collocazione geografica dei server che accoglieranno i tuoi dati**. Ti potrebbe venire chiesto di trasferire i dati al di fuori dell’Unione Europea (UE) e della European Economic Area (EEA). Mentre i dati possono muoversi liberamente all’interno della UE/EEA, i trasferimenti al di fuori idi UE/EEA sono possibili solo se vengono assicurati livelli sufficienti e appropriati di protezione dei dati personali. Sul sito di CNIL puoi trovare una mappa che mostra [i diversi livelli di protezione dei dati nei diversi paesi del mondo](https://www.cnil.fr/en/data-protection-around-the-world).
* **Se devi immagazzinare dati relativi alla salute**, assicurati che il provider di cui ti servi sia [certificato](https://esante.gouv.fr/labels-certifications/hds/liste-des-herbergeurs-certifies) o [approvato](https://esante.gouv.fr/labels-certifications/hds/liste-des-herbergeurs-agrees) per questo genere di attività.
* Altri punti da tenere presente:
    - l’esistenza di una policy di sicurezza accessibile;
    - misure fisiche di protezione e sicurezza presso il sito di hosting;
    - cifratura dei dati e altri processi per assicurare che il provider non abbia accesso ai dati che gli vengono affidati;
    - gestione degli aggiornamenti, gestione delle autorizzazioni, autenticazione del personale e sicurezza degli sviluppi applicativi;
    - facilità della reversibilità/portabilità dei dati in un formato strutturato di uso comune, in qualsiasi momento e su richiesta.
