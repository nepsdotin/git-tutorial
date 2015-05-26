# Installation Instructions

## Installation on Windows

[http://git-scm.com/download/win](http://git-scm.com/download/win)
## Installation on Linux

Depending on the linux flavours you are using you can follow as below

If you want to install Git on Linux via a binary installer, you can generally do so through the basic package-management tool that comes with your distribution. If you’re on Fedora for example, you can use yum:

**For Fedora / CentOS :**

```
$ sudo yum install git
```

**For Debian / Ubuntu :**

```
$ sudo apt-get install git
```

For more options, there are instructions for installing on several different Unix flavors on the Git website, at [](http://git-scm.com/download/linux) .

## Installation on Mac

### Using GIT Installer
There are several ways to install Git on a Mac. The easiest is probably to install the Xcode Command Line Tools. On Mavericks (10.9) or above you can do this simply by trying to run git from the Terminal the very first time. If you don’t have it installed already, it will prompt you to install it.

If you want a more up to date version, you can also install it via a binary installer. An OSX Git installer is maintained and available for download at the Git website, at [http://git-scm.com/download/mac](http://git-scm.com/download/mac).

### Using Homebrew 

https://kj-prince.com/blog/install-git-mac-osx-homebrew/

## To Check Installation

```
$ git --version
git version 1.7.12.4
```

## One Time Setup
```
git config user.name <name>
git config --global user.email <email>

git config --global user.name "Napoleon Arouldas"
git config --global user.email crew@putforshare.com

#To Setup an Editor for giving your commit message
git config --system core.editor <editor>

# To Edit your config file
git config --global --edit
```

# To list all the config info
```
git config --list
```

## Optional To Create SSH Keys
[https://help.github.com/articles/generating-ssh-keys](https://help.github.com/articles/generating-ssh-keys)

[https://help.github.com/ssh-issues/](https://help.github.com/ssh-issues/)

Git stores configuration options in three separate files, which lets you scope options to individual repositories, users, or the entire system:

    <repo>/.git/config – Repository-specific settings.
    ~/.gitconfig – User-specific settings. This is where options set with the --global flag are stored.
    $(prefix)/etc/gitconfig – System-wide settings. 

When options in these files conflict, local settings override user settings, which override system-wide. If you open any of these files, you’ll see something like the following:

```
[user] 
name = John Smith
email = john@example.com
[alias]
st = status
co = checkout
br = branch
up = rebase
ci = commit
[core]
editor = vim
```
