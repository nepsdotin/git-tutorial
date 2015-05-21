# Exercise on Checkout

### Do This 

```
$ cd /path/newrepo
$ git init 

# Add some content to index.md
$ vi index.md 

$ git add index.md
$ git commit -m 'Added first rev of index.md'

# Add some content to readme.md
$ vi readme.md

$ git add readme.md
$ git commit -m 'Added first rev of readme.md'

# Add some content to index.md, readme.md

$ git add .
$ git commit -m 'Add some changes to both index.md, readme.md'

# Add some content to readme.md
$ git add .
$ git commit 'Complete content added to readme.md'
```

### Try This Exercise 1
```
$ git checkout master
Already on 'master'
```

### Try This Exercise 2
```
$ git log --oneline

97edb3b Complete content added to readme.md
2023bde Add some changes to both index.md, readme.md
49de400 Added first rev of readme.md
6cc0648 Added first rev of index.md

$ git checkout 49de400
```

### Try This Exercise 3

```
$ git checkout master
$ git checkout 2023bde index.md
# ** Something interesting happens ** only index.md is checkedout.
``` 

# Exercise on Reset

### basic stuff
```
$ cd to/new/path
$ git init

# Add some content
$ vi index.md

$ git status
# On branch master
#
# Initial commit
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#   index.md
nothing added to commit but untracked files present (use "git add" to track)


$ git add index.md
# On branch master
#
# Initial commit
#
# Changes to be committed:
#   (use "git rm --cached <file>..." to unstage)
#
#   new file:   index.md
#

$ git commit -m 'First commit on index.md'

$ git log --oneline
94647dd First commit of Git doc

$ git status
# On branch master
nothing to commit (working directory clean)

# Add some stuff
$ vi index.md

$ git status
# On branch master
# Changes not staged for commit:
#   (use "git add <file>..." to update what will be committed)
#   (use "git checkout -- <file>..." to discard changes in working directory)
#
#   modified:   index.md
#
no changes added to commit (use "git add" and/or "git commit -a")
```

### Removing content from staging area
```
$ git add index.md
$ git reset 
Unstaged changes after reset:
M   index.md
```

### Removing content from staging area and working area
```
# watch the index.md in your work tree
$ git reset --hard
HEAD is now at 94647dd First commit of Git doc

# can repeat this with multiple snapshots and commits
```
