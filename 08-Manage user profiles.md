# Sheet n°8: Manage user profiles

#### The way to manage profiles of your collaborators and your end-users must be thought out upstream of your developments. It consists in defining different access and authorization profiles so that each person can access only the data he or she actually needs.


## Good practices for user management 

* It all starts with the **use of unique and individual identifiers**, whether they are users of your application or collaborators in development.

* Make sure to **impose authentication** before any access to personal data, in accordance with the [recommendations of the CNIL](https://www.cnil.fr/en/passwords-minimum-security-recommendations-businesses-and-citizens).

* To ensure that each person (user or collaborator) can only access to **data he or she actually needs**, your system must provide **differentiated data access management policies** (read, write, delete, etc.) according to people and needs. A global user profile management mechanism will allow you to group different rights according to a role exercised by a group of users within the application.

* The management of user profiles can be used along with **logging systems in order to trace activities, and detect anomalies or events related to security**, such as fraudulent access and misuse of personal data. These devices must not be used for any purpose other than ensuring the proper use of the computer system. Logs must also not be kept longer than necessary. In general, a period of six months is adequate.

* You can also plan code audits or penetration testing within your development environment to **ensure robustness of your profile management system**.

## Streamline the management of clearance profiles

* Plan to **document or automate the movement of your collaborators**. For example, these procedures should lead the actions to be taken when people are no longer authorized to access a room or an IT resource, or at the end of their contract.

* Managing your users and collaborators implies **a regular review of the permission** according to the evolution of uses and organizational movements within your project. The use of directory services, such as _Lightweight Directory Access Protocol_ (_LDAP_), will help you monitor these changes and allow you to refine your access strategies, for example by assigning roles based on usage profiles. This allows you to better respect the principle of least privilege.


* The use of "supreme" accounts (type _root_, administrator, etc.) has to be avoided for conventional operations, as it constitutes the keystone of your system and a privileged target for a possible external attacker. We recommend that you associate a strong password policy with it (10 to 20 characters or multi-factor) and that you limit the number of people with knowledge of it to the strictest necessary.


* **Favour the use of a password manager within your project** and the transition to strong authentication when possible. Avoid generic accounts shared by several people.
