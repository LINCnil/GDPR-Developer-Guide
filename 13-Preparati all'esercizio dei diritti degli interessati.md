# Scheda n°13: Preparati all’esercizio dei diritti degli interessati

#### Le persone di cui tratti i dati mantengono dei diritti su quei dati: diritto di accesso, di rettifica, di opposizione, di cancellazione, di portabilità dei dati e di limitazione del trattamento. Devi fornire loro gli strumenti per esercitare in modo effettivo i loro diritti, e allo stesso tempo includere nei tuoi sistemi informatici tutti gli strumenti informatici necessari perché quei diritti possano essere adeguatamente rispettati.

#### Definendo in anticipo le modalità con cui potranno contattarti, e i modi con cui risponderai alle loro richieste, sarai in grado di gestire in modo efficace il loro esercizio dei diritti.


## Misure minime da attivare

* All organisations that use personal data have **the obligation to indicate where and how** individuals can exercise their rights in relation to this data. For example, you can mention an e-mail address or a web form when informing individuals, as well as in your privacy policy.

* In order to facilitate the exercise of people's rights, these rights may also be **implemented**, in whole or in part, directly in **the application or software you develop**. This specific implementation is not mandatory, but it allows you to meet users' expectations and reduce the time and complexity of processing this type of request.

* Above all, in case of access or operations directly performed by a person who exercises his or her rights, do not forget to manage his **authentication** in a secure way. Overall, **trace** also all operations that have an impact on his or her personal data.

* Ogni organizzazione che usa dati personali ha **l’obbligo di indicare dove e come** le persone interessate possono esercitare i propri diritti relativamente a quei dati. Per esempio, puoi indicare un indirizzo email o un form web al momento in cui informi le persone del trattamento o nella tua privacy policy.
* Per facilitare l’esercizio dei diritti delle persone, questi diritti possono anche essere **implementati**, in tutto o in parte, direttamente **nell’applicazione o nel software che sviluppi**. Questo ti permette di venire incontro alle aspettative degli utenti e di ridurre il tempo e la complessità di trattare le loro richieste.
* Soprattutto, sia nell’accesso ai propri dati che nelle operazioni effettuate direttamente da una persona sui propri dati in tuo possesso, non dimenticare di gestire **l’autenticazione** in modo sicuro. Ad ogni modo, **tieni traccia** di tutte le operazioni che hanno un impatto sui suoi dati personali.

## Alcuni esempi di diritti e di una loro possibile implementazione

* **Diritto di accesso**: le persone hanno il diritto di ottenere una copia di tutte le informazioni su di loro di cui sei in possesso. Questo, fra l’altro, permette a una persona di sapere se dati che la riguardano sono oggetto di trattamento e di ottenerne una copia in un formato di uso comune. In particolare, la persona può controllare la correttezza delle informazioni.

  **_Possibile implementazione_**: Prevedi una funzionalità che consenta la visualizzazione di tutti i dati relativi a uno specifico interessato. Se la quantità di dati è eccessiva, offri all’interessato la possibilità di scaricare un archivio contenente tutti i suoi dati.

- **Diritto di cancellazione**: le persone hanno il diritto di chiedere la cancellazione di tutti i dati di cui disponi su di loro.

  **_Possibili implementazioni_**:

  1. Prevedi una funzionalità che cancelli tutti i dati di una persona.
  2. Prevedi anche una notifica automatica a tutti i responsabili esterni perché a loro volta cancellino i dati relativi a quella persona.
  3. Prevedi anche la possibilità di cancellare i dati anche dai backup, o fornisci una soluzione alternativa che, quando si ripristina un backup, non ripristini i dati cancellati.

* **Diritto di opposizione**: in alcuni casi le persone hanno il diritto a opporsi al trattamento dei loro dati per uno scopo specifico.  
**_Possibile implementazione_**: prevedi una funzionalità che permetta agli interessati di esprimere la propria opposizione al trattamento. Quando l’interessato esercita il proprio diritto di opposizione in questo modo, il Titolare del trattamento deve cancellare i dati già raccolti, e deve astenersi dal raccogliere altri dati relativi alla persona in questione.
* **Diritto alla portabilità dei dati**: le persone hanno il diritto a ricevere i propri dati in un formato leggibile da computer per il proprio uso personale o per il trasferimento a un’altra organizzazione  
  **_Possibile implementazione_**: Prevedi una funzionalità che consenta alle persone di scaricare i propri dati in un formato machine-readable standard (CSV, XML, JSON, etc.).
* **Diritto di rettifica**: le persone hanno il diritto a chiedere la modifica dei propri dati quando questi siano scorretti, al fine di evitare la disseminazione di informazioni erronee.  
**_Possibile implementazione_**: consenti la modifica diretta dei dati nell’account dell’utente.
* **Diritto alla limitazione del trattamento**: le persone hanno il diritto a chiedere la sospensione per un certo periodo di tempo del trattamento dei propri dati, ad esempio per valutare una loro disputa riguardo al trattamento dei loro dati o per dar loro il tempo di esercitare i propri diritti.
  **_Possibile implementazione_**: Permetti agli amministratori di sistema di mettere “in quarantena” i dati di una persona: da quel momento quei dati non possono più essere né letti né modificati.

## In conclusione

* Il [sito Data & Design](https://design.cnil.fr/en) sviluppato dal Digital Innovation Laboratory di CNIL sviluppa questi concetti e contiene [esempi di interfacce per l’esercizio dei diritti](https://design.cnil.fr/en/concepts/exercising-rights/).

* E poi, lascia andare la tua **inventiva**!(In caso di dubbi, puoi aconsultare la CNIL o il Garante nelle forme previste).
