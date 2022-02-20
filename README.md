# Azratek Package Archive
## What is the Azratek Package Archive format?
The Azratek Package Archive format is a software package archive format.

It is basically a `tar` archive compressed with `gzip` (Please read the
[Package Specification](https://github.com/azratektechnologies/azratek-package-archive/blob/main/docs/PACKAGE-SPECIFICATION)).
## Creating an Azratek Package Archive
1. Create a directory containing the package's files.
2. Create a `PACKAGE` file (template is available at
[templates/PACKAGE](https://github.com/azratektechnologies/azratek-package-archive/blob/main/templates/PACKAGE)).
3. Create a `DEPENDENCIES` file containing the package's dependencies.
4. Create an `INSTALL` file containing the install script.
5. Create an `UNINSTALL` file containing the unintall script.
6. Create a directory named after the package's name, e.g. package name is `example`, the directory must be `/example` containing the installable files.
7. Create a `docs` directory containing the package's documentation.
8. Create the package using `apr-make` (available in [apr-utils](https://github.com/azratektechnologies/apr-utils)).
