---
layout: home
title: "Undoing and Reverting"
---

Undoing and Reverting
---------------
{: .-three-column}

##### ```git checkout``` to revert changes on a file
```
git checkout <commit> -- <file>  //pull file into working dir from amother commit 
git checkout <commit>^ -- <file>  //pull file into working dir from the previous commit (^) to the specified commit
git checkout <commit> path/to/file  //revert single file to previous commit
```

