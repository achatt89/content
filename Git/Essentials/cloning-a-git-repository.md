# Cloning a Git repository
author: catalin

levels:

  - beginner

type: normal

inAlgoPool: false

category: must-know

links:

  - >-
    [www.atlassian.com](https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-clone){website}

---
## Content

The second way though which you can get your hand on a **Git** repository is by *cloning* it.

The term **cloning** entails how the whole **Git** flow works. Instead of providing a working copy, the `git clone` command makes a full copy of the *repository*, including all project history.

In case of server failure, corruption or other unfortunate events, any clone can be used to restore the state of the project.

The syntax used to clone a repository is:
```
$ git clone [url]
```

You can clone any open-source project or even private ones as long as you have the right credentials. For example, you can clone the `reduck` library from its specific url:
```
$ git clone 
    https://github.com/enkidevs/reduck
```

Running this command will: 
 - create a directory named "reduck"
 - initialise a `.git` directory inside
 - pull all repository data in the `.git` directory
 -  check out a working copy of the latest version of the project

Another name for the parent directory can be specified as follows:
```
$ git clone https://github.com/enki/repo \
                            myAwesomeClone
```

Apart from through the `https://` protocol used above, **Git** also supports transfer through **SSH** and local protocols.

---
## Practice

What's the last step **Git** automatically does after running `git clone`?

???

* checks out a working copy of the latest version of the project
* initialises the `.git` directory
* pulls repository data in the `.git` directory
* create a new folder directory

---
## Revision

Does running `git clone` with a repository's url require having an existing working copy on you machine?

???

*No
*Yes
*Only if you don't provide a new new directory name