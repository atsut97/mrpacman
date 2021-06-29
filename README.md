# Mr. Pacman

Rudimentary and simple package manager utility for my personal use.

## Description

`mrpacman` is a Bash script to manage packages that is locally
installed on the system for my personal use. I believe packages should
basically be managed by the default package manager on the system, but
I sometimes need to keep a program or library the latest version. In
such a case, however, updating programs and libraries to the latest at
all times is very bothersome and annoying. This script manages
packages installed on the system and collects instructios how to
install and update software, so it makes it easy to keep them up with
the latest.

## Examples

``` shell
pacman -Ss tmux
```
Search for regexp "tmux" in package database.

``` shell
pacman -S emacs
```
Download and install emacs including dependencies.

``` shell
pacman -Syu
```
Update package list and upgrade all packages afterwards.

``` shell
pacman -Syu emacs
```
Update package list, upgrade all packages, and then install emacs if it wasn’t already installed.
