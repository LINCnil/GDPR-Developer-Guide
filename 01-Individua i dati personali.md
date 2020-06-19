# Scheda n°1: Individua i dati personali

#### Comprendere i concetti di “dati personali”, “scopo” e “trattamento” è essenziale per sviluppare trattamenti rispondenti ai requisiti di legge. In particolare, stai attento a non confondere “anonimizzazione” e “pseudonimizzazione”, che sono definiti con molta precisione nel GDPR.

## Definizione
* Il concetto di **dati personali** è definito nel [Regolamento Generale per la Protezione dei Dati Personali](https://eur-lex.europa.eu/legal-content/IT/TXT/HTML/?uri=CELEX:32016R0679&from=IT) come *“qualsiasi informazione riguardante una persona fisica identificata o identificabile («interessato»)”*. La definizione copre un àmbito vasto che include tanto dati che identificano direttamente (ad es. nome e cognome) quanto dati che identificano indirettamente (ad es, numero di telefono, targa dell’auto, identificativo del terminale, ecc.).
* Qualsiasi operazione su dati di questo tipo (raccolta, registrazione, trasmissione, modifica, disseminazione, ecc.) costituisce **trattamento ai sensi dei GDPR** e deve quindi rispondere ai requisiti definiti dalla legge. Queste operazioni di trattamento devono essere lecite e avere una finalità specificata. I dati personali raccolti e trattati devono essere rilevanti e limitati a quelli strettamente necessari per raggiungere la finalità prefissata.

## Esempi di dati personali

* Quando si riferiscono a persone fisiche, **i seguenti dati sono dati personali**:
    * Cognome, nome, pseudonimo, data di nascita
    * foto e registrazioni della voce
    * numero di telefono fisso o mobile, indirizzo postale, indirizzo email
    * indirizzo IP, identificatore di connessione telematica o cookie identificativo
    * Impronta digitale, impronta del palmo o reticolo venoso della mano, impronta retinica
    * Targa automobilistica, codice fiscale, numero di matricola
    * Dati di utilizzo dell’applicazione, commenti, ecc.

* **L’identificazione di persone fisiche si può ottenere**:
    * da un singolo dato (esempi: cognome e nome)
    * dall’incrocio di insiemi di dati (esempio: una donna che vive a un dato indirizzo, nata in una certa data e membro di una data associazione).

* Alcuni dati sono considerati **particolarmente sensibili**. Il GDPR proibisce la raccolta o l’uso di questi dati a meno che, in particolare, l’interessato abbia dato il proprio consenso (consenso attivo, esplicito e preferibilmente per iscritto, che deve essere libereo, specifico e informato).

* I requisiti di cui al punto precedente riguardano i seguenti tipi di dati:

    * dati relativi alla **salute degli individui**
    * dati relativi alla **vita sessuale** o **all’orientamento sessuale**
    * dati che possono rivelare una (anche supposta) origine **razziale** o **etnica**
    * opinioni politiche, credo religiosi, convinzioni filosofiche o appartenenza a sindacati 
    * dati **genetici** e **biometrici usati allo scopo di identificare in modo univoco un individuo**.

## Anonimizzazione di dati personali

* Un **processo di anonimizzazione di dati personali** mira a rendere impossibile l’identificazione degli individui appartenenti al dataset. &Egrave; pertanto un processo irreversibile. Quando questa anonimizzazione riesce, i dati non sono più considerati dati personali e le prescrizioni del GDPR non si applicano più.

* Di default, ti raccomandiamo di **non considerare mai anonimi dei dataset non trattati.** L’anonimizzazione è il risultato del trattamento di dati personali al fine di prevenire in modo irreversibile l’identificazione, in qualunque modo la si tenti: 
* _individuazione_: non è possibile isolare uno o tutti i record del dataset che identificano un individuo
    * _collegabilità_: il dataset non consente di collegare due o più record che si riferiscono a uno stesso interessato o a uno stesso gruppo di interessati
    * _inferenza_: non è possibile dedurre, con probabilità significativa, il valore di un attributo a partire dai valori di un insieme di altri attributi.
    
* queste operazioni di trattamento implicano nella maggior parte dei casi una **perdità di qualità del dataset risultante**. L’[opinione sulle tecniche di anonimizzazione](https://ec.europa.eu/justice/article-29/documentation/opinion-recommendation/files/2014/wp216_en.pdf) dell Gruppo di Lavoro Articolo 29 (Art. 29 WP) descrive le principali tecniche di anonimizzazione attualmente in uso, nonché esempi di dataset erroneamente considerati anonimi. &Egrave; importante notare che le tecniche di anonimizzazione hanno delle controindicazioni. La scelta se anonimizzare o meno i dati, nonché la scelta della particolare tecnica di anonimizzazione deve essere fatta caso per caso, sulla base del particolare contesto, dell’uso e delle necessità (natura dei dati, utilità dei dati, rischi per le persone, ecc.) .


## Pseudonimizzazione di dati personali

* **La pseudonimizzazione è un compromesso fra mantenere i dati nella loro forma originale e produrre dataset anonimizzati**.

* Si riferisce al trattare i dati personali in modo che **dati che si riferiscono a una persona fisica non possano più essere attribuiti ad essa senza l'uso di informazioni aggiuntive**. Il GDPR insiste che tali informazioni aggiuntive debbano essere conservate separatamente e soggette a misure tecniche e organizzative volte a evitare la re-identificazione degli interessati. A differenza dell'anonimizzazione, la pseudonimizzazione può essere un processo reversibile.

* In pratica, un processo di pseudonimizzazione consiste nel **sostituire in un dataset i dati immediatamente identificanti (cognome, nome, ecc.) con dati indirettamente identificanti** (pseudonimo, numero di pratica, ecc.) allo scopo di ridurre la loro sensibilità. Questi dati indiretttamente identificanti potrebbero essere il risultato di un hash crittografico dei dati degli individui, come l'indirizzo IP, la user ID, l'indirizzo e-mail.

* I dati risultanti dalla pseudonimizzazione sono considerati come **dati personali e pertanto soggetti alle prescrizioni del GDPR**. Ad ogni modo, il Regolamento Europeo incoraggia l'uso della pseudonimizzazione nel trattamento di dati personali. Inoltre il GDPR ritiene che la pseudonimizzazione renda possibile ridure il rischio per gli interessati e contribuisca alla compliance con il Regolamento.
