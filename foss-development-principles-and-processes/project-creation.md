# Project Creation

**Defining goals**: Identify what is your project's vision and what are target users

These days, it seems that anybody who writes a piece of code ends up pushing it to GitHub with an open-source license and says, “I’ve open-sourced it.” Creating an open-source project isn’t just about making your code freely available to others. So, before announcing to the world that you have open-sourced something that hasn’t been used by anyone other than you in your spare time, stop to ask yourself what your goals are for the project.

The first goal is always to create something useful.Make sure that what you’re offering is useful by looking for others who are doing similar projects and figuring out how large of a user base you’re looking at.

After that, decide why you are open-sourcing the project in the first place. Is it because you just want to share what you’ve done? Do you intend to continue developing the code, or is this just a snapshot that you’re putting out into the world? If you have no intention of continuing to develop the code, then the rest of this article doesn’t apply to you. Make sure that the readme file in your repository states this clearly so that anyone who finds your project isn’t confused.

If you are going to continue developing the code, do you want to accept contributions from others? If not, then, once again, this article doesn’t apply to you. If yes, then you have some work to do. Creating an open-source project that’s conducive to outside contributions is more work than it seems. You have to create environments in which those who are unfamiliar with the project can get up to speed and be productive reasonably quickly, and that takes some planning.

**Choosing A License: **The license is aim to protect the contributors' right

Before you share your code, the most important decision to make is what license to apply. The open-source license that you choose could greatly help or hurt your chances of attracting contributors. All licenses allow you to retain the copyright of the code you produce. While the concept of licensing is quite complex, there are a few common licenses and a few basic things you should know about each. \(If you are open-sourcing a project on behalf of a company, please speak to your legal counsel before choosing a license.\)

GPL

The GNU Public License was created for the GNU project and has been credited with the rise of Linux as a viable operating system. The GPL license requires that any project using a GPL-licensed component must also be made available under the GPL. To put it simply, any project using a GPL-licensed component in any way must also be open-sourced under the GPL. There is no restriction on the use of GPL-licensed applications; the restriction only has to do with the modification and distribution of derived works.

LGPL

The Lesser GPL is a slightly more permissive version of GPL. An LGPL-licensed component may be linked to from an application without the application itself needing to be open-sourced under GPL or LGPL. In all other ways, LGPL is the same as GPL, so any derived works must also be open-sourced under GPL or LGPL.

MIT

Also called X11, this licence is permissive, allowing for the use and redistribution of code so long as the license and copyright are included along with it. MIT-licensed code may be included in proprietary code without any additional restrictions. Additionally, MIT-licensed code is GPL-compatible and can be combined with such code to create new GPL-licensed applications.

BSD3

This is also a permissive license that allows for the use and redistribution of code as long as the license and copyright are included with it. In addition, any redistribution of the code in binary form must include a license and copyright in its available documentation. The clause that sets BSD3 apart from MIT is the prohibition of using the copyright holder’s name to promote a product that uses the code. For example, if I wrote some code and licensed it under BSD3, then an application that uses that code couldn’t use my name to promote the product without my permission. BSD3-licensed code is also compatible with GPL.

There are many other open-source licenses, but these tend to be the most commonly discussed and used.**Documentation: **Document the basic rules for the FOSS, decide an order for the community to follow.

**Use Version Numbers: **The version number is aim to provide a mechanism to provide

One common mistake made with open-source projects is neglecting to use version numbers. Version numbers are incredibly important for the long-term stability and maintenance of your project. When bugs came in, I had no idea whether people were using the most recent version because there was no way for them to tell when the code was released. Bugs were being reported that had already been fixed, but there was no way for the end user to figure that out.

Stamping each release with an official version number puts a stake in the ground. When somebody files a bug, you can ask what version they are using and then check whether that bug has already been fixed. This greatly reduced the amount of time I spent with bug reports because I was able to quickly determine whether someone was using the most recent version.

Unless your project has been previously used and vetted, start the version number at 0.1.0 and go up incrementally with each release. Don’t get me wrong: there are no set rules on how to increase version numbers in a project, though there are a couple of resources worth looking at: Apache APR Versioning and Semantic Versioning. Just pick something and stick with it.

In addition to helping with tracking, version numbers do a number of other great things for your project.

**Managing Contributions: **Allow committee to supervise each merge on the project to ensure the safety of the project.

Once you have everything set up, the next step is to figure out how you will accept contributions. Your contribution model can be as informal or formal as you’d like, depending on your goals. For a personal project, you might not have any formal contribution process. The developer guide would lay out what is necessary in order for the code to be merged into the repository and would state that as long as a submission follows that format, then the contribution will be accepted. For a larger project, you might want to have a more formal policy.

The first thing to look into is whether you will require a contributor license agreement \(CLA\). CLAs are used in many large open-source projects to protect the legal rights of the project. Every person who submits code to the project would need to fill out a CLA certifying that any contributed code is original work and that the copyright for that work is being turned over to the project. CLAs also give the project owner license to use the contribution as part of the project, and it warrants that the contributor isn’t knowingly including code to which someone else has a copyright, patent or other right. jQuery, YUI and Dojo all require CLAs for code submissions. If you are considering requiring a CLA from contributors, then getting legal advice regarding it and your licensing structure would be worthwhile.

Next, you may want to establish a hierarchy of people working on the project. Open-source projects typically have three primary designations:

Contributor

Anyone who has had source code merged into the repository is considered a contributor. The contributor cannot access the repository directly but has submitted patches that have been accepted.

Committer

People who have direct access to the repository are committers. These people work on features and fix bugs regularly, and they submit code directly to the repository.

Reviewer

The highest level of contributor, reviewers are commanders who also have directional impact on the project. Reviewers fulfill their title by reviewing submissions from contributors and committers, approving or denying patches, promoting or demoting committers, and generally running the project.

If you’re going to have a formal hierarchy such as this, you’ll need to draft a document that describes the role of each type of contributor and how one may be promoted through the ranks. YUI has just created a formal “Contributor Model,” along with excellent documentation on roles and responsibilities.

