#Inspecting a Repository with status, log

## Status

```
$ git status
```
List which files are staged, unstaged, and untracked.
```

# Not currently on any branch.
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#   modified:   index.md
#   deleted:    intro.md
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#   history.md
#   intro.md
```

## .gitignore files
config file used to ignore machine generated binaries.

### Placed at one of the places
```
1.  Just go and add files ( pattern ) to be excluded with one pattern per line .git/info/exclude

2.  .gitignore at the root folder of the project

```

### Very useful command if you have already commited the entire directory.
```
$ git rm --cached <path>
$ git rm --cached app/runtime/application.log
```

#### Lots of useful gitignore templates

[https://github.com/github/gitignore/](https://github.com/github/gitignore/)

## log

![](img/log.svg)

Display the entire commit history using the default formatting. If the output takes up more than one screen, you can use Space to scroll and q to exit.


```
$ git log -n <limit>
```
Limit the number of commits by <limit>. For example, git log -n 3 will display only 3 commits.


```
$ git log --oneline
```
Condense each commit to a single line. This is useful for getting a high-level overview of the project history.


```
git log --stat
```
Along with the ordinary git log information, include which files were altered and the relative number of lines that were added or deleted from each of them.


```
git log -p
```
Display the patch representing each commit. This shows the full diff of each commit, which is the most detailed view you can have of your project history.


```
git log --author="<pattern>"
```
Search for commits by a particular author. The <pattern> argument can be a plain string or a regular expression.


```
git log <since>..<until>
```
Show only commits that occur between <since> and <until>. Both arguments can be either a commit ID, a branch name, HEAD, or any other kind of revision reference.


```
git log --graph --decorate --oneline
```