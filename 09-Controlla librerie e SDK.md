# Scheda n°09: Controlla librerie e SDK

#### Usi librerie, SDK o altri componenti software scritti da terze parti? Ecco alcuni suggerimenti su come integrarli mantenendo comunque il controllo del tuo sviluppo.

## Fai una scelta informata

* **Valuta il valore di ciascuna dipendenza che aggiungi.** Alcuni componenti software di uso comune sono lunghi solo poche righe. Però, ogni elemento aggiunto significa un aumento della superficie di attacco del tuo sistema. Se una singola libreria offre più funzionalità, integra solo le funzionalità di cui hai reale esigenza. Attivando il numero minimo di funzionalità riduci il numero di potenziali *bug* a cui sarai esposto. 

* **Scegli software, librerie e SDK che vengono mantenuti:**
* Se vuoi usare software libero o open source, scegli progetti o soluzioni con una comunità attiva di utenti, aggiornamenti regolari e buona documentazione.
  
* Se usi altri tipi di soluzioni con un supporto commerciale, assicurati contrattualmente che il codice sia mantenuto e aggiornato per la durata di vita del tuo progetto.
  
* **Tieni in considerazione la privacy.** Alcune librerie e alcuni SDK si ripagano usando i dati personali raccolti dalle applicazioni e dai siti in cui sono integrati. Assicurati che queste terze parti rispondano alle leggi applicabili sui dati personali, inclusa la corretta raccolta del consenso.

* **Se usi meccanismi crittografici, ti sconsigliamo fortemente di implementarti da solo gli algoritmi di cifratura**, piuttosto scegli librerie crittografiche che sono riconosciute, mantenute e semplici da usare.

## Valuta gli elementi individuati

* **Leggi  la documentazione e cambia le configurazioni di default**. &Egrave; importante sapere come funzionano le dipendenze del tuo codice. Le librerie di terze parti e gli SDK di solito hanno dei file di configurazione di default che spesso, per mancanza di tempo, non vengono nemmeno adattati, aprendo la via a molte falle di sicurezza. 
* **Fai un audit delle tue librerie e degli SDK.** Sai davvero tutto quello che fanno le librerie e gli SDK che integri nel tuo sviluppo? Quali dati vengono trasmessi attraverso queste dipendenze, e a chi? Un audit ti permetterà di determinare le prescrizioni di legge sulla protezione dei dati a cui devi attenerti e di stabilire le responsabilità di tutti gli attori coinvolti.
  **Fai una mappa delle dipendenze.** Le librerie di terze parti possono anche integrare altre componenti: fare un audit del loro codice ti permetterà di mappare meglio le tue dipendenze e di agire al meglio se una di loro mostra dei problemi. Per le componenti di terze parti, raccomandiamo anche che tu faccia degli audit di sicurezza e che li tenga poi monitorati.
* **Fai attenzione al [typosquatting](https://it.wikipedia.org/wiki/Typosquatting) e altre tecniche malevole.** Controlla i nomi delle dipendenze, e delle loro dipendenze, per evitare attacchi. Non fare copia-e-incolla di linee di comando da siti che non conosci.

## Mantieni aggiornate librerie e SDK

* **Usa sistemi di gestione delle dipendenze** (come yum, apt, maven, pip, ecc.) per mantenere una lista aggiornata delle tue dipendenze.
* **Gestisci gli aggiornamenti delle tue dipendenze**, specialmente nel caso di aggiornamenti di sicurezza che risolvono delle vulnerabilità. Devi predisporre una procedura documentata per gestirle e metterle in produzione nel minor tempo possibile.
* **Fai attenzione a versioni di librerie e SDK a fine vita o a fine contratto**  che non saranno più supportati: cerca di trovare un’altra soluzione (scegli una nuova libreria, rinnova il supporto commerciale).
* **Controlla lo status dei progetti open-source**, in particolare il cambio di dominio o di proprietà del pacchetto, alcuni attacchi usano aggiornamenti fasulli di dipendenze ampiamente in uso.
