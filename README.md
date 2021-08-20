# Mr. Pac-Man

Rudimentary and simple package manager utility for my personal use.

I have got an idea of the name from PAC-MAN™, ©1980 BANDAI NAMCO
Entertainment Inc.

## Description

Mr. Pac-Man, or `mrpacman`, is acronyms for "My Rudimentary PACkage
MANager" and yet "ManageR of PACkage MANager". It is a Bash script to
manage packages and modules that are installed locally on the system
for my personal use. I believe packages should basically be managed by
the default package manager on the system, but I need keep some
programs and libraries the latest versions that are not available in
the repository of the default package manager. For those packages, I
have to delegate management of them to alternative package/module
managers such as `pip`, `go modules`, `yarn`, `cabal` and `cargo`, or
I cannot help but manage and install them manually. In such cases
updating them to the latest at all times by hand is very bothersome
and annoying. This script manages packages installed manually on the
system, collects instructions how to install and update packages and
executes commands of delegated package managers so that it makes it
easy to keep up packages on the system to the latest.

## Examples

``` shell
mrpacman -Ss tmux
```
Search for regexp "tmux" in package database.

``` shell
mrpacman -S emacs
```
Download and install `emacs` including dependencies.

``` shell
mrpacman -Syu
```
Update package list and upgrade all packages afterwards.

``` shell
mrpacman -Syu emacs
```
Update package list, upgrade all packages, and then install `emacs` if
it wasn’t already installed.
