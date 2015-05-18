# Exercise on Status, log, gitignore

# gitignore

### Using .git/info/excludes file

```
cd dir-your-choice
$ git init

#create a .js file in your editor

$ git status

# On branch master
#
# Initial commit
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#   app.js
nothing added to commit but untracked files present (use "git add" to track)

#edit .git/info/exclude

add js/*.js
add bin/*

$ git status 

# On branch master
#
# Initial commit
#
nothing to commit (create/copy files and use "git add" to track)


# You can see git has ignored .js file
```
### Using .gitignore file

### Repeat the previous exercise with ignoring .css files 

```
#create a .js file in your editor

$ git status

# On branch master
#
# Initial commit
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#   default.css
nothing added to commit but untracked files present (use "git add" to track)

#edit .gitignore

js/*.js
css/*.css
bin/*

$ git status 

# On branch master
#
# Initial commit
#
nothing to commit (create/copy files and use "git add" to track)
```

### Using git rm --cached <path>

```
### Add some stuff to default.css

$ git status
$ git rm --cached default.css

$ git status

# Not currently on any branch.
nothing to commit (working directory clean)
```


