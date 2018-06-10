# Open Water Foundation / Learn Cygwin #

This documentation provides resources to learn how to to use the free and open source Cygwin Linux-like environment on Windows.
Cygwin is useful because it allows Linux programs to be run on a Windows computer without installing an entirely separate virtual machine.
In particular, Cygwin allows shell scripts to be run, which helps automate common tasks.
The advantage of using Cygwin is that someone familiar with Linux can be effective on Cygwin similar to Linux,
and programs can transfer between Cygwin and Linux.
Alternatives to Cygwin:

* [Windows/DOS batch file](https://en.wikipedia.org/wiki/Batch_file) - runs in Windows/DOS command shell, limited functionality and portability 
* [Windows PowerShell](https://en.wikipedia.org/wiki/PowerShell) - often used for Windows system administration and automation
* [Windows Subsystem for Linux](https://msdn.microsoft.com/en-us/commandline/wsl/about) - useful for development but has limitations
* a scripting language such as Python (requires installing the language interpreter and requires knowing the language)

One or more of the above options may be used on the same computer.
However; Cygwin provides extensive software options that may be more straightforward.
In some cases, a decision must be made as to where to install a software program.
For example, should Python be installed and run on Windows, Linux, Cygwin, or multiple environments?

This documentation has been written based on experience using Cygwin at the Open Water Foundation.
The remainder of this page includes the following sections:

* [About the Open Water Foundation](#about-the-open-water-foundation) - author and maintainer of this documentation
* [How to Use this Documentation](#how-to-use-this-documentation) - overview of main sections
* [License](#license)
* [Source Repository on GitHub](#source-repository-on-github)

-----------

## About the Open Water Foundation ##

The [Open Water Foundation](http://openwaterfoundation.org) is a 501(c)3 nonprofit social enterprise that focuses
on developing and supporting open source software for water resources, so that organizations can make better decisions about water.
OWF has created this documentation to educate its staff, collaborators, and clients that work with spatial data.

See also other [OWF learning resources](http://learn.openwaterfoundation.org).

## How to Use this Documentation ##

The documentation is organized in order of information and tasks necessary to install/update, configure, and use Cygwin.

This documentation is not intended to be a full reference for Cygwin but focuses on important topics that
will help understand technical concepts and be successful using Cygwin.
The following main sections are included in this documentation:

* [Install Cygwin](install/install) - explanation of how to install Cygwin
* [User Environment](user-env/user-env) - information about a user's home folder and environment
* [Cygwin/Windows Integration](cygwin-windows/cygwin-windows) - information about Cygwin and Windows are integrated
* [Using Cygwin Command Line](using-cygwin-cl/using-cygwin-cl) - using the Cygwin command line terminal shell
* [Using Cygwin X Windows](using-cygwin-xwin/using-cygwin-xwin) - using the Cygwin command line terminal shell
* [Cygwin Development Environment](cygwin-dev-env/cygwin-dev-env) - topics related to software development
* [Troubleshooting](troubleshooting/troubleshooting) - troubleshooting help
* [Resources](resources/resources) - useful resources

Use the menu on the left to navigate to pages within the documentation.
Use the menu on the right to navigate to sections within a page.
Menus may be compressed into an icon if the page size is small, such as on a mobile device.

## License ##

The OWF Learn Cygwin website content and examples are licensed under the
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0).

## Source Repository on GitHub ##

The source files for this documentation are maintained in a GitHub repository:  [owf-learn-cygwin](https://github.com/OpenWaterFoundation/owf-learn-cygwin).

## Release Notes ##

See the [Release Notes in the GitHub Project](https://github.com/OpenWaterFoundation/owf-learn-cygwin#release-notes).
