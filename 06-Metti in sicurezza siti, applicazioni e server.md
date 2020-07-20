# Scheda n°6: Metti in sicurezza siti, applicazioni e server

#### Ogni sito, applicazione e server deve incorporare regole di base di sicurezza allo stato dell’arte, non solo per  le comunicazioni di rete, ma anche per l’autenticazione e la gestione dell’infrastruttura.

## Mettere in sicurezza le reti di comunicazione

* **Implementare TLS versione 1.2 or 1.3** (al posto di SSL) su tutti i siti web e per le trasmissioni dati elle tue applicazioni mobili, per esempio con [LetsEncrypt](https://letsencrypt.org/fr/), usando solo le versioni più recenti e controllando la correttezza dell’implementazione.
* **Rendi obbligatorio l’uso di TLS** per tutte le pagine del tuo sito e per tutte le applicazioni mobili.
* **Riduci le porte i comunicazione aperte** a quelle strettamente necessarie per il corretto funzionamento delle applicazioni installate. Se l’accesso a un server web è possibile solo attraverso il protocollo HTTPS, allora solo le port 80 e 443 del server devono essere accessibili, e tutte le altre porte possono essere bloccate dal firewall.
* **OWASP ha pubblicato delle schede-guida**, ad esempio per [implementare correttamente TLS](https://cheatsheetseries.owasp.org/cheatsheets/Transport_Layer_Protection_Cheat_Sheet.html) o per [mettere in sicurezza un webservice](https://cheatsheetseries.owasp.org/cheatsheets/Web_Service_Security_Cheat_Sheet.html).

## Mettere in sicurezza le autenticazioni

* **Segui le [raccomandazioni CNIL per le password](https://www.cnil.fr/fr/node/23803)**. In particolare, ricordati di mettere un limite al numero di tentativi di accesso.

* **Non archiviare mai le passowrd in chiaro**. Memorizza il loro hash usando una libreria consolidata, come [bcrypt](https://en.wikipedia.org/wiki/Bcrypt).

* **Se usi cookie per l’autenticazione**, ti raccomandiamo:
* di forzare l’uso di HTTPS tramite [HSTS](https://en.wikipedia.org/wiki/HTTP_Strict_Transport_Security);
    
* di usare il flag `secure`;
    
* usa il flag `HttpOnly`.
    
* **Testa le librerire di crittografia installate sui tuoi sistemi** e disabilita quelle obsolete (RC4, MD4, MD5 etc.). Incoraggia l’utilizzo di AES256. [Leggi le note di OWASP al riguardo](https://owasp.org/www-project-cheat-sheets/cheatsheets/Cryptographic_Storage_Cheat_Sheet.html).

* **Adotta una politica specifica per le password degli amministratori**. Come minimo, cambia le loro password ogni volta che un amministratore lascia il lavoro, e comunque sempre in caso di sospetta violazione della sicurezza.

* **Limita l’accesso ai tool e alle interfacce di amministrazione al solo staff qualificato per il loro uso.** Per le operazioni quotidiane, incoraggia l’utilizzo di account a privilegi ridotti.

* **L’accesso remoto alle interfacce di amministrazione deve essere soggetto a misure di sicurezza rinforzate.** Per esempio, per i server interni, può essere una buona soluzione dotarsi di una VPN con autenticazione forte dell’utente e della macchina che usa per connettersi.

## Mettere in sicurezza le infrastrutture

* **Fai backup regolari, cifrati e controllati regolarmente**. Questo è particolarmente utile nel caso di attacchi di tipo *ransomware* perché in quel caso la disponibilità di un backup di tutti i sistemi è la tua sola possibilità di ripristinare i sistemi.

* **Limita la dimensione dello stack software che impieghi** e per ciascun elemento dello stack:
* **Installa gli update critici** senza ritardo, programmando un controllo automatico settimanale;
    * **Automatizza il controllo delle vulnerabilità** abbonandoti per esempio ai [Data Feed di NVD](https://nvd.nist.gov/vuln/data-feeds).
    
* **Adotta strumenti di scoperta delle vulnerabilità** per i processi più critici, in modo da poter scoprire possibili violazioni di sicurezza. Puoi usare sistemi per la scoperta e la prevenzione di attacchi anche sui sistemi e sui server critici. Questi test devono essere condotti regolarmente e comunque prima della messa in produzione di ogni nuovo software.

* **Limita o proibisci l’accesso sia fisico che via software alle porte di diagnostica e di configurazione remota**. Per esempio, puoi avere l’elenco di tutte le porte aperte con lo strumento `netstat`.

* **Proteggi i database che esponi su Internet**, come minimo limitando il più possibile l’accesso e cambiando la password di default per l’account dell’amministratore.

* Per quanto riguarda la gestione di database, le buone pratiche includono:

    * per l’accesso al database **usare account nominativi ** e creare account specifici per ciascuna applicazione;
    * **revoca i privilegi di amministratore** degli account (utente o applicativo) per evitare modifiche alla struttura del database (tabelle, viste, processi, ecc.);
    * assicurati di proteggerti contro attacchi di tipo SQL injection o *script injection;
    * incoraggia la cifratura a riposo di dischi e database.
