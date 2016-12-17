# What is this repository?
This is a mirror of the *ssss* codebase written by B. Poettering. The
[original website](http://point-at-infinity.org/ssss/) has tarballs, but
no source control. This repository imports the five public releases from
the author's website into Git for convenience.

# Sources
The sources for this mirror are the author's [released tarballs][1]. To
my knowledge, there is no publicly-accessible source code repository for
this tool, and the source is only available from the tarballs
themselves.

# Authenticity
I have no ability to authenticate the source other than through the
SHA-1 hashes posted on the author's website. The hashes are listed as:

    ssss-0.5.tar.gz (SHA1: 3f8f5046c2c5c3a2cf1a93f0a9446681852b190e)
    ssss-0.4.tar.gz (SHA1: 462a4309fabc02abf6f3470c5223f0aea44e2a05)
    ssss-0.3.tar.gz (SHA1: 433590f2c132e0040b13d1c21a2bf55eead6929c)
    ssss-0.2.tar.gz (SHA1: bcfdf3212e461baaa5922193faa1aec2bfffbb9c)
    ssss-0.1.tar.gz (SHA1: 66f8fca5793034fc42032f70de7f9195e4bb4bcd)

The hashes were successfully compared to the tarballs before inclusion
in this repository, but I can make no personal claims about the validity
of the code beyond that.

While the mirrored code is not cryptographically signed, and is not
actively maintained, it *is* currently included in the packages
available for [Debian Jessie][2] and Sid, and the MD5 signatures for the
imported copy of ssss-0.5.tar.gz match those reported for Debian Jessie.

    $ md5sum ssss-0.5.tar.gz | fgrep 24227252aa195a146d09de1df10357a1
    24227252aa195a146d09de1df10357a1  ssss-0.5.tar.gz

This seems like reliable evidence that it is covered by the [Debian
security team][3], and is considered reliable by the current Debian
maintainer. Please use your own judgment.

# Getting Involved
I lack the C and cryptographic expertise to vet the source code myself.
It may work; it may not. It may be safe; it may not. I simply wanted to
preserve the code in a way that would allow others to maintain and
improve the code using a modern source control system.

To avoid remaining a legacy  project, this repository needs a number of
things. Please consider contributing as you're able.

1. Code auditing.
1. Security auditing.
1. Validation of the cryptographic implementation.
1. Improved documentation on how to *use* the software, ideally in an
   accessible wiki.

# Final Thoughts
I consider myself a steward for this project, rather than the author's
successor. I would very much like to see this project brought up to
date, or forked into a more modern implementation should that be
necessary. The issue that this code addresses is too important to
languish, and I sincerely hope that the right sort of people will choose
to get involved.

[1]: http://point-at-infinity.org/ssss/
[2]: https://packages.debian.org/source/jessie/ssss
[3]: https://www.debian.org/security/
