# Release Branches

A release branch is just a branch in the version control system, which is isolated from mainline development. Not only open source software development, but many proprietary development organizations also use them.

Release branches are pretty much important in open source projects. If you don't use it, it could lead to bad results. First, the overall development process is slowed. Second, the release's quality will be poorer because there were only a few people working on it, and they want to finish it in a hurry so everyone else could get back to work, while others are just sitting idle. Third, it divides the development team psychologically, by setting up a situation in which different types of work interfere with each other unnecessarily.

## Mechanics of Release Branches

A branch usually is generated from another branch or from the trunk. The trunk is where main development is. When the release branch is generated and stabilized, it is time to tag a snapshot from the branch with a name like, e.g., "1.0.0". The resultant tag represents the exact state of the project's source tree in the 1.0.0 release . The next micro release in the same line is likewise prepared on the 1.0.x branch, and when it is ready, a tag is made for 1.0.1. When it's time to start thinking about a 1.1.x release, make a new branch from trunk.

Maintenance can be in parallel along with both 1.0.x and 1.1.x, and releases can be made independently from both lines

In fact, it is usual to publish two close releases from two different lines. The older series is made for conservative users who just want stable software while more adventurous people are more willing to have a try of the new release to get the newest features even there could be instability and risks.

This is not the only release branch strategy. You can use any strategy you think it could work. But there is one point you should always follow: the purpose of using a release branch is to isolate release work from the daily development and its instability.

