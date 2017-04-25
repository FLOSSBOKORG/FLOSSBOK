# **Version Control**

---

Version control is a system that records changes to a file or set of files over time so that specific versions can be recalled later. A version control system serves the following purposes:

* Version control enables multiple people to simultaneously work on a single project. Each person edits his or her own copy of the files and chooses when to share those changes with the rest of the team. Thus, temporary or partial edits by one person do not interfere with another person’s work.

* Version control enables one person to use multiple computers to work on a project.

* Version control integrates work done simultaneously by different team members. In most cases, edits to different files or even the same file can be combined transparently. When conflicts happens, the version control system may request human assistance.

* Version control gives access to historical versions of a project. This is insurance against system failures or data lossage. It supports rolling back to a previous version. For any part of a file, people can determine when, why, and by whom it was ever edited.

## **System Components**

Version control uses a repository \(a database of changes\) and a working copy where people do their work. Working copy \(sometimes called a checkout\) is the personal copy of all the files in the project. A repository is a database of all the edits to, and/or historical versions \(snapshots\) of, the project. Repository may contain edits that have not been applied to personal working copy.

A version control system lets multiple users simultaneously edit their own copies of a project. Usually, it is able to merge simultaneous changes by two different users. A conflict occurs when two different users make simultaneous, different changes to the same line of a file. In this case, the version control system cannot automatically decide which of the two edits to use. Manual intervention is required to resolve the conflict.

## Types of Version Control Systems

There are two general varieties of version control: centralized and distributed. The main difference between centralized and distributed version control is the number of repositories. In centralized version control, there is just one repository, and in distributed version control, there are multiple repositories. Here are pictures of the typical arrangements:

![](https://lh6.googleusercontent.com/aDK3zQ0ftlZdkZQJ0d2cBzI8zzl0nK0tjmpiy23072WuXSlzZzBz3ytndLDj0W-iElcWYX-Stx5NUTtYmUasGr1U9JHm8pDf6vsufpuckZkC-gOGFEZl1iFMgo0LyML8JeGYJ3Ho)![](https://lh6.googleusercontent.com/gVIdJFm3uThjwjhq0iYNoCparkx5IQPSejpKZzmS-jyfdgNzuZVrLEG4HsWbJUnOIDv3sRW632_6ed-Bk-f9bcuIWo3XP-H_3BwraA7GRzzvlf9Xvt6MygXY6jgVDVgsf3ez6_zV)

In centralized version control, each user gets his or her own working copy, but there is just one central repository. In distributed version control, each user gets his or her own repository and working copy. Centralized version control has been used by many open source projects for a long time. However, in recent years most widely-known projects have migrated their repositories to distributed version control. Distributed version control is more modern, runs faster, is less prone to errors, has more features, and is somewhat more complex to understand.

