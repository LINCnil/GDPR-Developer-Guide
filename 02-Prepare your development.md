# Sheet n°2: Prepare your development

#### The principles of personal data protection must be integrated into IT developments from the design phase onwards in order to protect the privacy of the people whose data you are going to process, to give them better control over their data and to limit errors, losses, unauthorised modifications or misuses of their data in applications.

## Methodological choices

* **Put privacy protection at the center of your developments** by adopting a [Privacy By Design](https://edpb.europa.eu/our-work-tools/public-consultations-art-704/2019/guidelines-42019-article-25-data-protection-design_en) methodology.

* If you use agile methods for your developments, consider **integrating security at the center of your process**. The ANSSI has made available a guide ["digital security & agility"](https://www.ssi.gouv.fr/uploads/2018/11/guide-securite-numerique-agile-anssi-pa-v1.pdf) (in French only) which indicates how to conduct your developments within the framework of an agile method while taking into account the security aspects. Don't hesitate to draw inspiration from it.

* For any development aimed at the general public, **consider the privacy settings**, and in particular the default settings, such as the characteristics and user content visible by default.

* **Conduct a [Privacy Impact Assessment (PIA)](https://www.cnil.fr/en/privacy-impact-assessment-pia)**. For [certain processing operations](https://ico.org.uk/for-organisations/guide-to-data-protection/guide-to-the-general-data-protection-regulation-gdpr/accountability-and-governance/data-protection-impact-assessments/) it is mandatory. In other cases it is a good practice that will allow you to identify and deal with all the risks upstream of your developments. The CNIL has a special section on its website and provides a [free software](https://www.cnil.fr/en/open-source-pia-software-helps-carry-out-data-protection-impact-assesment) dedicated to this type of analysis.


## Technological choices

#### Architecture and features

* **Include privacy protection, including data security requirements, at the design stage of the application or service**. These requirements should influence [architecture choices](#Sheet_n°5:_Making_an_informed_choice_of_architecture) (e.g. decentralized vs. centralized) or functionality (e.g. short term anonymization, data minimization). The default settings of the application must meet minimum security requirements and comply with the law. For example, the default complexity of passwords must comply at least with the [CNIL recommendation on passwords](https://www.cnil.fr/fr/node/23803).

* **Maintain control of your system**. It is important to keep control of your system, both to ensure proper operation and to guarantee a high level of security. Keeping a system simple allows you to understand precisely how it works and to identify its weak points. If a certain complexity is required, it is advisable to start with a simple, correctly designed and secure system. Then, it is possible to increase the complexity little by little, while continuing to secure the new features that are added.

* **Don't rely on a single line of defense**. In spite of all the steps taken to design a secure system, it may happen that some components added later may not be sufficiently secure. To minimize the risk to end users, it is advisable to defend the system in depth. For example, checking the data entered in an online form is part of the periphery defenses. If this defense is hijacked, database query protection can take over.

#### Tools and practices

* **Use programming standards that take into account safety**. Often, lists of standards, best practices or coding guides improving the security of your developments are already available. Ancillary tools can also be integrated into your integrated development environments ("**IDE**") in order to automatically check that your code complies with the various rules that are part of these standards or good practices. You can easily find lists of good practices for your favourite programming language on the Internet. For example [here](https://wiki.sei.cmu.edu/confluence/display/seccode/SEI+CERT+Coding+Standards) for C, C++ or Java. For web application development, specific good practice guides exist, such as those published by [OWASP](https://www.owasp.org).

* **The technological choices are critical.** A few parameters need to be taken into account:
    * Depending on the field of application or functionality developed, one language or technology may be more appropriate than another.
    * Time-tested languages and technologies are safer. They have, in general, been audited to correct the most known vulnerabilities. However, you should be careful to use the latest versions of each of the technology building blocks you will be using.
    * You must avoid coding your final solution in a language you have just learned and not yet mastered. Otherwise, you expose yourself to an increased risk of a security flaw due to lack of experience.
* **Set up a secure development environment that allows versioning of the code** by following the [dedicated sheet](#Sheet_n°3:_Secure_your_development_environment) in this guide.
