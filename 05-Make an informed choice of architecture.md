# Sheet n°5: Make an informed choice of architecture

#### When designing the architecture of your application, you must identify personal data that will be collected and define a path and life cycle for each of them. The choice of supporting assets (local storage, server, cloud service) is a crucial step, which must be adapted to your needs, but also to your technical knowledge. The registry and conduction a privacy impact assesment can assist you in this choice.

## Examining life cycle of data and processes, from collection to erasure

* Represent and describe how the product generally works before starting your project, with a diagram of data flows and a detailed description of the processes carried out.

* When data is only **stored on the user's terminal** (local storage) or remains **confined on communication networks under the control of the user** (e.g. Wi-Fi or other local network), the main point of attention is data security. The duration for which data is stored and the actual deletion should be determined by the individuals.

* **When the data transits through online services**, the choice of hosting the data yourself or using a service provider must be made according to your security knowledge and the expected quality of service. Recognized cloud offerings may offer higher levels of security. However, they generate new risks that need to be mastered. [Recommendations for companies planning to use Cloud computing services](https://www.cnil.fr/sites/default/files/typo/document/Recommendations_for_companies_planning_to_use_Cloud_computing_services.pdf) can guide at this selection stage.


## In case of use of external hosting

* **Choose a service provider that ensures appropriate security and confidentiality measures and is sufficiently transparent**. 

* **Make sure you know the geographical location of the servers that will host your data**. You may be required to transfer data outside the European Union (EU) and the European Economic Area (EEA). While data can move freely within the EU/EEA, transfers outside the EU/EEA are possible, provided that sufficient and appropriate level of data protection is ensured. The CNIL provides an on-site map showing the [different levels of data protection in countries around the world](https://www.cnil.fr/en/data-protection-around-the-world).

* **If you need to host health data**, make sure that provider used is [certified](https://esante.gouv.fr/labels-certifications/hds/liste-des-herbergeurs-certifies) or [approved](https://esante.gouv.fr/labels-certifications/hds/liste-des-herbergeurs-agrees) for this activity.

* Other points to be aware of include:
    - the existence of an accessible security policy;
    - physical security and safety measures at the hosting site;
    - data encryption and other processes to ensure that the provider does not have access to the data entrusted to it;
    - the management of updates, the management of authorizations, the authentication of personnel and the security of application developments;
    - the easy reversibility/portability of data in a structured and commonly used format, on request and at any time.
