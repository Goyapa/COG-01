# Git version control system

#### Git is a free and open source distributed version control system([VCS](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)).

### [TryGit](https://try.github.io): 
###### also have a look at [codeschool](https://www.codeschool.com/courses/try-git)

### [Version Control System(VCS)](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)
### [Getting Started - Git Basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)

## Basic Git commands
Command                                                         |   Explanation
-------                                                         |   ------------
$ git init                                                      |   Initial Step: Creates a new local repository (Repositorium, Aufbewahrungsort), move to Step 1 or Step 4.
|||
$ git status                                                    |   Step 1: shows git's actual status: Changes, untracked files etc.
|||
$ git add [filename]                                            |   Step 2: add changes to INDEX(Liste) as a general rule
$ git add myScript.js                                           |   add "myScript.js" to the INDEX also called the Stage
|||
$ git commit -m 'description'                                   |   Step 3: Commit (übergebe) changes as a general rule, repeat at Step 1 or move to Step 5.
$ git commit -m "Fix typo in introduction to user guide"        |   The description should give the reader a hint what was done. 
$ git commit                                                    |   [How to Write a Git Commit Message](http://chris.beams.io/posts/git-commit/)
|||
GitHub                                                          |   the following commands are more specific to remote repositories
$ git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY    |   Step 4:  Clone remote repository, move to Step 1.
$ git clone https://github.com/Goyapa/COG-01.git                |   sample
$ git remote -v                                                 |   List the current configured remote repository of your fork.
$ git push -u origin master                                     |   Step 5: Push changes to remote repository (your fork)
$ git push                                                      |   The -u tells Git to remember the parameters
$ git pull                                                      |   update local repository with remote changes (your fork)
|||
But syncing a fork e.g. from https://github.com/Goyapa/COG-01   |   https://help.github.com/articles/syncing-a-fork/
$ git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git | add remote upstream repository as a general rule
$ git remote add upstream https://github.com/Goyapa/COG-01      | Step 01: add original repository you forked from
$ git fetch upstream                                            | Step 02: sync changes of the original repository with your fork 
$ git checkout master                                           | Step 03: if you are not already in master
$ git merge upstream/master                                     | Step 04: merge changes (Änderungen zusammenfügen)
$ git push -u origin master                                     | Step 05: push changes from upstream to remote repository (your fork)
Tip: Syncing your fork only updates your local copy of the repository.  |   To update your fork on GitHub, you must push your changes.
$ git remote rm upstream                                        | if you want to remove the remote upstream
|||
Git Config                                                      |   Cloud9 is preconfigured, get and set configuration variables
$ git config --list                                             |   have a look
$ git config --global user.name "John Doe"                      |   set/change your user name
$ git config --global user.email johndoe@example.com            |   set/change your email
|||
$ git mv                                                            |   [git-mv](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository#Moving-Files) - Move or rename a file, a directory, or a symlink
$ git mv [previousFilename] [newFilename]                           |   rename file with git as a general rule
$ git mv mySuper.js myHero.js                                       |   rename "mySuper.js" to "myHero.js"          
$ git mv [xyzFolder/previousFolderName] [xyzFolder/newFolderName]   |   rename folder with git as a general rule
$ git mv commandline/Basic-cammands/ commandline/Basics-commands    |   rename folder from "Basic-cammands" to "Basics-commands"
|||
$ git diff                                                          |   [git-diff](https://git-scm.com/docs/git-diff) - Show changes between commits, commit and working tree, etc
$ git diff HEAD -- ./test                                           |   compare with the tip of the current branch, but limit the comparison to the file "test"



```
Via Twitter ;-)
Sebastian McKenzie @sebmck  Jan 16
I've started tracking how many hours I sleep by checking the time difference between my GitHub commits.
```

### [Git Project](https://git-scm.com/)

### [Git Documentation](https://git-scm.com/doc)

### [Online Book and Ebook](https://git-scm.com/book/en/v2)


## Git Branching: 
Branching means you diverge from the main(e.g. Master) line of development and continue to do work without messing with that main line.
Branches are used to develop features isolated from each other.

### [Git Branching - Branches in a Nutshell](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell)

### [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/)

### [Git branching model as pdf](http://nvie.com/files/Git-branching-model.pdf)

## GitHub:

### [GitHub Help](https://help.github.com/)

### [Collaborating on projects using pull requests](https://help.github.com/categories/collaborating-on-projects-using-pull-requests/)

## Git Cheat Sheets:

### [GitHub Cheat Sheet](https://training.github.com/kit/downloads/github-git-cheat-sheet.pdf)    

### [Visual Git Cheat Sheet](http://ndpsoftware.com/git-cheatsheet.html)

## Tools:

### [Meld](http://meldmerge.org/) 
Meld is a tool for comparing files and directories, and for resolving differences between them. It is also useful for comparing changes captured by version control systems(e.g. Git).

## Other resources:

### [Git - The Simple Guide](http://rogerdudler.github.io/git-guide/)

### [A workshopper for Git and GitHub](https://github.com/jlord/git-it)


