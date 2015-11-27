# Exercise 1.1
### Try This
Start a new git repository for an existing code base


```
$ cd /path/to/my/codebase
$ git init
```
# Exercise 1.2
### Linux users can Try This
```
$ ls -lA
```
##### Note:
You should find a ** .git ** directory inside the repo folder that you just created.

# Exercise 1.3
### Try This in a different folder
```
$ cd /path/to/different/folder
$ ls -lA
$ git log
fatal: bad default revision 'HEAD'

```
##### Note:
You can't find a **.git** directory inside the repo folder that you just created because you have not initialised the repository.

# Exercise 1.4
### Try This

#### $ git status
```
# On branch master
#
# Initial commit
#
nothing to commit (create/copy files and use "git add" to track)
```

Create index.md and add some text.
#### $ git status
```
# On branch master
#
# Initial commit
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#   index.md
nothing added to commit but untracked files present (use "git add" to track)
```







