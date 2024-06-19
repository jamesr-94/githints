---
layout: home
title: "Getting started"
---


Getting started
---------------
{: .-three-column}

##### Create a git repo in current directory
```git init <repoName>```

##### Clone a git repo from url
```git clone <url> <name>```

##### fetches code from the remote repository, without merging
```git fetch origin <branch>```


##### fetches code from remote and merges changes with local
```
git pull 
git pull origin <branch> 
```
##### create a new branch off the current state
```
git branch <branch>
git checkout -b <branch> //create a new branch and check it out
```

Preparing Commits
---------------
{: .-three-column}

##### ```git diff``` to see what has changed
```
git diff //shows changed files that havent been staged
git diff --staged  //shows changed files that have been staged
```
##### ```git add```
```
git add --all //stage all changes including modifications, deletions
git add . // (git 1.x)stage all new files + modifications
git add --ignore-removal . // (git 2.x)stage all new files + modifications
git add -update //stage modifications + deletions
```
##### ```git rm``` to remove files 
```
git rm <file>  //removes file and stages the removal
git rm --cached <file>  //removes file from staging area without removing from disk
```
##### ```git mv```
```
git mv <source> <target> //move (or rename) a file and have the modification tracked (equivalent to git rm + git add)
```

Committing and pushing changes
---------------
{: .-three-column}

##### ```git commit```
```
git commit -m "commit message here" //commit staged files with message
git commit -a -m "commit message here" //automatically stage files and commit with message
git commit --amend  //revise the most recent commit message that hasnt yet been pushed
```
##### ```git push```
```
git push origin HEAD //push to current branch
```


Undoing and Reverting
---------------
{: .-three-column}

##### ```git checkout``` to revert changes on a file
```
git checkout <commit> -- <file>  //pull file into working dir from amother commit 
git checkout <commit>^ -- <file>  //pull file into working dir from the previous commit (^) to the specified commit
git checkout <commit> path/to/file  //revert single file to previous commit
```
