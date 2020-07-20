<p align="center"><img src="https://github.com/LINCnil/GDPR-Developer-Guide/raw/it/templates/BANNIERE-IT.jpg" width="100%" align="middle"></p>


# GDPR Guida per sviluppatori

#### Al fine di aiutare gli sviluppatori di applicativi e di siti web a rendere il loro lavoro rispondente ai requisiti del GDPR, la CNIL ha redatto una nuova guida alle buone pratiche sotto licenza aperta, in modo che possa essere arricchita da altri professionisti.

Questa guida è pubblicata con [licenza GPLv3](https://www.gnu.org/licenses/gpl-3.0.html) e [open license 2.0](https://www.etalab.gouv.fr/wp-content/uploads/2017/04/ETALAB-Licence-Ouverte-v2.0.pdf) (esplicitamente compatibile con [CC-BY 4.0 FR](https://creativecommons.org/licenses/by/4.0/deed.fr)). Potete contribuire liberamente alla sua reedazione.

Questa versione italiana è stata gentilmente fornita da collaboratori esterni e rivista dal Garante per la Protezione dei Dati Personali. La [versione francese](https://github.com/LINCnil/Guide-RGPD-du-developpeur) è la versione autentica di questa guida.

La guida contiene indicazioni e buone pratiche, e pertanto fornisce a ogni stakeholder delle chiavi utili per comprendere il GDPR, quale che sia la dimensione della sua organizzazione. La guida può anche stimolare la discussione e lo sviluppo di pratiche all’interno delle organizzazioni e nelle relazioni con i clienti.

## Che cosa contiene la guida?

Questa guida è divisa in **16 schede tematiche** che coprono la maggior parte delle necessità degli sviluppatori in ciascuno stadio di progetto, dalla preparazione dello sviluppo all’uso di analytics.

Il Regolamento Generale per la Protezione dei Dati Personali (GDPR) specifica che la protezione dei diritti e delle libertà delle persone fisiche richiede **“l'adozione   di misure tecniche e organizzative adeguate per garantire il rispetto delle disposizioni del presente regolamento”** (Considerando 78).

La determinazione di tali misure è necessariamente **collegate al contesto delle operazioni di trattamento poste in essere**, e il Titolare del trattamento (l’entità pubblica o privata che tratta i dati personali) deve pertanto assicurare la protezione dei dati che è chiamato a trattare.

Le buone pratiche di questa guida, pertanto, **non intendono coprire tutte le richieste del Regolamento né intendono essere prescrittive**, ma forniscono un primo livello di misure per affrontare i problemi di sicurezza dei dati negli sviluppi IT che riguardano il trattamento di dati personali. A seconda della natura dei trattamenti, in alcuni casi potrà essere necessario implementare misure aggiuntive al fine di rispondere pienamente ai requisiti di legge. 

## Sommario

0. [Sviluppa in linea con il GDPR](#Scheda_n°0_:_Sviluppa_in_linea_con_il_GDPR)

1. [Individua i dati personali](#Scheda_n°1_:_Individua_i_dati_personali)

2. [Prepara lo sviluppo](#Scheda_n°2_:_Prepara_lo_sviluppo)

3. [Sviluppa in un ambiente sicuro](#Scheda_n°3_:_Sviluppa_in_un_ambiente_sicuro)

4. [Gestisci il codice sorgente](#Scheda_n°4_:_Gestisci_il_codice_sorgente)

5. [Fai scelte architetturali informate](#Scheda_n°5_:_Fai_scelte_architetturali_informate)

6. [Metti in sicurezza siti, applicazioni e server](#Scheda_n°6_:_Metti_in_sicurezza_siti,_applicazioni_e_server)

7. [Minimizza la raccolta dati](#Scheda_n°7_:_Minimizza_la_raccolta_dati)

8. [Gestisci i profili utente](#Scheda_n°8_:_Gestisci_i_profili_utente)

9. [Controlla librerie e SDK](#Scheda_n°09_:_Controlla_librerie_e_SDK)

10. [Garantisci la qualità del codice e della documentazione](#Scheda_n°10_:_Garantisci_la_qualità_del_codice_e_della_documentazione)

11. [Testa le tue applicazioni](#Scheda_n°11_:_Testa_le_tue_applicazioni)

12. [Informa gli utenti](#Scheda_n°12_:_Informa_gli_utenti)

13. [Preparati all'esercizio dei diritti degli interessati](#Scheda_n°13_:_Preparati_all'esercizio_dei_diritti_degli_interessati)

14. [Definisci un periodo di conservazione dei dati](#Scheda_n°14_:_Definisci_un_periodo_conservazione_dei_dati)

15. [Considera la base giuridica durante l’implementazione tecnica](#Scheda_n°15_:_Considera_la_base_giuridica_durante_l'implementazione_tecnica)

16. [Usa le analytics nei tuoi siti e applicazioni](#Scheda_n°16:_Usa_le_analytics_nei_tuoi_siti_e_applicazioni)



## Come posso contribuire a questa guida?

**Questa guida è disponibile in due versioni**:

* Una [versione web sul sito di CNIL](http://www.cnil.fr/en/rgpd-developers-guide) e [nel tab "Releases"](https://github.com/LINCnil/GDPR-Developer-Guide/releases) di questo repository;
* Questa [versione GitHub](https://github.com/LINCnil/GDPR-Developer-Guide), che offre a chiunque la possibilità di contribuire.

**Il contributo si articola in alcuni passi**:

* Registrati su GitHub;
* Vai alla pagina di progetto
* Puoi:
    * usare il tab "Issue" per aprire commenti o partecipare alla discussione
    * Usare l’opzione "Fork" per apportare le tue modifiche e proporre la loro inclusione tramite il bottone "Pull Requests".

**Le tue proposte di contributo verranno esaminate da CNIL prima della pubblicazione**. La versione web della Guida al GDPR per sviluppatori sarà aggiornata regolarmente.

## Uso

Per rilasciare tu stesso una copia di questo repository, puoi usare **Pandoc**. Questo strumento ti aiuta a convertire le schede in un unico documento docx, odt o HTML.

Puoi trovare le istruzioni su come installare Pandoc [qui]( https://pandoc.org/installing.html)

* **Per generare un file .docx**:

```bash
pandoc -s --toc --toc-depth=1 -o Guide_GDPR_sviluppatori.docx [0-9][0-9]*.md
```

* **Per generare un file .odt**:

```bash
pandoc -s --toc --toc-depth=1 -o Guide_GDPR_sviluppatori.odt [0-9][0-9]*.md
```

* **To generare un file .html file**:

```bash
pandoc -s --template="templates/mytemplate.html" -H templates/pandoc.css -o index.html README.md [0-9][0-9]*.md
```
