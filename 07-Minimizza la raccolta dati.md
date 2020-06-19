# Scheda n°7: Minimizza la raccolta di dati

#### Devi raccogliere solo i dati personali rilevanti, adeguati e necessari per la finalità per la quale li raccogli, come definita al momento della raccolta.

## Prima della raccolta, pensa ai diversi tipi di dati che devi raccogliere e limita la raccolta a ciò che è strettamente necessario.

* Pensa ai diversi **tipi di dati** che dovrai raccogliere prima di implementare la tua applicazione e **documenta** questi ragionamenti.
* Se **per una certa categoria di persone non servono** alcuni dati, non raccoglierli.
* Tratta e archivia i dati in modo da **ridurre l’accuratezza** (analogamente a quanto avviene per la pseudonimizzazione). Per esempio, se l’applicazione necessita solo dell’anno di nascita, archivia soltanto l’anno di nascita invece dell’intera data di nascita.
* Se raccogli dati particolarmente sensibili, come dati riguardanti la salute o informazioni giudiziarie, assicurati di raccogliere solo il **minimo necessario**. A causa delle restrizioni legali, la soluzione più semplice è ancora una volta **non raccoglierli** se puoi farne a meno.
* Minimizza anche i dati raccolti nei **log di sistema** e non fargli registrare dati sensibili o critici (password, dati sanitari, ecc.)
* Alcune funzionalità potrebbero migliorare l’esperienza utente ma **non sono strettamente necessarie per il corretto funzionamento dell’applicazione** (ad es. la geolocalizzazione per migliorare una ricerca geografica). In questo caso, l’utente finale deve poter **scegliere se usare o meno queste funzionalità**. Se decide di usarle, i dati ulteriori che raccoglierai devono essere conservati solo per il tempo strettamente necessario e non devono mai essere usati per altri scopi. 
* Ricordati di associare un **periodo di conservazione** a ciascuna categoria di dati, sulla base dello scopo del trattamento e degli obblighi di legge relativi alla loro conservazione. Anche i logo di sistema devono avere un periodo di conservazione predefinito. Documenta i periodi di conservazione che hai definito, perché dovrai poterli motivare.

## Una volta che i dati sono stati raccolti, predisponi meccanismi di cancellazione automatica.

* Implementa un sistema automatico di **eliminazione** al termine della conservazione. Puoi anche predisporre revisioni manuali periodiche dei dati conservati.
* Per assicurare una cancellazione completa, cancella **fisicamente** tutti i dati non più necessari tramite strumenti specializzati, o distruggendo i media fisici.
* Se i dati sono ancora utili, puoi ridurne la sensibilità usando metodi di **pseduonimizzazione** o **anonimizzazione**. Nel caso della pseudonimizzazione, i dati rimangono soggetti alle norme sulla protezione dei dati personali (vedi [Scheda 1](#Scheda_n°1_:_Individua_i_dati_personali)).
* Tieni un log delle **procedure di cancellazione automatica**. Questi log possono essere usati come **prova di cancellazione** di un certo dato. 

