# Sheet n°1: Identify personal data

#### Understanding the notions of "personal data", "purpose" and "processing" is essential to ensure that software complies with the law when it processes user data. In particular, be careful not to confuse "anonymisation" and "pseudonymization", which have very precise and different definitions in the GDPR.

## Definition
* The notion of **personal data** is defined in the [General Data Protection Regulation](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) (GDPR) as "[any information relating to an identified or identifiable natural person (referred to as "data subject")](https://www.cnil.fr/en/personal-data-definition)". It covers a broad scope that includes both directly identifying data (e.g. first and last name) and indirectly identifying data (e.g. telephone number, license plate, terminal identifier, etc.).

* Any operation on this type of data (collection, recording, transmission, modification, dissemination, etc.) constitutes **processing within the meaning of the GDPR** and must therefore meet the requirements laid down by that regulation. Such processing operations must be lawful and have a specified purpose. The personal data collected and processed must be relevant and limited to what is strictly necessary to achieve the purpose.

## Examples of personal data

* Where they relate to natural persons, **the following data are personal data**:
    * Surname, first name, pseudonym, date of birth;
    * photos, sound recordings of voices;
    * fixed or mobile telephone number, postal address, email address;
    * IP address, computer connection identifier or cookie identifier;
    * Fingerprint, palm or venous network of the hand, retinal print;
    * License plate number, social security number, ID number;
    * Application usage data, comments, etc...

* **Identification of natural persons can be carried out**:
    * from a single piece of data (examples: surname and first name);
    * from crossing of a set of data (example: a woman living at such and such an address, born on such and such a day and member of such and such an association).

* Some data are considered **particularly sensitive**. The GDPR prohibits the collection or use of such data, unless, in particular, all involved data subjects have given their express consent (active, explicit and preferably written consent, which must be free, specific and informed).

* These requirements concern the following data:

    * data relating to the **health of individuals**;
    * data concerning **sexual life** or **sexual orientation**;
    * data revealing an alleged **racial** or **ethnic** origin;
    * political opinions, religious beliefs, philosophical beliefs or trade union membership;
    * **genetic** and **biometric data used for the purpose of uniquely identifying an individual**.

## Anonymisation of personal data

* An **anonymisation process of personal data** aims at making impossible to identify individuals within data sets. It is therefore an irreversible process. When this anonymisation is effective, the data are no longer considered as personal data and the requirements of the GDPR are no longer applicable.

* By default, we recommend that you **never consider raw datasets as anonymous**. Anonymisation results from processing personal data in order to irreversibly prevent  identification, whether by:

    * _singling out_: it is not possible to isolate some or all records which identify an individual in the dataset;
    * _linkability_: the dataset does not allow to link together two or more records concerning the same data subject or a group  of data subjects;
    * _inference_:  it is  not  possible  to  infer,  with  significant  probability, the value of an attribute from the values of a set of other attributes.

* These data processing operations imply in most cases a **loss of quality on the produced dataset**. The Article 29 Working Party (Art. 29 WP) [opinion on anonymisation techniques](https://ec.europa.eu/justice/article-29/documentation/opinion-recommendation/files/2014/wp216_en.pdf) describes the main anonymisation techniques used today, as well as examples of datasets wrongly considered anonymous. It is important to note that anonymisation techniques have short comings. The choice whether or not to anonymize the data as well as the choice of an anonymisation technique must be made on a case-by-case basis according to the different contexts of use (nature of the data, usefulness of the data, risks for people, etc.).


## Pseudonymization of personal data

* **Pseudonymization is a compromise between retaining raw data and producing anonymized datasets**.

* It refers to the processing of personal data in such a way that **data relating to a natural person can no longer be attributed without additional information**. The GDPR insists that this additional information must be kept separately and be subject to technical and organisational measures to avoid re-identification of data subjects. Unlike anonymisation, pseudonymization can be a reversible process.

* In practice, a pseudonymization process consists in **replacing directly identifying data (surname, first name, etc.) in a dataset with indirectly identifying data** (alias, number in a filing system, etc.) in order to reduce their sensitivity. They may result from a cryptographic hash of the data of individuals, such as their IP address, user ID, e-mail address.

* Data resulting from pseudonymization are considered as **personal data and therefore remain subject to the obligations of the GDPR**. However, the European Regulation encourages the use of pseudonymization in the processing of personal data. Moreover, the GDPR considers that pseudonymization makes it possible to reduce the risks for data subjects and to contribute to compliance with the Regulation.
