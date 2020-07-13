# Welcome to [`@itsN1X`](https://google.com/search?q=itsN1X)/[`8696_libreotp`](https://github.com/itsN1X/8696_libreotp)
This repository was updated to [`itsN1X`](https://github.com/itsN1X)/`8696_libreotp` with `bindle`/`libre_otp`/tree/[`pu`](https://github.com/bindle/libreotp/tree/pu) on day 8696.  
##### Feel free to make any contributions. Keep your commits atomic and neatly commented.  
One may `checkout` the latest branch at `master` itself. Please read this entire document first.

----

### Additional resources:


- [Encode/decode OTP data using TCP/UDP.](port-seq-enc.sh)

- [Extension/examples of translations.](port-seq.sh)

- [RFC-2104 documentation.](rfc2104.txt)

- [RFC-3602 documentation.](rfc3602.txt)

- [RFC-4226 documentation.](rfc4226.txt)

- [RFC-6238 documentation.](rfc6238.txt)

- [Format for TOTP secret](secret.txt)



----

## Legacy `README`

```
LibreOTP
=====================

   The goal of LibreOTP is to provide a portable suite of tools and libraries
   which implements Time-based One-time Password Algorithm (TOTP) and HMAC-based
   One-time Password Algorithm (HOTP) in a package which does not have
   external crypto dependencies.


Contents
--------

   1. Disclaimer
   2. Maintainers
   3. Source Code
   4. Package Maintence Notes


Disclaimer
==========

   This software is provided by the copyright holders and contributors "as
   is" and any express or implied warranties, including, but not limited to,
   the implied warranties of merchantability and fitness for a particular
   purpose are disclaimed. In no event shall Bindle Binaries be liable for
   any direct, indirect, incidental, special, exemplary, or consequential
   damages (including, but not limited to, procurement of substitute goods or
   services; loss of use, data, or profits; or business interruption) however
   caused and on any theory of liability, whether in contract, strict
   liability, or tort (including negligence or otherwise) arising in any way
   out of the use of this software, even if advised of the possibility of
   such damage.


Maintainers
===========

   David M. Syzdek
   Bindle Binaries
   syzdek@bindlebinaries.com


Source Code
===========

   The source code for this project is maintained using git
   (http://git-scm.com).  The following contains information to checkout the
   source code from the git repository.

   Browse Source:

      https://github.com/bindle/libreotp

   Git URLs:

      git://github.com/bindle/libreotp.git
      https://github.com/bindle/bindleadmin.git
      git@github.com:bindle/bindleadmin.git

   Downloading Source:

      $ git clone git://github.com/bindle/libreotp.git

   Preparing Source:

      $ cd libreotp
      $ ./autogen.sh

   Git Branches:

      master - Current release of packages.
      next   - changes staged for next release
      pu     - proposed updates for next release
      xx/yy+ - branch for testing new changes before merging to 'pu' branch


Package Maintence Notes
=======================

   This is a collection of notes for developers to use when maintaining this
   package.

   New Release Checklist:

      - Switch to 'master' branch in Git repository.
      - Update version in configure.ac.
      - Update date and version in ChangeLog.
      - Commit configure.ac and ChangeLog changes to repository.
      - Create tag in git repository:
           $ git tag -s v${MAJOR}.${MINOR}
      - Push repository to publishing server:
           $ git push --tags origin master:master next:next pu:pu

   Creating Source Distribution Archives:

      $ ./configure
      $ make update
      $ make distcheck
      $ make dist-bzip2

```
