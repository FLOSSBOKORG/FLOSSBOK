# Maintaining Multiple Release Lines

Most mature projects have multiple release lines in parallel. This means that they can have release 1.0.0, 1.0.1 and 1.0.2 while they also have the release 1.1.0. They will maintain both lines simultaneously. This is good because users are very careful about upgrade. So most of them will keep using the current old version until the new version has a stable release, then they will try to upgrade. But there are also adventurers who like to try the new features in the new version first. So it can satisfy both users by having multiple release lines in parallel.

After the 1.1.x line is more stable, the 1.0.x line can be cut. This can be announced in 1.1.x release announcement, or in a separate announcement. But no matter way you use, you need to let users know so that they can make upgrade decisions accordingly.

Some projects still have a time window in which they previous release lines are still maintained, which means that they still accept bug reports and making maintenance releases when significant bugs are found. Other projects don't give this kind support for previous lines anymore, but they watch incoming bug reports to calculate how many people are still using the older line. When the percentage drops below a certain point, they will cut that line.

## Security Releases

A security release is a release made to close a security vulnerability. Without security release, the code that fixes the bug cannot be made public until the release is available. Only the developers can examine the fix among themselves, and test the release privately, but widespread real-world testing is not possible.To solve this lack of test, a security release will consist of some existing release plus the fixes for the security bug, with no other changes to ensure no other bugs will be added.

To indicate the security release, you can add an extra component to an existing release . For example, usually, 1.1.2.1 is a security release against 1.1.2, since it contains a fourth component. 

