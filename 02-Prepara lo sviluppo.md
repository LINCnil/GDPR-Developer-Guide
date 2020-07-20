# Scheda n°2: Prepara lo sviluppo

#### I principi della protezione dei dati personali devono essere integrati negli sviluppi IT dalla fase di design in poi, al fine di proteggere la privacy delle persone i cui dati verranno trattati, per dare loro un maggior controllo sui loro dati e per limitare errori, perdite, modifiche non autorizzate o abusi dei loro dati nelle applicazioni.

## Scelte metodologiche

* **Metti la protezione della privacy al centro dei tuoi sviluppi** adottando una metodologia di [Privacy By Design](https://edpb.europa.eu/our-work-tools/public-consultations-art-704/2019/guidelines-42019-article-25-data-protection-design_it).

* Considera di **integrare la sicurezza al centro dei processi**.  ANSSI rende disponibile una guida ["digital security & agility"](https://www.ssi.gouv.fr/uploads/2018/11/guide-securite-numerique-agile-anssi-pa-v1.pdf) (solo in Francese) che indica come portare avanti gli sviluppi nell’ambito di un framework agile tenendo in conto gli aspetti di sicurezza. Prendila come fonte di ispirazione.

* Per ogni sviluppo rivolto al grande pubblico, **considera i setting di sicurezza** e in particolare i valori di default come, per esempio, le caratteristiche e i contenuti utente visibili per default.

* **Conduci un [Privacy Impact Assessment (PIA)](https://www.cnil.fr/en/privacy-impact-assessment-pia)**. Per [alcune operazioni di trattamento](https://ico.org.uk/for-organisations/guide-to-data-protection/guide-to-the-general-data-protection-regulation-gdpr/accountability-and-governance/data-protection-impact-assessments/) è obbligatorio. In altri casi costituisce una buona pratica che ti permetterà di individuare e affrontare i rischi a valle del tuo sviluppo. La CNIL ha una sezione speciale del proprio sito e fornisce un [software libero](https://www.cnil.fr/en/open-source-pia-software-helps-carry-out-data-protection-impact-assesment) dedicato a questo tipo di analisi.


## Scelte tecnologiche

#### Architettura e caratteristiche

* **Includi la protezione della privacy, inclusi i requisiti per la sicurezza dei dati, nella fase di design dell’applicazione o del servizio.** Questi requisiti dovrebbero influenzare le [scelte architetturali](#Scheda_n°5:_Fare_una_scelta_informata_di_architettura) (ad es. decentralizzato vs. centralizzato) o le funzionalità (ad es. anonimizzazione, minimizzazione dei dati). Le regolazioni di default dell’applicazione devono almeno rispondere ai requisiti minimi di sicurezza e rispondere ai requisiti di legge. Per esempio, la complessità di default delle password deve rispondere come minimo alle [raccomandazioni CNIL sulle password](https://www.cnil.fr/fr/node/23803)
* **Mantieni il controllo del tuo sistema**. &Egrave; importante che tu mantenga il controllo del tuo sistema, sia per assicurarne il corretto funzionamento, sia per garantire un alto livello di sicurezza. Mantenere il tuo sistema semplice ti permette di comprendere con precisione come funziona e di individuarne i punti deboli. Se una certa complessità è necessaria, è consigliabile partire da un sistema semplice, sicuro e progettato correttamente. Su questa base è possibile aumentare la complessità passo a passo, mettendo via via in sicurezza le nuove funzionalità che vengono aggiunte.
* **Non contare su una sola linea di difesa**. Nonostante tutte le misure prese per progettare un sistema sicuro, può sempre accadere che alcune componenti aggiunte in un secondo tempo non siano sufficientemente sicure. Per minimizzare i rischi per gli utenti finali, è suggeribile che il sistema adotti una difesa in profondità. Per esempio, controllare i valori immessi in un modulo online è parte delle difese perimetrali. Se questa difesa viene scavalcata, la protezione delle query al database può risultare compromessa.

#### Strumenti e pratiche

* **Usa standard di programmazione che tengono in conto la sicurezza**. Spesso sono già disponibili liste di standard, buone pratiche o guide di programmazione per migliorare la sicurezza dei tuoi sviluppi. Puoi anche integrare tool aggiuntivi nel tuo ambiente integrato di sviluppo (“**IDE**”) in modo da controllare in automatico che il tuo codice corrisponda alle regole dettate dagli standard e dalle buone pratiche. Su Internet puoi facilmente reperire elenchi di buone pratiche per i tuoi linguaggi di programmazione preferiti. Per esempio [qui](https://wiki.sei.cmu.edu/confluence/display/seccode/SEI+CERT+Coding+Standards) per C, C++ o Java. Esistono anche buone pratiche specifiche per lo sviluppo di applicazioni Web, come quelle pubblicate da [OWASP](https://www.owasp.org).
* **Le scelte tecnologiche sono critiche**. Alcuni aspetti che devi tenere in conto:
    * A seconda del campo di applicazione o della funzionalità sviluppata, uno specifico linguaggio o tecnologia potrebbe essere più appropriato di un altro.
    * I linguaggi e le tecnologie più maturi sono più sicuri. In generale, sono stati soggetti a audit per correggere le vulerabilità più note. Ad ogni modo, devi fare attenzione a usare le ultime versioni di ciascun componente tecnologico che userai.
    * Devi evitare di scrivere la tua soluzione in un linguaggio che hai appena imparato e non domini ancora completamente. La tua mancanza di esperienza potrebbe esporti a maggiori rischi.
* **Appronta un ambiente di sviluppo sicuro che ti consenta la gestione delle versioni del codice** seguendo la [scheda dedicata](#Sheet_n°3:_Secure_your_development_environment) di questa guida.
