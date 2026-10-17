# Notes made during project implementation
**During every tutorial project, I make notes on what I had to do to achieve the goal. These notes are stored here.**

0) The instructions are again outdated(though much more detailed than usually!). For example, Java 11 is used, though Jenkins support for Java 11 was dropped in 2024. I used Java 21 instead.
1) epel does not have to be installed in order to install JDK.
2) Jenkins interface is changed somewhat as well. I will not list individual changes, they are not that important.
3) Maven is now also installable through the package manager.
4) Java and Maven paths are recognized automatically and do not have to be set manually in Jenkins.(?)
5) In a Tomcat Docker container, the /webapps.dist is actually ./webapps.dist (though maybe the instruction is just unclear and also means this)
6) Password-based .ssh is less safe than key-based .ssh(someone could try and guess the password), and the key-based authentication for a new user is simple to setup anyway. I created a separate key for Jenkins server to access Docker, so that I shouldn't copy the main key there.
7) There is no existing Jenkins job, of course. Either this is the result of a Jenkins update, or this is a part of a bigger tutorial and the old job part was missed out.
8) pom.xml expectes Java 7 instead of a newer version. Also, the Dockerfile included uses Java 17. Both were changed to 21.
9) final change to trigger the pipeline :)