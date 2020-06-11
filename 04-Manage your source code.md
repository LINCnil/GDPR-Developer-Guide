# Sheet n°4: Manage your source code

#### Whatever the size of your project, it is highly recommended to use a source code management tool, such as a *version control system*,  to track its different versions over time.

## Set up your version control system efficiently, thinking about its security.

* A version control system is a software program that allows you to store **all your source code and associated files**, while keeping the **chronology of all changes** that have been made. A simple FTP server is not a version control system.

* Set up your environment correctly using the features offered by your version control system. It is recommended that you implement strong **authentication** and/or **authentication with SSH keys** at the beginning of your project.

* In addition, assign *levels of access* to your project to the users of your version control system and define for each level the corresponding **permissions** (for example, a "guest" level with limited read rights, a "developer" level with write rights, etc.).

* Make regular **backups** of your source code management system. In particular, remember to back up your main server where all changes are saved.

* Set up development procedures to work efficiently even if **several people are developing at the same time**. For example, you may decide not to work on the same branch (_master_), but to set up feature-based branches, which will be merged into the main branch as development progresses. Such development strategies are already well documented, for example in [Git Flow](https://nvie.com/posts/a-successful-git-branching-model/). In addition, some version control systems offer to set up **protected branches** that prevent unauthorized changes to the files in these branches.


## Be aware of your source code content.

* Implement **code quality metrics tools** that will scan your code as soon as it is _committed_ to check its good quality. You can also add scripts to check these metrics in the [version control system configuration](https://git-scm.com/book/uz/v2/Customizing-Git-Git-Hooks): the _commit_ will be cancelled if the source code is not of sufficient quality.

* Keep your secrets and passwords out of your source code repository:
    * in separate **files, which have not been _committed_**. Remember to use special files from your version control system (such as _.gitignore_ for _Git_) so that you don't _commit_ sensitive files by mistake.
    * in **environment variables**, take care to check that environment variables are not accidentally written to *logs* or displayed when an application error occurs.
    * using [**specific secret or configuration management software**](https://www.digitalocean.com/community/tutorials/an-introduction-to-managing-secrets-safely-with-version-control-systems#using-configuration-management-systems-for-secret-management).  

  Finally, if you need to include such data in your repository, consider **automatically encrypting/decrypting** the files using a *plugin* from your version control system (e.g. [_git-crypt_](https://github.com/AGWA/git-crypt)).

* After a _commit_ that contains personal or other critical data, don't forget to [purge](https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History) [completely](https://help.github.com/en/github/authenticating-to-github/removing-sensitive-data-from-a-repository#purging-a-file-from-your-repositorys-history) the source code repository: even after modification, the data may still be available in your repository history.

* Be careful before **publishing your source code online**. Review **its entire contents** to make sure that no personal data, passwords or other secrets are present, including the entire change history.

## Examples of tools

* Unlike tools such as [Subversion](https://subversion.apache.org/), which need a central server to run, the main version control systems ([Git](https://git-scm.com/), [Mercurial](https://www.mercurial-scm.org/) for example) are **decentralized**.

* For most of these tools, a **web interface and related tools** (bug management, wiki for your documentation, etc.) are provided. These solutions can either be accessible via the internet ([GitHub](https://github.com/), [Bitbucket](https://bitbucket.org/), etc.), or they can be integrated into your own servers.
