# Sheet n°3: Secure your development environment

#### The security of production, development and continuous integration servers as well as developer workstations must be a priority because they centralize access to a large amount of data.

## Assess your risks and adopt the appropriate security measures

* **Assess the risks** in the tools and processes used for your developments. Make an inventory of your existing security measures and define an action plan to improve your risk coverage. Appoint a person responsible for its implementation.

* Consider the risks on all the tools you use, including risks related to SaaS (Software as a Service) and collaborative tools in the cloud (such as [Slack](https://slack.com), [Trello](https://trello.com), [GitHub](https://github.com), etc.).

## Secure your servers and workstations in a homogeneous and reproducible way

* Lists of **recommendations** concerning the security of servers, workstations and internal networks are available in the [sheets n° 5 to 8](https://www.cnil.fr/sites/default/files/atoms/files/cnil_guide_securite_personnelle_gb_web.pdf) of the **security of personal data guide** of the CNIL.

* Write a **document listing those measures and explaining their configuration** to ensure that security measures are implemented uniformly on servers and workstations. In order to reduce the workload, **configuration management tools**, such as [Ansible](https://github.com/ansible/ansible), [Puppet](https://github.com/puppetlabs/puppet) or [Chef](https://github.com/chef/chef), can be used.

* Update servers and workstations, if possible automatically. You can set up a watchlist of the most important vulnerabilities, for example the [NVD Data Feeds](https://nvd.nist.gov/vuln/data-feeds).

## Put special emphasis on access management and traceability of operations

* Remember to document the management of your **SSH keys** (use of state of the art cryptography and key length algorithms, protection of private keys with a passphrase, key rotation). For examples of good practice, see [the document on the secure use of (open)SSH](https://www.ssi.gouv.fr/uploads/2014/01/NT_OpenSSH_en.pdf).

* Encourage strong authentication on the services used by the development team.

* **Trace** access to your machines and, if possible, implement **automated log analysis**. In order to keep reliable traces, the use of generic accounts is to be avoided.
