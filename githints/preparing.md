---
layout: home
title: "Preparing Commits"
---

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