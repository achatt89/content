# Tracking and Staging files
author: catalin

levels:

  - beginner

type: normal

inAlgoPool: false

category: must-know

links:

  - >-
    [git-scm.com](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository){website}

---
## Content

You can easily check the status of your files inside a **Git** project with the `git status` command:
```
$ git status
# On branch master
# Your branch is up-to-date with
# 'origin-master'.
# nothing to commit, working directory
# clean
```
The message in the code snippet above is shown when there are no *tracked* and *modified* files.

Let's suppose you add `enki.txt` to your project. Running the same command you will see a different result:
```bash
$ git status
# On branch develop
# You branch ...
# Untracked files:
#     enki.txt
# nothing added to commit ...
```
You can see that the `enki.txt` file is **untracked**. In order for **Git** to manage changes in this file (track it) you must use the `git add` command:
```
$ git add enki.txt
```
You can also add all the files in the current directory with the same command:
```
$ git add *
```

Running `git status` again, we can see that the file is now **staged** and ready to be part of a **commit**:
```
$ git status
# ...
# Changes to be committed:
#    new file:    enki.txt

```

---
## Practice

What's the command that will add all the files in the current directory to the staging area?
```
$ git ??? ???
```

*`add`
*`*`
*`--all`
*`stage`
*`commit`
*`status`
*`-a`

---
## Revision

What git command can be used to check what files are untracked, modified or staged?

```
$ git ???
``` 
*`status`
*`checkout`
*`stats`
*`add`
*`branch`
*`list`