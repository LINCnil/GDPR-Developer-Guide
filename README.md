<p align="center"><img src="https://github.com/LINCnil/GDPR-Developer-Guide/raw/master/templates/BANNIERE-EN.JPG" width="100%" align="middle"></p>


# GDPR Developer Guide

#### In order to assist web and application developers in making their work GDPR-compliant, the CNIL has drawn up a new guide to best practices under an open source license, which is intended to be enriched by professionals.

This guide is published under [license GPLv3](https://www.gnu.org/licenses/gpl-3.0.html) and under [open license 2.0](https://www.etalab.gouv.fr/wp-content/uploads/2017/04/ETALAB-Licence-Ouverte-v2.0.pdf) (explicitly compatible with [CC-BY 4.0 FR](https://creativecommons.org/licenses/by/4.0/deed.fr)). You can freely contribute to its redaction.

The [French version](https://github.com/LINCnil/Guide-RGPD-du-developpeur) is the authentic version of this guide.

#### Is this guide for developers only?

This guide is mainly aimed at developers working alone or in teams, team leaders, service providers but also at anyone interested in web or application development.

It provides advice and best practices, and thus gives useful keys to understand the GDPR for every stakeholder, regardless of the size of their structure. It can also stimulate discussions and practices within the organisations and in customer relationships.

#### What does the guide contain?

This guide is divided into **16 thematic sheets** which cover most of the needs of developers at each stage of their project, from the preparation of the development to the use of analytics.

The General Data Protection Regulation (or GDPR) specifies that the protection of the rights and freedoms of natural persons requires that **"appropriate technical and organisational measures be taken to ensure that the requirements of this Regulation are met"** (Recital 78).

The determination of these measures is necessarily **related to the context of the processing operations put in place**, and the controller (the public or private entity processing personal data) must therefore ensure the security of the data it is called upon to process.

The good practices in this guide **are therefore not intended to cover all the requirements of the regulations nor to be prescriptive**, they provide a first level of measures to take into account privacy protection issues in IT developments that are intended to be applied to all data processing projects. Depending on the nature of the processing carried out in certain cases, additional measures will have to be implemented in order to fully comply with the regulations.

## Table of contents

0. [Develop in compliance with the RGPD](#Sheet_n°0_:_Develop_in_compliance_with_the_RGPD)

1. [Identify personal data](#Sheet_n°1_:_Identify_personal_data)

2. [Prepare your development](#Sheet_n°2_:_Prepare_your_development)

3. [Securing your development environment](#Sheet_n°3_:_Securing_your_development_environment)

4. [Manage your source code](#Sheet_n°4_:_Manage_your_source_code)

5. [Make an informed choice of architecture](#Sheet_n°5_:_Make_an_informed_choice_of_architecture)

6. [Securing your websites, applications and servers](#Sheet_n°6_:_Securing_your_websites,_applications_and_servers)

7. [Minimize data collection](#Sheet_n°7_:_Minimize_data_collection)

8. [Manage user profiles](#Sheet_n°8_:_Manage_users_profiles)

9. [Control your libraries and SDKs](#Sheet_n°09_:_Control_your_libraries_and_SDKs)

10. [Ensure the quality of the code and its documentation](#Sheet_n°10_:_Ensure_quality_of_the_code_and_its_documentation)

11. [Test your applications](#Sheet_n°11_:_Test_your_applications)

12. [Inform users](#Sheet_n°12_:_Inform_users)

13. [Prepare to exercise people's rights](#Sheet_n°13_:_Prepare_for_the_exercise_of_people_rights)

14. [Define a data retention period](#Sheet_n°14_:_Define_a_data_retention_period)

15. [Take into account the legal basis in the technical implementation](#Sheet_n°15_:_Take_into_account_the_legal_bases_in_the_technical_implementation)

16. [Use analytics on your websites and applications](#Sheet_n°16:_Use_analytics_on_your_websites_and_applications)



## How can I contribute to this guide?

**This guide is available in two versions**:

* A [web version on the CNIL website](http://www.cnil.fr/en/rgpd-developers-guide) and in the tab [the "Releases" tab](https://github.com/LINCnil/GDPR-Developer-Guide/releases) of this repository;
* This [GitHub version](https://github.com/LINCnil/GDPR-Developer-Guide), which offers the possibility for everyone to contribute.

**The contribution is done in a few steps**:

* Register on Github;
* Go to the project page;
* You can:
    * Use the "Issue" tab to open comments or participate in the discussion
    * Use the "Fork" option to make your own modifications and propose their inclusion via the "Pull Requests" button.

**Your contribution proposal will be examined by the CNIL before publication**. The web version of the RGPD developer's guide will be regularly updated.

## Usage


To release this repository yourself, you can use the **Pandoc** tool. This tool will allow you to convert the records into a docx file or an HTML document.

You can find the instructions to install this tool [here]( https://pandoc.org/installing.html)

* **To generate a .docx file**:

```bash
pandoc -s --toc --toc-depth=1 -o Guide_RGPD_developper.docx [0-9][0-9]*.md
```

* **To generate an .html file**:

```bash
pandoc -s --template="templates/mytemplate.html" -H templates/pandoc.css -o index.html README.md [0-9][0-9]*.md
```
