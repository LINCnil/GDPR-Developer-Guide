# Sheet n°15: Take into account the legal basis in the technical implementation

#### Processing of personal data must be based on one of the "legal basis" mentioned in [Article 6 of the GDPR](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32016R0679&from=FR#d1e1888-1-1). The legal basis of a processing operation is in a way the justification of the existence of the processing operation. The choice of a legal basis has a direct impact on the conditions for implementing the processing operation and [the rights of individuals](#Fiche_n°13_:_Preparing_the_exercise_of_persons_rights). Thus, anticipating the legal basis of the processing operations prior to any development will help you integrating the necessary functions to ensure that these processing operations comply with the law and respect the individuals rights.

## Definition of the legal bases in the GDPR

* In the context of a development for a private organization (companies, associations, etc.), the legal basis often used are:
    * **The contract**: the processing is necessary for the performance or preparation of a contract between the data subject and the body carrying out the processing operation;
    * **The legitimate interest**: the organization has a "legitimate" interest in carrying out the processing and it is not likely to adversely affect the rights and freedoms of the data subjects;
    * **Consent**: the data subject has given his or her explicit consent to the processing.

* If you are a public authority or a body pursuing tasks in the public interest, other legal bases may also be used:
    * **The legal obligation**: the processing is imposed by regulatory texts.
    * **The public-interest mission**: the processing is necessary for the performance of a task carried out in the public interest.

* Finally, in very specific cases,  **protect of vital interests** may be used as a legal basis, for example when processing is necessary to monitor the spread of epidemics or in cases of humanitarian emergency.


## Choose the appropriate legal basis

* First of all, check on the CNIL website that **a text does not impose any particular constraints** (for example: [cookies and other trackers](https://www.cnil.fr/sites/default/files/atoms/files/draft_recommendation_cookies_and_other_trackers_en.pdf)).

* **Only one legal basis must be chosen** for a given purpose. Legal basis cannot be cumulated for the same purpose. The same data processing operation may pursue several purposes and a legal basis must then be defined for each of them.

* As mentioned above, if you are a **public authority**, the legal obligation and the public interest mission will be the most relevant in most cases.

* If your processing operation is part of a contractual relationship and its purpose is objectively and strictly necessary for the provision of the user's service (e.g. name, first name and address to create an account on an e-commerce site) then **contract should be appropriate**.

* If your processing is not part of a contractual relationship with the user, then **the legal basis of consent or legitimate interest** may be invoked. If your processing is potentially intrusive (profiling, collection of geolocation data, etc.) then **consent is likely to be the appropriate legal basis**.

* If your processing contains **sensitive data** (health data, data concerning life or sexual orientation, etc.), then you will need to identify, in addition to the legal basis, an exception provided for by [Article 9 of the GDPR](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32016R0679&from=FR#d1e2051-1-1).

## Rights exercises and modalities of information to be provided according to legal basis

* The following table summarizes the exercises of rights to be provided in accordance with legal basis:

| | Right of access | Right to rectification | Right to erasure | Right to restriction of processing| Right to data portability | Right to object |
|:---------------------:|:-------------:|:----------------------:|:--------------------:|:-----------------------------------:|:----------------------:|:---------------------------:|
| **Consent**      | ✔             | ✔                      | ✔                    | ✔                                   | ✔                      | **Withdraw of consent**|
| **Contract**           | ✔             | ✔                      | ✔                    | ✔                                   | ✔                      | ✘                           |
| **Legitimate interest**  | ✔             | ✔                      | ✔                    | ✔                                   | ✘                      | ✔                           |
| **Legal obligation** | ✔             | ✔                      | ✘                    | ✔                                   | ✘                      | ✘                           |
| **Public interest**    | ✔             | ✔                      | ✘                    | ✔                                   | ✘                      | ✔                           |
| **Protect of vital interests**   | ✔             | ✔                      | ✔                    | ✔                                   | ✘                      | ✘                           |

* The legal basis used must **always appear in the information transmitted to the person**.

* **Where your processing is based on legitimate interest**, you must also indicate the legitimate interests pursued (fight against fraud, system security, etc.).

* It is recommended to **document your choice of legal basis**.  As an example, these choices can be indicated in a processing map or associated with your technical documentation.


## The specific case of cookies and other trackers

* The European ePrivacy Directive requires the user's consent before any action is taken to store information - via cookies, identifiers or other tracers (software fingerprints, pixels) or to access information stored in the user's terminal equipment.

* However, an exception is made when cookies are for the sole purpose of carrying out electronic communication, or are strictly necessary to provide a service requested by the user.

* Furthermore, the use of a single tracer for multiple purposes does not exempt from obtaining consent for the purposes that require it. For example, if an authentication cookie is also used for advertising targeting purposes, consent must be obtained for the latter purpose, in the same way as for a non-logged site.
