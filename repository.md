## What is a repository and why would we want to use it?

Ref: \[Version Control Repository - Wikipedia\]\([https://en.wikipedia.org/wiki/Repository\_\(version\_control](https://en.wikipedia.org/wiki/Repository_%28version_control)\)\)

In open source software development, developers need to find a way to put things together. Essentially, we need a place to store the meta data of our project. This storage place, often known as forges or repositories, is a common practice in version control systems. A repository can store a set of files, and track the changes of them accordingly.

## Different type of repositories

Each revision control system handles storing changes differently. Traditionally, subversions are stored into databases. Nowadays, solutions directly on the filesystem or on the cloud is becoming more common.

## How are repository managed? \(centralized or distributed\)

Depending on the version control system, whether it is centralized or distributed, the whole set of information in the repository may be duplicated on every user's system or may be maintained on a single server.

## What components does a repository have?

Some of the metadata that a repository contains includes, among other things:

* A historical record of changes in the repository.
* A set of commit objects.
* A set of references to commit objects, called heads.

## Example case study

### source forge

[SourceForge](https://sourceforge.net/)  
[SourceForge - Wikipedia](https://en.wikipedia.org/wiki/SourceForge)

SourceForge is a Web-based service that offers software developers a centralized online location to control and manage free and open source software projects. It provides a source code repository.  
Users can create their projects on sourceforge easily.

### github repository

[GitHub](https://github.com/)  
[GitHub - Wikipedia](https://en.wikipedia.org/wiki/GitHub)

GitHub is a web-based Git or version control repository and Internet hosting service. It offers all of the distributed version control and source code management \(SCM\) functionality of Git as well as adding its own features.  It provides access control and several collaboration features such as bug tracking, feature requests, task management, and wikis for every project.

Any user could register a github account and then create his own project repository. The repository could be either private or public. Usually, the repository is licensed with a particular license \(LISENSE.TXT/LICENSE\) and an introduction file \(README/README.md\).

Using the git version control system, a user could create his local repository on his machine, add files and commit to it. With github repository, the user could push/pull changes in the remote repository and keep the file changes synchronized between local and the cloud.

