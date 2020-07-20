# Sheet n°09: Control your libraries and SDKs

#### Do you use libraries, SDKs, or other software components written by third parties? Here are a few tips on how to integrate these tools while keeping control of your developments.

## Make an informed choice

* **Assess the value of adding each dependency.** Some commonly used software bricks are only a few lines long. However, each added element is an increase in your system's attack surface. In the case where a single library offers several functionalities, integrate only the functionalities you actually need. By activating the minimum number of functionalities, you reduce the number of potential bugs that could occur.

* **Choose maintained software, libraries and SDKs:**

    * If you want to use free or open source software, try to choose projects or solutions with an active community, regular updates and good documentation.

    * If you use other types of solutions with commercial support, contractually ensure that the code will be maintained and updated for the life of your project.

* **Take privacy into account.** Some SDKs or libraries pay for themselves by using personal data collected from the applications or sites on which they are integrated. Make sure that such third parties comply with applicable laws regarding personal data, including a mechanism for obtaining user consent.

* **If you use cryptographic mechanisms, it is strongly discouraged to implement cryptographic algorithms or protocols yourself**, but rather try to choose cryptographic libraries that are maintained, recognized and easy to use.

## Evaluate the selected elements

* **Read the documentation and change the default configurations**. It is important to know how your dependencies work. Third party libraries and SDKs often come with default configuration files, which are rarely changed due to lack of time, which causes many security holes.
* **Audit your libraries and SDKs.** Do you really know what all the libraries and SDKs you integrate do? What data is sent through these dependencies and to whom? This audit will allow you to determine the data protection obligations to be respected and to establish the responsibility of the actors.
* **Map your dependencies.** Third-party libraries and SDKs can also integrate other components: auditing their code will allow you to better map all your dependencies and to better act if a problem affects one of them. It is also recommended that you perform security audits of your third-party components and monitor them.
* **Beware of [typosquatting](https://en.wikipedia.org/wiki/Typosquatting) and other malicious techniques.** Check the names of dependencies, as well as their own dependencies to avoid attacks. Do not copy and paste command lines from unknown sites.

## Maintain libraries and SDKs

* **Use dependency management systems** (such as yum, apt, maven, pip, etc.) to maintain an up-to-date list of your dependencies.
* **Manage updates to your dependencies,** especially in the case of security updates that fix vulnerabilities. You must set up a documented procedure to manage and deploy them as soon as possible.
* **Be aware of the versions of libraries and SDKs at the end of support** that will no longer be maintained: try to find another solution (choose a new library, renew commercial support).
* **Check the status of open-source projects,** especially the change of domain or package ownership, some attacks using malicious updates of popular dependencies.
