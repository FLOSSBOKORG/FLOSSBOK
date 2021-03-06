# Packaging

The distribution form of free software is source code, no matter the software runs in source form or needs to be compiled first. With compiled software, most users will probably not compile the sources themselves, but will instead install from pre-built binary packages. However, those binary packages are still derived from a master source distribution. The point of the source package is to unambiguously define the release.   
There is a strict standard for how source releases should look.

## Format

The source code should be shipped in the standard formats for transporting directory trees. For Unix and  
 Unix-like operating systems, the convention is to use TAR format, compressed by compress, gzip, bzip   
or bzip2. For MS Windows, the standard method for distributing directory trees is zip format, which   
compresses automatically. For JavaScript projects, it is customary to ship the "minified" versions of the files together with the human-readable source files.

## Name and Layout

The name of the package should consist of the software's name plus the release number, the format suffixes appropriate for the archive type. For example, SoftwareName 2.1.0, packaged for Unix using GNU Zip \(gzip\) compression, would look like this:

softwarename-2.1.0.tar.gz

or for Windows using zip compression:

softwarename-2.1.0.zip

Either of these archives, when unpacked, should create a single new directory tree named softwarename-2.1.0 in the current directory. Under the new directory, the source code should be arranged in a layout ready for compilation and installation. In the top level of new directory tree, there should be an INSTALL file giving instructions on how to build and install the software for all the operating systems it supports. Also, there should be a plain text README file explaining what the software does and what release this is, and giving pointers to other resources, such as the project's web site, other files of interest, etc. There should also be a CHANGES file, explaining what's new in this release. The CHANGES file accumulates change lists for all releases, in reverse chronological order. There should also be a COPYING or LICENSE file, giving the software's terms of distribution.

### To Capitalize or Not to Capitalize

When referring to a project by name, people generally capitalize it, and capitalize acronyms if there is one: "MySQL 5.0", "Software 2.1.0", etc. Whether this capitalization is re- produced in the package name is up to the project. Either would be fine. The important thing is that the directory created by unpacking the tarball use the same capitalization.

### Pre-Releases

When shipping a pre-release, the qualifier is a part of the release number. So it should be included in the name. For example, the ordered sequence of alpha and beta releases would result in package names like this:

software-2.1.0-alpha1.tar.gz 

software-2.1.0-alpha2.tar.gz 

software-2.1.0-beta1.tar.gz 

software-2.1.0-beta2.tar.gz 

software-2.1.0-beta3.tar.gz 

software-2.1.0.tar.gz

The first would unpack into a directory named software-2.1.0-alpha1, the second into software-2.1.0-alpha2, and so on.



















