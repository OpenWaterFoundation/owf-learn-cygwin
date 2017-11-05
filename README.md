# owf-learn-cygwin #

This repository contains the [Open Water Foundation (OWF)](http://openwaterfoundation.org/) Cygwin training materials,
which provides guidance for using the Cygwin software, which is essentially a Linux-like environment running on Windows .
The documentation is written for the layperson in order to encourage use of GeoJSON.

See the deployed [OWF / Learn GeoJSON](http://learn.openwaterfoundation.org/owf-learn-cygwin/) documentation.

## Repository Contents ##

The repository contains the following:

```text
.github/              (Files specific to GitHub such as issue template)
.gitattributes        (Typical Git configuration file)
.github/              (GitHub-specific files such as issues template)
.gitignore            (Typical Git configuration file)
README.md             (This file)
build-util/           (Useful scripts to view, build, and deploy documentation)
mkdocs-project/       (Typical MkDocs project for this documentation)
  mkdocs.yml          (MkDocs configuration file for website)
  docs/               (Folder containing source Markdown and other files for website)
  site/               (Folder created by MkDocs containing the static website - ignored using .gitignore)

```

## Development Environment ##

The development environment for contributing to this project requires installation of Python, MkDocs, and Material MkDocs theme.
Python 2 on Cygwin has been used for development.  See the [OWF / Learn MkDocs](http://learn.openwaterfoundation.org/owf-learn-mkdocs/)
documentation for more information about MkDocs.

## Editing and Viewing Content ##

If the development environment is properly configured, edit and view content as follows:

1. Edit content in the `mkdocs-project/docs` folder and update `mkdocs-project/mkdocs.yml` as appropriate.
2. Run the `build-util/run-mkdocs-serve-8000.sh` script (Linux) or equivalent to start the Python web server.
3. View content in a web browser using URL `http://localhost:8000`.
4. Any files changes that are saved will cause the browser to refresh files.

## License ##

The OWF Learn GeoJSON website content and examples are licensed under the
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0).

## Contributing ##

Contribute to the documentation as follows:

1. Use GitHub repository issues to report minor issues.
2. Use GitHub pull requests.

## Maintainers ##

This repository is maintained by the [Open Water Foundation](http://openwaterfoundation.org/).

## Contributors ##

Steve Malers, Open Water Foundation (@smalers)

## Release Notes ##

The following release notes indicate the update history for documentation, with GitHub repository issue indicated,
if applicable (links to issues via README.md are not cleanly supported by GitHub so use the repository issues page to find).

* 2017-11-04 - initial version.
