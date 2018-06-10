# Learn Cygwin / Cygwin Development Environment #

The Cygwin user environment provides a convenient environment for performing computing tasks,
including software development and process automation.  See the [Using Cygwin Command Line](../using-cygwin-cl/using-cygwin-cl) section
for information about starting a command line terminal window.
The following topics are relevant to using Cygwin for software development.

* [Line Endings](#line-endings)
* [File Permissions](#file-permissions)
* [Git Version Control](#git-version-control)

---------

## Line Endings ##

Because Cygwin is POSIX compliant Linux implementation, text file line endings are newlines (`\n` or `LF`).
This can cause issues because files created by Windows programs use carriage return and newline (`\r\n` or `CRLF`).
These characters can be displayed by some text editors but are otherwise typically handled by the operating system and software.

A common situation is that the Cygwin Bash shell will not run a script with Windows line endings.
If necessary, the `dos2unix` program can be run to convert a file to Linux line endings.

See also the [Git](#git-version-control) discussion below.

## File Permissions ##

File permissions can be unexpected for Cygwin.
For example, a program such as [Gimp](https://www.gimp.org/) may create image files that are saved in repository working files.
These files should have normal permissions but may be shown as executable by Cygwin.
This issue is particularly irritating when working with version control systems such as Git,
which may recognize a file permissions (file mode) change as a version change.

This issue may also occur if files are checked out of a Git repository by Windows client
such as Git for Windows, and then further managed using Git on Cygwin.

**This issue is being evaluated by OWF staff.**

## Git Version Control ##

The Git version control system is often used to track versions of code and other files.
The Git client software can be downloaded and configured through normal Cygwin install process.
The following are issues that need to be considered when using Git on Cygwin:

* The Git software version on Cygwin may be older than that available from other downloads,
such as Git for Windows or Linux package managers.
This does not tend to be an issue other than when a major enhancement occurs.
* Because Cygwin's user files are separate from the Windows operating system,
configuring git using `git config` will save a separate set of configuration files than
Git for Windows and other tools.
Software developers just need to be aware of these issues.
For example, run the following (or equivalent) in each Git client to review configuration settings:  `git config --list`
* Mixing Git clients on the same development files, such as a Git-aware
integrated development environment (IDE) such as Eclipse, or text editor, can have issues.
For example, handling of file permissions and line endings may differ,
leading to changes being detected when the software developer did not actually change file content.
See other sections of this page for more information on core issues.
It is best to understand the tools being used by a software development team so that
incompatibilities can be addressed.
* A repository `.gitattributes` file with `* test=auto` can be used to minimize issues with line endings,
similar to how Linux and Windows interoperability is supported.
If files are checked out on Cygwin, the files can often be edited with Windows tools if such
tools gracefully handle line endings.
