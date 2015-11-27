# Uniqueness 

## Distributed
Every developer has his own repository. His repository would be used to put in files and take out the files from the repo.

and If he wants to share his code with others he can do that as well, **without disturbing others work**

## Contents Verified using SHA1 algorithm.
Everytime Git Commits your file it uses the file content and generates a Hash for it and stores that hash as well.

And everytime you take out the file from the repository it takes the content and verifies with the hash with the one it stored and if it finds they are not same then it reports.

This makes it very robost if your remote repo is hacked by someone, You will get to know about that.

## Tracks complete list of files in a project as one content than individuals.

Aside from the practical distinctions between SVN and Git, their underlying implementation also follow entirely divergent design philosophies. Whereas SVN tracks differences of a file, Git’s version control model is based on snapshots. For example, an SVN commit consists of a diff compared to the original file added to the repository. Git, on the other hand, records the entire contents of each file in every commit.

## Lightweight Branching & Easy Merging ( ~ 5 merges can be done in a day).


