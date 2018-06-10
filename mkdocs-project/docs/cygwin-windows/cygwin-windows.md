# Learn Cygwin / Cygwin / Windows Integration #

Cygwin software is compiled to run on Windows and Windows programs can also be run from within Cygwin.
Some basic conventions are implemented to allow this integration.

* Cygwin recognizes Windows drive letters.  To access the C drive, use the path `/cygdrive/C`.
* The `PATH` environment variable, which is used to find executable programs, is
initialized to the Windows `PATH` but using `/cygdrive` in front of drive letters.

**Need to expand this section.**
