# Scheda n°3: Sviluppa in un ambiente sicuro

#### La sicurezza dei server di produzione, sviluppo e continuous integration, non ché quella delle macchine degli sviluppatori deve essere una priorità, perché centralizzano l’accesso a vaste moli di dati.

## Valuta i tuoi rischi e adotta misure di sicurezza appropriate

* **Valuta i rischi** degli strumenti e dei processi che usi per lo sviluppo. Fai un inventario delle misure di sicurezza esistenti e definisci un piano d’azione per migliorare la tua copertura dai rischi. Incarica una persona come responsabile della sua implementazione.

* Considera i rischi per tutti gli strumenti che usi, includi gli strumenti SaaS (Software as a Service) e strumenti collaborativi in cloud (come [Slack](https://slack.com), [Trello](https://trello.com), [GitHub](https://github.com), ecc.).

## Metti in sicurezza server e workstation in modo omogeneo e riproducibile

* Una lista di raccomandazioni riguardo alla sicurezza di server, workstation e  reti interne sono disponibili nelle [schede dal n° 5 all’8](https://www.cnil.fr/sites/default/files/atoms/files/cnil_guide_securite_personnelle_gb_web.pdf) della Guida alla Sicurezza dei dati personali dello CNIL.

* **Redigi un documento che elenchi le misure di sicurezza e ne spieghi la configurazione**, per assicurare che le misure di sicurezza siano implementate uniformemente sia sui server che sulle workstation. Per ridurre il carico di lavoro, puoi usare **strumenti di configuration management** come [Ansible](https://github.com/ansible/ansible), [Puppet](https://github.com/puppetlabs/puppet) o[Chef](https://github.com/chef/chef).

* Aggiorna sempre server  e workstation, se possibile in modo automatico. Puoi definire una watchlist delle vulnerabilità più importanti, per esempio gli [NVD Data Feed](https://nvd.nist.gov/vuln/data-feeds) del NIST.

## Poni particolare attenzione alla gestione degli accessi e alla tracciabilità delle operazioni

* Ricordati di documentare la gestione delle tue **chiavi SSH** (uso di algoritmi di crittografia e lunghezze delle chiavi allo stato dell’arte, protezioni delle frasi con una password, rotazione delle chiavi). Per esempi di buone pratiche, vedi il [documento sull’uso siduro di (open)SSH](https://www.ssi.gouv.fr/uploads/2014/01/NT_OpenSSH_en.pdf).

* Incoraggia l’autenticazione forte nei servizi usati dal team di sviluppo.

* **Traccia** gli accessi alle macchine e, se possibile, implementa una **analisi automatica dei log**. Per poter raccogliere tracce affidabili, occorre evitare l’uso di account generici.
