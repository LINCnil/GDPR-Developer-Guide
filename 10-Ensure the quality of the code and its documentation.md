# Sheet n°10: Ensure quality of the code and its documentation

#### It is essential to adopt good code-writing techniques as soon as possible. Code readability reduce the effort of maintenance and bug fixes over time for you and your (possibly future)collaborators.

## Document code and architecture

* Documentation is sometimes left out during development, due to lack of time or visibility on the project. However, it is **crucial for the maintainability of your project**: it allows you to understand how the code works globally, and to know which parts of the code are affected by a modification.

* **Document the architecture, not just the code**: you need to be able to keep the big picture in mind when you write your documentation and help developers understand how all your components work together. Therefore, focus on diagrams and clear explanations when documenting your project.

* **Maintain the documentation along with the code**: The best way to keep your documentation up to date is to modify it as you go along with the code.

* If you use a source code manager, you can also include documentation changes for each "_commit_" that modifies your code (see in particular [the "Manage your source code" form](#Sheet_n°4_:_Manage your source code)).

* **Do not forget to address security in your documentation**. In particular, you can document the different configuration choices for your application, and explain which settings are the most secure.

## Check the quality of your code and its documentation.

* A quality code involves **adoption of good practices and coding conventions** applied consistently throughout the program. It is also best to refer to [existing conventions](https://github.com/Kristories/awesome-guidelines). Here are a few examples of good practice:
    * **Using explicit variable and function names** makes it easier to understand what is going on at first glance.
    * **Correctly indenting your code** allows you to see the structure of the code more quickly.
    * **Avoiding code redundancy** reduces the correction efforts that have to be made in several places. An oversight is quickly forgotten.

* **Tools can help you control the quality of your code**. Once correctly set up, they will avoid re-reading the code to check the correct implementation of coding conventions. Example of these tools are:

    * **Integrated development environments** ("_IDE_"), possibly using plugins ("_plugins_"), can be configured to respect code indentation rules, line breaks between different portions of code, or the position of braces and other parentheses.
    * **Source code quality measurement software** can report code duplications, compliance with programming rules or potential bugs.
