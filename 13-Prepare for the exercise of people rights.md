# Sheet n°13: Prepare for the exercise of people rights

#### The persons whose data you process have rights on his or her data: right of access, to rectification, to object, to erasure, to data portability and to restriction of processing. You must give them the means to effectively exercise their rights and provide in your computer systems the technical tools that will allow their rights to be properly taken into account.

#### Preparing in advance how they will contact you and how you will deal with their requests will enable you to manage the exercise of these rights effectively.


## Minimum measures to be put in place

* All organisations that use personal data have **the obligation to indicate where and how** individuals can exercise their rights in relation to this data. For example, you can mention an e-mail address or a web form when informing individuals, as well as in your privacy policy.

* In order to facilitate the exercise of people's rights, these rights may also be **implemented**, in whole or in part, directly in **the application or software you develop**. This specific implementation is not mandatory, but it allows you to meet users' expectations and reduce the time and complexity of processing this type of request.

* Above all, in case of access or operations directly performed by a person who exercises his or her rights, do not forget to manage his **authentication** in a secure way. Overall, **trace** also all operations that have an impact on his or her personal data.

## Here are some examples of rights and their possible implementation

* **Right of access**: people have the right to obtain a copy of all the information you have about them. This allows, among other things, a person to know whether data concerning him or her is being processed and to obtain a readable copy in an understandable format. In particular, it allows the accuracy of the data to be checked.  
**_Possible implementation_**: Provide a functionality to display all data relating to a person. If there is a lot of data, you can split the data into several displays. If the data is too large, offer the person to download an archive containing all his or her data.

* **Right to erasure**: Persons have the right to request the deletion of all the data you hold on them.  
**_Possible implementations_**:
    1. Provide a functionality to erase all data relating to a person.
    2. Also provide for automatic notification of processors to also erase the data relating to that person.
    3. Provide for data erasure also in backups, or provide an alternative solution that does not restore erased data relating to that person.

* **Right to object**: individuals have the right to object in certain cases to their data being used for a specific purpose.  
**_Possible implementation_**: provide a functionality allowing the data subject to object to the processing. When the data subject exercises his or her right to object in this way, the controller must delete data already collected, and must not subsequently collect any more data related to that person.

* **Right to data portability**: Individuals have the right to retrieve their data in a machine-readable format for their own use or for transfer to another organisation.  
**_Possible implementation_**: Provide a feature that allows the data subject to download his or her data in a standard machine-readable format (CSV, XML, JSON, etc.).

* **Right to rectification**: Individuals have the right to request the modification of their data when it is incorrect in order to limit the use or dissemination of erroneous information.  
**_Possible implementation_**: Allow to directly modify data in the user account.

* **Right to restriction of processing**: individuals have the right to request that the processing of their data be blocked for a certain period of time, e.g. the time to examine a dispute on their part regarding the use of their data or a request to exercise rights.  
**_Possible implementation_**: Allow administrators to put data about a person in "quarantine": this data can then no longer be read or modified.

## In conclusion

* The [Data & Design site](https://design.cnil.fr/en) developed by the CNIL's Digital Innovation Laboratory develops these concepts and contains [examples of interfaces for exercising rights](https://design.cnil.fr/en/concepts/exercising-rights/).

* Finally, be **inventive**! (In case of doubt, ask the CNIL for advice).
