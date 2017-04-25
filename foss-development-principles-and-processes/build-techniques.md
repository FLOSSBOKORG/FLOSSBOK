# Build Techniques

---

## Build Process

In the context of software development, build refers to the process that converts files and other assets under the developers' responsibility into a software product in its final or consumable form. The build process usually include compiling source codes, generating manifest file, producing installer, copying and moving files around among different directories, and packaging binary files, running unit tests, etc. 

## Build Tools/Frameworks

There are many open-source build frameworks available, such as make, Ant, Maven, rake, etc. Most of these tools allows you to automate these repeatable build process and tasks.

### Ant

Apache Ant is a Java library and command-line tool whose mission is to drive processes described in build files as targets and extension points dependent upon each other. The main known usage of Ant is the build of Java applications.

### Maven

Maven is another build framework for Java applications, whose primary goal is to allow a developer to comprehend the complete state of a development effort in the shortest period of time. Maven can manage a project's build, reporting and documentation from a central piece of information.

## Continuous Integration

![](/assets/ci_flow.png)

Continuous Integration \(CI\) is a practice of merging all developer working copies to a shared mainline several times a day. Before continuous integration, build automation is a prerequisite. The CI server is usually linked to the version control system \(e.g. Git, SVN\) and supports build tools/frameworks mentioned out of the box. Before checking into the code, developers should run automated unit tests on their local machine to ensure their changes won’t break the build. The build server, as part of the CI process, periodically run automated unit and integration tests. Problem are reported to the developers through email or other integrated messenger services. The idea is to apply quality control to the product continuously and hopefully find out any potential problems as quickly as possible. Many open source CI solution are available, such as Jenkin, Travis CI, Strider, CruiseControl, among many others.

