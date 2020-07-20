# Scheda n°15: Considera la base giuridica durante l’implementazione tecnica

#### Il trattamento dei dati personali si deve basare su una delle “basi giuridiche” indicate nell’[Articolo 6 del GDPR](https://eur-lex.europa.eu/legal-content/IT/TXT/HTML/?uri=CELEX:32016R0679&from=IT#d1e1898-1-1). La base giuridica di un trattamento è in un certo senso la giustificazione dell’esistenza del trattamento. La scelta di una base giuridica ha una ricaduta diretta sulle condizioni per implementare le operazioni di trattamento e i [diritti degli interessati](#Scheda_n°13_:_Preparati_all'esercizio_dei_diritti_degli_interessati). Per questo, individuare le basi giuridiche del trattamento prima di avviare qualsiasi sviluppo ti aiuterà a includere le funzioni necessarie ad assicurare che tutte le operazioni di trattamento rispondano ai requisiti di legge e rispettino i diritti delle persone.

## Definizione delle basi giuridiche nel GDPR

* Nell’ambito di un’organizzazione privata, le basi giuridiche usate per sviluppare un trattamento di dati sono di solito:
    * **Contratto**: il trattamento è necessario per la preparazione o la realizzazione di un contratto fra l’interessato e l’entità che effettua le operazioni di trattamento;
    * **Legittimo interesse**: l’organizzazione ha un “legittimo” interesse a eseguire le operazioni di trattamento, purché non vengano meno i diritti e le libertà degli interessati.;
    * **Consenso**: L’interessato ha dato il suo esplicito consenso al trattamento dei propri dati.

* Un ente o una autorità pubblica che svolgono compiti di pubblico interesse possono usare anche altre basi giuridiche:
    * **Obbligo di legge**: il trattamento è richiesto da un testo normativo.
    * **Compito di pubblico interesse**: il trattamento è necessario per svolgere un compito nel pubblico interesse.

* Infine, in casi molto specifici, la base giuridica può essere la **tutela degli interessi vitali**, per esempio in casi di emergenza sanitaria.


## Scegli la base giuridica appropriata

* Per prima cosa, controlla sul sito di CNIL o del Garante che non ci siano **norme che impongono specifici vincoli** (per esempio: [cookie e altri tracciatori](https://www.cnil.fr/sites/default/files/atoms/files/draft_recommendation_cookies_and_other_trackers_en.pdf)).

* **Una sola base giuridica può essere scelta** per una data finalità. Non si possono cumulare più basi giuridiche per una stessa finalità. Le stesse operazioni possono rispondere a più di una finalità, e ciascuna di esse deve avere la propria base giuridica.

* Come detto sopra, nel caso di una **pubblica autorità**, l’obbligo di legge e il pubblico interesse saranno le basi giuridiche più rilevanti nella maggior parte dei casi.

* Se le operazioni di trattamento sono parte di una relazione contrattuale e il loro scopo è oggettivamente e strettamente necessario per la fornitura del servizio all’utente (ad es. nome, cognome e indirizzo per creare un account su un sito di commercio elettronico), allora la base giuridica più appropriata dovrebbe essere il **contratto**.

* Se il trattamento non  è parte di una relazione contrattuale con l’utente, allora puoi appellarti **alla base giuridica del consenso o del legittimo interesse**. Se il trattamento è potenzialmente intrusivo (ad esempio, raccolta di dati di geolocalizzazione, ecc.) allora **è probabile che la base giuridica appropriata sia il consenso**.

* Se il trattamento riguarda **dati sensibili** (dati riguardanti la salute, orientamento sessuale, politico, ecc.) allora, oltre alla base giuridica, devi identificare anche un’eccezione [nell’articolo 9 del GDPR](https://eur-lex.europa.eu/legal-content/IT/TXT/HTML/?uri=CELEX:32016R0679&from=IT#d1e2058-1-1) al divieto di trattamento.

## Esercizio dei diritti e informazione da fornire a seconda della base giuridica

* La tabella qui sotto riassume i diritti che possono essere esercitati per ciascuna base giuridica:

| | Diritto di accesso | Diritto di rettifica | Diritto di cancellazione | Diritto di limitazione | Diritto alla portabilità dei dati | Diritto di obiezione |
|:---------------------:|:-------------:|:----------------------:|:--------------------:|:-----------------------------------:|:----------------------:|:---------------------------:|
| **Consenso** | ✔             | ✔                      | ✔                    | ✔                                   | ✔                      | **Ritiro del consenso** |
| **Contratto**         | ✔             | ✔                      | ✔                    | ✔                                   | ✔                      | ✘                           |
| **Legittimo interesse** | ✔             | ✔                      | ✔                    | ✔                                   | ✘                      | ✔                           |
| **Obbligo di legge** | ✔             | ✔                      | ✘                    | ✔                                   | ✘                      | ✘                           |
| **Pubblico interesse** | ✔             | ✔                      | ✘                    | ✔                                   | ✘                      | ✔                           |
| **Tutela degli interessi vitali** | ✔             | ✔                      | ✔                    | ✔                                   | ✘                      | ✘                           |

* La base giuridica deve sempre comparire nell’informativa fornita alla persona interessata.

* **Se il trattamento si basa sul legittimo interesse**, devi anche indicare quale interesse intendi perseguire (contrasto alle frodi, sicurezza del sistema, ecc.).

* Ti raccomandiamo di **documentare la tua scelta di una base giuridica**. Per esempio, puoi riportare queste scelte in una mappa dei processi o includerle nella documentazione tecnica.


## Il caso specifico dei cookie e degli altri tracciatori

* La Direttiva Europea ePrivacy richiede il consenso dell’utente prima di qualsiasi azione che registri informazioni (tramite cookie, identificatori o altri tracciatori come fingerprint e pixel) o che acceda a informazioni registrate nel dispositivo dell’utente.

* Viene fatta un’eccezione quando i cookie hanno il solo scopo di consentire comunicazioni elettroniche, o sono strettamente necessari per fornire un servizio richiesto dall’utente.

* Inoltre, l’uso di un singolo tracciatore per una pluralità di scopi non ti esenta dall’ottenere il consenso per ciascuno degli scopi che lo richiedono. Per esempio, se un cookie di autenticazione viene usato anche per consentire pubblicità mirate, devi ottenere il consenso per questo secondo scopo, come faresti se l’utente non fosse autenticato.

  
