# Testing and Releasing

Before the distribution of the public release is made available to the world at large, there should be some tests and made approved by some minimum number of developers. Those approvals must then be signaled to the world at large, using digital signatures and identifying hashes. By using the digital signatures and hashes, users can verify that the copy they receive has not been maliciously tampered with. In most projects, the developers just use their personal digital signatures, and there could be as many developers as they want to sign. The more signs, the more testing the release undergoes, and more secure the release is.

Once approved, the release should be accompanied by the digital signatures and hashes in the project's download area. One way is to accompany each released package with a file giving the corresponding digital signatures, and another file giving the checksum. For example, if one of the released packages is software-2.1.0.tar.gz, place in the same directory a file software-2.1.0.tar.gz.asc containing the digital signature for that tarball, another file software-2.1.0.tar.gz.md5 containing its MD5 checksum, and another software-2.1.0.tar.gz.sha256, containing its SHA256 checksum, etc. A different way to provide checking is to collect all the signatures for all the released packages into a single file, software-2.1.0.sigs; the same may be done with the checksums.

## Candidate Releases

Usually for projects containing many changes, release candidates can be released first, such as software-2.1.0-beta1 before software-2.1.0 so that the candidate releases code can have a wide testing before publishing the official release. If bugs are found, they can be fixed and the new candidate release will be released \(software-2.1.0-beta2\). The process continues until no unacceptable bugs are left, then the last candidate release can be the real official release.

A candidate release should be treated the same as a real release. The alpha, beta, or rc qualifier is enough to warn conservative users to wait until the real release. What's more, the announcement emails for the candidate releases should point out the purpose of candidate releases. The candidate releases is a good way to uncover bugs.

## Announcing Releases

Announcing a release is like announcing any other event, and should use the procedures described in the section called “Publicity” in Chapter 6, Communications. There are a few specific things to do for re- leases, though.

Whenever you write the URL to the downloadable release tarball, make sure to also write the MD5/ SHA1 checksums and pointers to the digital signatures file. Since the announcement happens in multi- ple forums \(mailing list, news page, etc.\), this means users can get the checksums from multiple sources, which gives the most security-conscious among them extra assurance that the checksums themselves have not been tampered with. Meanwhile, giving the link to the digital signature files multiple times doesn't make those signatures more secure, but it does reassure people \(especially those who don't fol- low the project closely\) that the project takes security seriously.

In the announcement email, and on news pages that contain more than just a blurb about the release, make sure to include the relevant portion of the CHANGES file, so people can see why it might be in their interests to upgrade. This is as important with candidate releases as with final releases; the presence of bugfixes and new features is important in tempting people to try out a candidate release.

Finally, don't forget to thank the development team, the testers, and all the people who took the time to file good bug reports. Don't single out anyone by name, though, unless there's someone who is individ- ually responsible for a huge piece of work, the value of which is widely recognized by everyone in the project. Be wary of sliding down the slippery slope of credit inflation \(see the section called “Credit” in Chapter 8, Managing Participants\).

