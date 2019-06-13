# Opspack - Package Manager For Bug Bounty/Offensive.

[![undefined](https://img.shields.io/github/release/BugHunterID/opspack.svg)](https://github.com/BugHunterID/opspack/releases/latest)
[![undefined](https://img.shields.io/github/last-commit/BugHunterID/opspack.svg)](https://github.com/BugHunterID/opspack)
[![undefined](https://img.shields.io/github/languages/top/BugHunterID/opspack.svg)](https://github.com/BugHunterID/opspack)
[![undefined](https://img.shields.io/github/commits-since/BugHunterID/opspack/latest.svg)](https://github.com/BugHunterID/opspack/tags)

Opspack `(Open Source Security Package)` is a simple package manager for bug bounty/offensive. Using command line interface that can be used to install,update and upgrade tools easily with lots of open source repositories on Github.


## Contributing with us

Contributing with us making a correction or adding a tool. 

##### Contribute through adding tools 

1. Make a folder and file: `opspack/opspackage/installer/{package name}/{package name}.ops`
2. Fill in file {packagename}.ops

```
#!/bin/bash -e

. script/opsFunction

PACKNAME="MyPackageName"            ## Package Name
REPO="MyUserGithub"                 ## Username Github
VERSION="2.2"                       ## Version
PACKDES="Mypackage Is bla bla bla"  ## Description
TAG="Scanner"                       ## Tag : scanner
PACKDEP="xterm"

TARBALL="${REPO}/${PACKNAME}/archive/${VERSION}.tar.gz" ## Don't modify
downloadsource "http://github.com/${TARBALL}" PPA ## Don't modify
echo " complete" ## Don't modify
```
3. Make a push request. or You can add by using the [issue page](https://github.com/BugHunterID/opspack/issues/new) with format : 

```
Title         : [Tools] name tools
Description   : 

Github Link : https://github.com/BugHunterID/opspack
Required    : Example PHP CURL / PHP >= 7

```

## Disclaimer

This is an open source for everyone, you may redistribute, modify, use patents and use privately without any obligation to redistribute. but it should be noted to include the source code of the library that was modified (not the source code of the entire program), include the license, include the original copyright of the author (radenvodka), and include any changes made (if modified). Users do not have the right to sue the creator when there is damage to the software or even demand if there is a problem caused by the makers of this tool. because every risk is caused by the user risk itself.


License : [![GPLv3 license](https://img.shields.io/badge/License-GPLv3-blue.svg)](http://perso.crans.org/besson/LICENSE.html)

***GPL v3.0 specifically designed to allow users to use software distributed through networks such as websites and online services***
