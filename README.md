# [mM]-Task
## Summary
This task should be a starting point for you before you contributing to an [ag-gipp project](https://github.com/ag-gipp). We are using several techniques and tools to organize our development process. To keep it well structured and organized, every developer must be familiar with those tools before he/she is contributing new code. Please note that successfully finishing this task does not replace project specific contributing guidelines.

This project aims for two goals. One is to solve a problem programmatically, while the other one is to give you the understanding of our workflow and the tools we are using. The [task description](#task-description) explains the task you have to solve. Please follow each point of the [detailed instructions](#detailed-instructions) and at least get familiar with the tools in the [optional features](#optional-features) section. Note that most of the linked guides are comprehensive and way too big for your purposes. It's up to you to find the right dose of information you need.

## Task Description
Write a program in Java which takes an input text file and converts all the m's to M's and all the M's to m's. BTW, this is all it should do. It should not modify the input file in any other way. You should use the text file located at:

https://staff.fnwi.uva.nl/t.h.koornwinder/art/informal/KLSadd.tex

## Detailed Instructions 

<a href="https://github.com"><img align="right" src="https://image.flaticon.com/icons/svg/25/25231.svg" height="28"></a><a href="https://git-scm.com/"><img align="right" src="https://git-scm.com/images/logos/downloads/Git-Logo-2Color.png" height="28"></a>
### Git & GitHub

1. Create a GitHub account and send one of us ([mM-Task Supervisors](https://github.com/orgs/ag-gipp/teams/mm-tasksupervisor/members)) your username.
2. Get familiar with the basics of [Git](https://git-scm.com/book/en/v2/) and [GitHub](https://guides.github.com/activities/hello-world) to achieve the following steps
    1. `Checkout` your project template on your local machine (do not make any changes directly on the GitHub page! Use your terminal or your IDE to work with Git, i.e., pull, commit, push changes.)
    2. Create a file called `README.md` and explain what your project will do, what you need to achieve and how to use the program when finished your task. Put this file in your project parent directory so that it will show up in your GitHub-project start page.
    3. Create a `.gitignore` File and put it into your parent directory.
    4. __Optional:__ in bigger projects, we usually work on multiple branches. To get familiar with this technique, push your first changes to another branch (please use your terminal and not your IDE to see how it works most natively). However, in your task, you are the only developer and the project is small so it is not necessary to work with multiple branches furthermore. Thus, merge the second branch back to `master` and just work on the `master` branch. Don't forget to delete the temporary branch you just created. This keeps your repository clean.

_From now on, push every change to GitHub!_ 

<a href="https://www.jetbrains.com/idea/"><img align="right" src="http://resources.jetbrains.com/storage/products/intellij-idea/img/meta/intellij-idea_logo_300x300.png" height="28"></a><a href="https://maven.apache.org/"><img align="right" src="https://maven.apache.org/images/maven-logo-black-on-white.png" height="28"></a>
### Maven & IntelliJ

3. Familiarize yourself with maven and create a new maven project for your task in your git repository. ([Maven in 5min](http://maven.apache.org/guides/getting-started/maven-in-five-minutes.html), [Introduction to Directory Layouts](http://maven.apache.org/guides/introduction/introduction-to-the-standard-directory-layout.html))
4. Set up an [IDE](https://en.wikipedia.org/wiki/Integrated_development_environment) (we strongly recommend to use [IntelliJ](https://www.jetbrains.com/idea/download/)) for your maven project. 
    * __Tipp:__ if you are using IntelliJ, I recommend this order (maven first, IntelliJ second), because IntelliJ can import an existing maven project quickly, while the other way around can be a bit more tricky when you are new with IntelliJ. This only works when your `pom.xml` is correct. Another maybe helpful website is [IntelliJ's help page for maven](https://www.jetbrains.com/help/idea/maven.html). 
    * __Note:__ it might be obvious for some people, but please aware that starting your program in IntelliJ (pressing green arrow/run button) does not compile your project via maven! Maven is a separate lifecycle. You can control maven either from your terminal or in IntelliJ's [maven project tool window](https://www.jetbrains.com/help/idea/maven-projects-tool-window.html).
5. Update your .gitignore for java and your IDE. Find out the best practice what should be ignored by your own.

<a href="https://travis-ci.com/"><img align="right" src="https://travis-ci.com/images/logos/TravisCI-Mascot-1.svg" height="28"></a><a href="http://junit.org/junit5/"><img align="right" src="http://junit.org/junit5/assets/img/junit5-logo.png" height="28"></a>
### JUnit & Travis

Before you can start actually to develop your code, you should get familiar with the concepts of testing. ([Why Software Testing is Important](https://www.atlassian.com/blog/software-teams/why-software-testing-is-important))

6. Get familiar with JUnit tests ([JUnit Tutorial](http://www.vogella.com/tutorials/JUnit/article.html)) and write a simple dummy test.
7. Run your tests with `mvn`. ([Run Unit Tests with Maven](https://www.mkyong.com/maven/how-to-run-unit-test-with-maven/), [Official Maven Guide for JUnit Tests](http://maven.apache.org/surefire/maven-surefire-plugin/examples/junit.html)).
8. Set up Travis as your continues integration service for your project ([Travis for Beginners](http://docs.travis-ci.com/user/for-beginners/)). Make sure Travis automatically runs your tests when you push new code to GitHub ([Travis setup Java](http://docs.travis-ci.com/user/languages/java/)). 
    * __Tip:__ this is usually achieved by telling Travis to compile the project with maven. When the maven tests failed, Travis failed to build your project.
9. Adding the [travis embedding status image](https://docs.travis-ci.com/user/status-images/) to your README.md, so it appears on your project website on GitHub and everybody can quickly see if your tests run or fail.


<a href="http://www.oracle.com/technetwork/java/index.html"><img align="right" src="https://logos-download.com/wp-content/uploads/2016/10/Java_logo_icon.png" height="32"></a>
### Programming with Java

Finally, you can start to solve the task. Before you start, please note the [optional features](#optional-features) below. They might be redundant, especially when you see that we are not always using them for our actual projects. However, it is good programming practice and 1. and 2. will become officially part of the contributing guidelines in the future for all [ag-gipp projects](https://github.com/ag-gipp).

_From now on, regularly update your test cases when you developing new code or practicing the TDD._

10. Develop a solution for your task (continually uploading and testing your changes)
11. When you think you finished your work, check that
    1. you can build your project with maven (with tests),
    2. your Travis embedding image is green (_passing_) on your GitHub project website,
    3. and your program produces an exact copy of the input file, except for the swapped letters `m` and `M`.
12. Finally, please send your supervisor the input, the output, and also the program with instructions on how to run it. 


<a href="https://medium.com/@rshariffdeen/how-to-tdd-eca446f0bbdb"><img align="right" src="https://cdn-images-1.medium.com/max/1600/1*kHWRvTO6AM0dRqv9de9yKQ.jpeg" height="28"></a><a href="http://checkstyle.sourceforge.net/"><img align="right" src="http://checkstyle.sourceforge.net/images/logo.png" height="28"></a><a href="https://logging.apache.org/log4j/2.x/"><img align="right" src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f9/Apache_Log4j_Logo.png/1200px-Apache_Log4j_Logo.png" height="28"></a>
## Optional Features
The following features are optional but strongly improves your code quality and help everybody to debug and read your code. Most (but not all) of our projects already using those tools. Already implementing them in your current task solution will be highly appreciated.
1. Get familiar with logging via Log4j2 ([Log4j2 Best Practicing](https://examples.javacodegeeks.com/enterprise-java/log4j/log4j-2-best-practices-example/)). Preferably, use `XML` to configure your logging. ([Log4j2 Configuration](https://logging.apache.org/log4j/2.x/manual/configuration.html))
2. Get familiar with [Checkstyle](https://en.wikipedia.org/wiki/Checkstyle) to improve your coding style ([Checkstyle Website](http://checkstyle.sourceforge.net/)). Include Checkstyle to your maven project. This will force maven to check the style of your code whenever you compile your project with maven. Note that this has also effect on your Travis setup!
3. Check [TDD](https://en.wikipedia.org/wiki/Test-driven_development) (Test-driven development). Some developers are pleased using this technique; others don't like it. It's worth to try it once or at least to know what this technique is. ([Practicing TDD in Java](https://technologyconversations.com/2013/12/24/test-driven-development-tdd-best-practices-using-java-examples-2/))

## Final Statement
Please note that this task is not a tutorial to guide you through each tool. You have to figure out each part on your own. We do not claim to become an expert in every mentioned tool, but we expect a basic knowledge from you once you finished this task. Thus, don't lose yourself in hundreds of manual pages but get familiar with the basics that are necessary.

Also, if you have any comments for us, for example how we could improve this task, what was too difficult or too easy, let us know your opinion. We highly appreciate your feedback.

Good luck! 
