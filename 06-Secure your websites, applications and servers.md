# Sheet n°6: Secure your websites, applications and servers

#### Any website, application or server must incorporate basic state-of-the-art security rules, not only on network communications but also on authentication and infrastructure.

## Securing communication networks

* **Implement TLS version 1.2 or 1.3** (replacing SSL) on all websites and for data transmissions of your mobile applications, for example with [LetsEncrypt](https://letsencrypt.org/fr/), using only the most recent versions and checking its correct implementation.

* **Make the use of TLS mandatory** for all pages of your site and for your mobile applications.

* **Limit the communication ports** strictly necessary for the proper functioning of the installed applications. If access to a web server is only possible using the HTTPS protocol, only ports 443 and 80 of this server must be accessible, all other ports can be blocked by the firewall.

* **The OWASP has published on its website some cheatsheets** for exemple to [correctly implement TLS](https://cheatsheetseries.owasp.org/cheatsheets/Transport_Layer_Protection_Cheat_Sheet.html) or to [secure a webservice](https://cheatsheetseries.owasp.org/cheatsheets/Web_Service_Security_Cheat_Sheet.html).

## Securing Authentications

* **Follow [the CNIL recommendation on passwords](https://www.cnil.fr/fr/node/23803)**. In particular, remember to limit the number of access attempts.

* **Never store passwords in clear text**. Store them as a hash using a proven library, such as [bcrypt](https://en.wikipedia.org/wiki/Bcrypt).

* **If cookies are used for authentication**, it is recommended:

    * to force the use of HTTPS via [HSTS](https://en.wikipedia.org/wiki/HTTP_Strict_Transport_Security);

    * to use the `secure` flag;

    * use the `HttpOnly` flag.

* **Test the cryptographic suites installed on the systems** and disable obsolete ones (RC4, MD4, MD5 etc.). Encourage the use of AES256. [Read the OSWAP note on the subject](https://cheatsheetseries.owasp.org/cheatsheets/Cryptographic_Storage_Cheat_Sheet.html).

* **Adopt a specific password policy for administrators**. Change the passwords, at least, each time an administrator leaves and in case of suspected breach. Encourage strong authentication when possible.

* **Limit access to administration tools and interfaces to qualified staff.** Encourage the use of lower-privilege accounts for day-to-day operations.

* **Remote access to administration interfaces should be subject to increased security measures.** For example, for internal servers, implementing a VPN with strong authentication of the user and the workstation he or she is using may be a good solution.

## Securing infrastructures

* **Make backups, if possible encrypted and checked regularly**. This is especially useful in case of a ransomware attack on your systems as having backups for all your systems will be the only measure that will allow you to restore your systems.

* **Limit the size of the software stack used,** and for each element of the stack:

    * **Install critical updates** without delay by scheduling an automatic weekly check;
    * **Automate a vulnerability watch** by subscribing to the [NVD Data Feeds](https://nvd.nist.gov/vuln/data-feeds) for example.

* **Use vulnerability detection tools** for the most critical processes to detect possible security breach. Systems for detecting and preventing attacks on critical systems or servers can also be used. These tests must be conducted regularly and before any new software version is put into production.

* **Restrict or fordbid physical and software access to diagnostic and remote configuration ports.** For example, you can list all open ports using the *netstat* tool.

* **Protect the databases you make available on the Internet**, at least by restricting access as much as possible (for example, by IP filtering) and by changing the default password for the administrator account.

* In terms of database management, good practices include:

    * **using nominative accounts** for database access and create specific accounts for each application;
    * **revoking the administrative privileges** of user or application accounts to avoid modification to database structure (table, vues, process, etc);
    * having protection against SQL or script injection attacks;
    * encouraging at rest disk and database encryption.
