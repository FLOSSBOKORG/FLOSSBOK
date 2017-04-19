Centralized version control systems are based on the idea that there is a single “central” copy of your project somewhere \(probably on a server\), and programmers will “commit” their changes to this central copy.

“Committing” a change simply means recording the change in the central system. Other programmers can then see this change. They can also pull down the change, and the version control tool will automatically update the contents of any files that were changed.

Most modern version control systems deal with “changesets,” which simply are a groups of changes \(possibly to many files\) that should be treated as a cohesive whole. For example: a change to a C header file and the corresponding .c file should always be kept together.

Centralized version control solves the problems described in the the article about [Version Control](/version-control.md). Programmers no longer have to keep many copies of files on their hard drives manually, because the version control tool can talk to the central copy and retrieve any version they need on the fly.

Some of the most common centralized version control systems you may have heard of or used are CVS, Subversion \(or SVN\) and Perforce.

## A Typical Centralized Version Control Workflow {#WhatisVersionControl-ATypicalCentralizedVersionControlWorkflow}

When you’re working with a centralized verison control system, your workflow for adding a new feature or fixing a bug in your project will usually look something like this:

* Pull down any changes other people have made from the central server.
* Make your changes, and make sure they work properly.
* Commit your changes to the central server, so other programmers can see them.



