# Releasing Number

Before talking about how to make a release, we need to first take a look at how to name releases, and what are contained in the release name. A release means that:

* Some old bugs have been fixed.
* New bugs have been added, except sometimes in the case of security releases or other one-offs.
* New features may have been added.
* New configuration options may have been added, or the meanings of old options may have changed subtly.
* Incompatible changes may have been introduced.

As you can see, not all of things new release may have are good. This is why experienced users approach new releases with some trepidation, especially when the software is mature and was already mostly doing what they wanted.   
Therefore, there are two purposes of release numbering: firstly, the numbers should unambiguously tell the ordering of releases within a given series, secondly, they should indicate the degree and nature of the changes in each release.

## Release Number Components

Release numbers are groups of digits separated by dots:   

SoftwareName 1.1 

SoftwareName 2.1.4

...and so on. The dots are separators of each single number, not representing decimal numbers. There is no limit to the number of components, but most projects do not go beyond three or four. 

In addition to the numeric components, sometime the descriptive label such as "Alpha" or "Beta" will be used, for example:

SoftwareName 1.1.0 \(Alpha\) 

SoftwareName 2.1.4 \(Beta\)

An Alpha or Beta qualifier means that the future release will have the same number components without the qualifier. Thus, "1.1.0 \(Alpha\)" will eventually become "1.1.0". In order to use the qualifiers in a row, the qualifiers themselves can have meta-qualifiers. For example:

SoftwareName 2.1.0 \(Alpha 1\)

SoftwareName 2.1.0 \(Alpha 2\)

SoftwareName 2.1.0 \(Beta 1\) 

SoftwareName 2.1.0 \(Beta 2\) 

Notice that when it has the qualifier, number components "2.1" is written as "2.1.0". They are equivalent. You can drop all trailing zeroes for brevity. But if your are using a qualifier, one might as well go for completeness instead. Other qualifiers includes "Stable", "Unstable", "Development", and "RC" \("Release Candidate"\). The most widely used ones are "Alpha" and "Beta" and "RC", but you should always include a numeric meta-qualifier when using "RC". That is, you don't release "SoftwareName 2.1.0 \(RC\)", you release "SoftwareName 2.1.0 \(RC 1\)", followed by RC2, etc.

Although the dots in release numbers are not decimal points, they do indicate place-value significance. All "0.X.Y" releases precede "1.0". "3.14.158" immediately precedes "3.14.159", and non-immediately precedes "3.14.160".

A consistent release numbering policy enables a user tell the difference of the two releases of the same piece of software by just looking at the release numbers. In a typical three-component system, the first component is the major number, the second is the minor number, and the third is the micro number \("patch" number\). For example, release "2.2.1" is the second micro release \(or patch release\) in the third minor release line within the second major release series .A major series is simply all the releases that share the same major number, and a minor series is all the releases that share the same minor and major number. That is, "2.1.0" and "3.1.1" are not in the same minor series, even though they both have "1" for their minor number; on the other hand, "2.1.0" and "2.1.2" are in the same minor line, though they are not adjacent if "2.1.1" was released between them. An increment of the major number indicates that major changes happened; an increment of the minor number indicates minor changes; and an increment of the micro number indicates really trivial changes. Some projects add a fourth component, usually called the patch number, for especially fine-grained control over the differences between their releases. There are also projects that use the last component as a build number, incremented every time the software is built and representing no change other than that build. This helps the project link every bug report with a specific build, and is probably most useful when binary packages are the default method of distribution.

Although there are many different conventions for how many components to use, and what the components mean, the differences tend to be minor. The next two sections discuss some of the most widely used conventions.

## Semantic Versioning

Most projects have rules about what kinds of changes are allowed into a release when incrementing the micro number, and different rules when incrementing minor number, and still different rules when incrementing the major number. This policy is now formalized as Semantic Versioning at[ http://semver.org/](http://semver.org/).

1. Changes to the micro number only must be both forward and backward compatible. The changes should be bug fixes only, or very small enhancements to existing features. New features should not be introduced in a micro release.
2. Changes to the minor number must be backward compatible, but not necessarily forward compatible. It's normal to introduce new features in a minor release, but usually not too many new features at once.
3. Changes to the major number mark compatibility boundaries. A new major release can be forward and backward incompatible. A major release is expected to have new features, and may even have entire new feature sets.

Remember that all these injunctions only apply to this particular three-component system. Your project could easily come up with a different three-component system, or even decide it doesn't need such fine granularity and use a two-component system instead. The important thing is to decide early, publish exactly what the components mean, and stick to it.

## The Even/Odd Strategy

Some projects use the parity of the minor number component to indicate the stability of the software: even means stable, odd means unstable. This applies only to the minor number, not the major or micro numbers. Increments in the micro number still indicate bug fixes \(no new features\), and increments in the major number still indicate big changes, new feature sets, etc.

The advantage of the even/odd system, which has been used by the Linux kernel project among others, is that it offers a way to release new functionality for testing without subjecting production users to potentially unstable code. People can see from the numbers that "2.4.21" is okay to install on their live web server, but that "2.5.1" should probably stay confined to home workstation experiments. The development team handles the bug reports that come in from the unstable \(odd-minor-numbered\) series, and when things start to settle down after some number of micro releases in that series, they increment the minor number \(thus making it even\), reset the micro number back to "0", and release a presumably stable package. 

This system preserves, or at least, does not conflict with, the compatibility guidelines given earlier. It simply overloads the minor number with some extra information. This forces the minor number to be incremented about twice as often as would otherwise be necessary, but there's no real harm in that. The even/odd system is probably best for projects that have very long release cycles, and which by their nature have a high proportion of conservative users who value stability above new features.

