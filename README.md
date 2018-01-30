# [mM]-Task
## Summary
This task should be a starting point for you before you contributing to an [ag-gipp project](https://github.com/ag-gipp). We are using several techniques and tools to organize our development process. To keep it well structured and organized, every developer must be familiar with those tools before he/she is contributing new code. Please note that finishing this task succesfully do not replace project specific contributing guide lines.

This task aims not only for solving a problem programmatically but also should show you all the tools we are using. The [task description](#task-description) explains the task you have to solve. Please follow each point of the [detailed instructions](#detailed-instructions) and at least get familiar with the tools in the optional instructions.

## Task Description
Write a program in Java which takes an input text file and converts all the m's to M's and all the M's to m's. BTW, this is all it should do. It should not modify the input file in any other way. You should use the text file located at:

https://staff.fnwi.uva.nl/t.h.koornwinder/art/informal/KLSadd.tex

## Detailed Instructions
1. Create a GitHub account and send one of us ([mM-Task Supervisors](https://github.com/orgs/ag-gipp/teams/mm-tasksupervisor/members)) your username.
2. Get familiar with the basics of [Git](https://git-scm.com/book/en/v2/) and [GitHub](https://guides.github.com/activities/hello-world) and do the following steps
    1. Checkout your project template on your local machine
    2. Create a file called README.md and explain what your project will do, what you need to achieve and how to use the program when you are done. Put this file in your project parent directory.
    3. Create a .gitignore file (look at the linked Git-Guide if you don't know what it is).

_From now on, push every changes to GitHub!_ 

Note we usually work on different branches. To get familiar with this technique, push your first changes to another branch. However, in your task this is not necessary. So merge the second branch to master and just work on the master branch.

3. Familiarize yourself with maven and create a new maven project for your task in your git repository. ([Maven in 5min](http://maven.apache.org/guides/getting-started/maven-in-five-minutes.html), [Introduction to Directory Layouts](http://maven.apache.org/guides/introduction/introduction-to-the-standard-directory-layout.html))
4. Set up an [IDE](https://en.wikipedia.org/wiki/Integrated_development_environment) (we strongly recommend to use [IntelliJ](https://www.jetbrains.com/idea/download/)) for your maven project.
5. Update your .gitignore for java and your IDE.

Before you can start to actually develop your code you should get familiar with the concepts of testing. ([Why Software Testing is Important](https://www.atlassian.com/blog/software-teams/why-software-testing-is-important))

6. Get familiar with JUnit tests ([JUnit Tutorial](http://www.vogella.com/tutorials/JUnit/article.html)) and write a simply dummy test.
7. Run your tests with `mvn`. ([Run Unit Tests with Maven](https://www.mkyong.com/maven/how-to-run-unit-test-with-maven/), [Official Maven Guide for JUnit Tests](http://maven.apache.org/surefire/maven-surefire-plugin/examples/junit.html)).
8. Set up travis as your continues integration service for your project ([Travis for Beginners](http://docs.travis-ci.com/user/for-beginners/)). Make sure travis automatically runs your tests when you push new code to GitHub ([Travis setup Java](http://docs.travis-ci.com/user/languages/java/)). __Tip:__ this is usually achieved by telling travis to compile the project with maven. When the maven tests failed, travis failed to build your project.
9. Adding the [travis embedding status image](https://docs.travis-ci.com/user/status-images/) to your README.md

Finally you can start to solve the task. Before you start, please note the [optional features](#optional-features) below. They might be redundant, espescially when you see that we are not always using them for our actual projects. However, it is good programming practice and we working on introducing them (at least 1. and 2.) to all [ag-gipp projects](https://github.com/ag-gipp).

_From now on, constantly update your test cases when you developing new code or practicing the TDD._

10. Develop a solution for your task (constantly uploading and testing your changes)
11. When you think you are done, check the following points
    1. You can build your project with maven
    2. Travis embedding image is green (_passing_) on your GitHub project side
    3. Your program didn't change the original input file
12. Finally, please send your supervisor the input, the output, and also the program with instructions on how to run it. 

## Optional Features
The following features are optional but strongly improves your code quality and helps everybody to debug and read your code. Most (but not all) of our projects already using those tools. It is strongly recommended to get at least familiar with them. Implementing them in your task solution will be highly appreciated.
1. Logging via Log4j2.
2. Checkstyle
3. Check [TDD](https://en.wikipedia.org/wiki/Test-driven_development) (Test-driven development). Some developers are very happy using this techniques, others don't like it. It's definetly worth to try it once or at least knowing what this technique is. ([Practicing TDD in Java](https://technologyconversations.com/2013/12/24/test-driven-development-tdd-best-practices-using-java-examples-2/))

## Final Statement
Please note that this task is not a tutorial to guide you through each tool. You have to figure out each part by your own. We do not claim to become an expert in every mentioned tool but we expect a basic knowledge from you when you finished this task. Thus, don't loose yourself in hundreds of manual pages. 

Good luck! 
