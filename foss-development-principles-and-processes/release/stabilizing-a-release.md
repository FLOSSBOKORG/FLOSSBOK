# Stabilizing a Release

Stabilization is the process of getting a release branch into a releasable state which is the process of deciding which changes will be in the release and which will not, then shaping the branch content accordingly.

There will always be situations where the team needs to make a decision whether a given change should be added to a release. This process could have danger since each person wants to see their own favorite changes added into the release. So then there will be many people trying to allow changes, while not enough people trying to bar them.

Thus, stabilizing a release is actually about creating mechanisms for saying "no". You need be able to say "no" but don't result in too many hurt feelings or disappointed developers, and also won't prevent deserving changes from getting into the release. Here are two ways of doing it.

## Dictatorship by Release Owner

The group agrees to let one person be the release owner. This person has the authority to decide what changes should be added the final release. Normal discussions and arguments are allowed, but in the end the final decision is still made by the release owner. In order to make this system work, the release owner should have technical competence to understand all the changes, and the social standing and people skills to navigate the discussions leading up to the release without causing too many hurt feelings.

Release owner doesn't need not be the same person as the project leader. In fact, sometimes it's good to make sure they're not the same person. Project leader's judgement isn't always true. Then we will need o have someone to provide a counterbalance to the project leader. Project leader needs to discuss with release owner instead of overriding a decision by the release owner, which will undermine the release owner's authority.

## Voting on Changes

As opposed to dictatorship by release owner, every developer can vote on which changes to include in the release. However, since what release stabilization tries to do is to exclude changes, the voting system should be designed in a way that getting a change into the release involves positive supports from multiple developers. The system should be arranged such that subgroups of developers must act in cooperation to get any change into the release. This not only means that more people review each change, it also makes any individual developer less hesitant to vote against a change, because she knows that no particular one among those who voted for it would take her vote against as a personal affront. The greater the number of people involved, the more the discussion becomes about the change and less about the individuals.

### Managing Collaborative Release Stabilization

If your project chooses to use a change voting system, you need to make sure that the physical mechanics of setting up ballots and casting votes are as convenient as possible. Although there is many open source electronic voting software available, actually the easiest thing to do is just to set up a text file in the release branch, called STATUS or VOTES or something like that. This file lists each proposed change and any developer can propose a change, along with all the votes for and against it, including any notes or comments.

### Release Manager

In practice, there are usually one or two people driving the release process, who are called release manager but different from a release owner who has final say over the changes. Release managers' responsibilities includes keeping track of how many changes are currently under consideration, how many have been approved, how many seem likely to be approved and so on. If they sense that important changes are not getting enough attention, they will gently nag other developers to review and vote. When a batch of changes are approved, they will merge them into the release branch. When the time comes to put the release out the door, the release managers also take care of the logistics of creating the final release packages, collecting digital signatures, uploading the packages, and making the public announcement.

