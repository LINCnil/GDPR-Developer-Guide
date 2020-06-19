# Scheda n°4: Gestisci il codice sorgente

#### Qualunque sia la dimensione del tuo progetto, ti raccomandiamo fortemente l’uso di uno strumento di gestione del codice sorgente, come ad esempio un *version control system*, per tenere traccia delle differenti versioni nel corso del tempo.

## Definisci un sistema efficiente di controllo delle versioni efficiente, pensando alla sua sicurezza.

* Un sistema di controllo delle versioni è un programma software che ti permette di archiviare **tutto il tuo codice sorgente e i file associati** mantenendo la **cronologia di tutte le modifiche** che sono state fatte. Un semplice server FTP non è un sistema di controllo delle versioni.
* Imposta il tuo ambiente correttamente usando le funzionalità offerte dal tuo sistema di controllo delle versioni. Ti raccomandiamo di utilizzare una **autenticazione forte** o un’**autenticazione con chiavi SSH** sin dall’inizio del tuo progetto.
* Oltre a questo, assegna dei *livelli di accesso* al progetto per i diversi utenti del tuo sistema di controllo delle versioni e per ciascun livello definisci i corrispondenti **permessi** (per esempio, un livello “guest” con diritti di limitati di lettura, un livello “developer” con diritti di scrittura, ecc.)
* Fai **backup** regolari del tuo sistema di gestione del codice sorgente: In particolare, ricordati di fare il backup del server principale dove vengono registrate tutte le modifiche.
* Definisci procedure di sviluppo per lavorare in efficienza anche se **più persone sviluppano in contrmporanea**. Per esempio, puoi  decidere **che non tutti lavorino sullo stesso ramo (*master branch*) ma che ciascuno lavori su un ramo distinto, che verrà poi inglobato nel ramo principale mano a mano che lo sviluppo procede. Questo tipo di strategie sono già ben documentate, per esempio in [Git Flow](https://nvie.com/posts/a-successful-git-branching-model/).** In aggiunta, alcuni sistemi di controllo delle versioni ti permettono di definire **branch protetti** che impediscono cambiamenti non autorizzati ai file di quei branch.


## Sii consapevole del contenuto del tuo codice sorgente.

* Adotta **strumenti di valutazione della qualità del codice** (quality metrics) che analizzano il codice al momento del *commit* per verificarne la buona qualità. Puoi anche aggiungere script per il controllo di queste metriche alla [configurazione del sistema di controllo delle versioni](https://git-scm.com/book/uz/v2/Customizing-Git-Git-Hooks), in modo che il *commit* sia annullato se il sorgente non è di una qualità sufficiente.
* Mantieni i file segreti e le password al difuori del repository del codice sorgente:
    * in **file separati, non soggetti a *commit***. Ricorda di usare i file speciali del tuo sistema di controllo delle versioni (come ad esempio _.gitignore_ PER _Git_) in modo che non ti succeda per errore di fare *commit* di file sensibili
    * riguardo alle **variabili d’ambiente** assicurati di controllare che non vengano accidentalmente registrate nei *log* o visualizzate quando un applicativo va in errore
    * usa [**specifici software di configuration management o di secret management**](https://www.digitalocean.com/community/tutorials/an-introduction-to-managing-secrets-safely-with-version-control-systems#using-configuration-management-systems-for-secret-management).  

- Infine, se devi includere dati di questo genere nel tuo repository, prendi in considerazione la possibilità di **cifrare/decifrare automaticamente** questi file tramite un *plugin* del sistema di controllo di versione (ad es. [_git-crypt_](https://github.com/AGWA/git-crypt)).

* Dopo un *commit* che contiene dati personali o altri dati critici, non dimenticare di fare un [*purge*](https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History) [completo](https://help.github.com/en/github/authenticating-to-github/removing-sensitive-data-from-a-repository#purging-a-file-from-your-repositorys-history) del repository del codice sorgente: anche dopo ulteriori modifiche, quei dati potrebbero essere ancora disponibili nella *history* del tuo repository.
* Fa’ attenzione prima di **pubblicare online il tuo codice sorgente**. Passa in rassegna **tutti i contenuti**, inclusa tutta la *history* delle modifiche.

## Esempi di strumenti

* A differenza di strumenti come [Subversion](https://subversion.apache.org/), che richiedono un server centrale per funzionare, i principali sistemi di controllo delle versioni (come ad esempio[Git](https://git-scm.com/) o [Mercurial](https://www.mercurial-scm.org/) for example) sono **decentralizzati**.

* La maggior parte di questi sistemi, inclusi gli strumenti relativi (bug management, wiki per la documentazione, ecc.), sono anche disponibili attraverso **un’interfaccia web** . Queste soluzioni possono essere accessbili via Internet ([GitHub](https://github.com/), [Bitbucket](https://bitbucket.org/), ecc.), o possono essere integrate nei tuoi server.
