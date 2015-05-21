# Lets Get Started

## init , add, commit

### The lifecycle of the status of your files.
![](img/lifecycle.png)

```
$ git init
```
Create an ** empty ** git repository or ** reinitialize ** an existing one

An initial HEAD file that references the HEAD of the master branch is also created.

Running git init in an existing repository is safe. It will not overwrite things that are already there.

### To Create A Bare Repository
Bare Repository is a Repository with no working directories, mostly they are remote repos.

```
$ git init --bare
```

basically a .git directory with subdirectories for objects, refs/heads, refs/tags. 

## add

Add file contents to the index

### To Understand

1.  git added index.md to the snapshot for the next commit.
2.  A snapshot represents the state of **your project** at a given point in time.
3.  git doesnt treats content changes to a file rather to file changes to a project.
4.  Git’s term for creating a snapshot is called **staging**.

### Two Step Process

1.  **Staging:** Telling Git what files to include in the next commit.
2.  **Committing:** Recording the staged snapshot with a descriptive message.


## commit
```
git commit
```

Record changes to the repository

```
git commit
git commit -m "<message>"

# Shortcut to tell git to stage all the changes for files that are already added, and commit. 

## Note:
New files should be separately added.

# It does not add any new files.
git commit -a
git commit --all
```

### --amend

```
$ git commit --amend -m 'message'
```
Adds new commit message with the previous staged content.

### commitID
```
commit 3157ee3718e180a9476bf2e5cab8e3f1e78a73b7
Author: John Smith
```

## clone

Clone a repository into a new directory

```
$ git clone <repo>
$ git clone <repo> [folder-where-to-clone]
```

## Git URLs
1.  ssh://[user@]host.xz[:port]/path/to/repo.git/
2.  git://host.xz[:port]/path/to/repo.git/
3.  http[s]://host.xz[:port]/path/to/repo.git/
4.  ftp[s]://host.xz[:port]/path/to/repo.git/
5.  rsync://host.xz/path/to/repo.git/

An alternative scp-like syntax may also be used with the ssh protocol:

[user@]host.xz:path/to/repo.git/

The ssh and git protocols additionally support ~username expansion:

ssh://[user@]host.xz[:port]/~[user]/path/to/repo.git/

git://host.xz[:port]/~[user]/path/to/repo.git/

[user@]host.xz:/~[user]/path/to/repo.git/

For local repositories, also supported by git natively, the following syntaxes may be used:

/path/to/repo.git/

file:///path/to/repo.git/
```

###### Note:
Sometimes You need to use sudo with all the commands