# Git

## Version Control
Version Control Systems (VCS) is a program or set of programs that tracks changes to a collection of files.</br>
Its goals are:
-  To easily recall earlier versions of individual files or the entire project.
-  To allow several team members to work on a project, files at the time without affecting each other's work.
Another name for VCS is *software configuration management (SCM) system.*</br>

With VCS you can:</br>
-  See changes made on project, when changes were made and by whom.
-  Create branches where changes can be made by different people performing actions at the same time like fixing bugs without affecting the main. Later on the changes can be merged if they are to be kept in the main branch.</br>
-  Retrive past versions of files or individual files.
-  Include comment with each change and explanation.

## Git
It is a distributed version control system that is free and open source that developers and other contributors can use to work on a project.</br>
### Git Terminology
1. __Repository (repo)__: It is where Git keeps all the the history and metadata for a project. A *bare repository* is one that isn't part of a working tree and is usually a directory with a name ending with *.git* e.g *barely.git*
2. __Working Tree__: Set of nested directories and files containing projects being worked on.
3. __Hash__: A number produced by a Hash function representing contents of a file or another object as a fixed number of digits. Using hashes enables Git tell whether a file has changed by hashing its contents and comparing result to the previous hash.
4. __Object__: A Git repository has four types of objects each uniquely identified by SHA-1 hash. 
-  *Blob object* contains ordinary file.
-  *Commit object* represents a specific version of the working tree.
-  *Tree object* represent a directory which has names, hashes and permissions.
-  *Tag* is a name attached to a commit.
5. __Commit__: is to make a commit object meaning you are commiting changes you have made.
6. __Branch__: is a named series of linked commit. *Head* is the most recent commit in a branch. When you initiate a repository the default branch created is the ``main`` often named ``master`` in Git. The head of current branch is named ``HEAD.``
7. __Remote__: is a named reference to another to another Git repository. When creating a repo, Git creates a remote named ``origin`` that is default remote for push and pull operates.
8. __Commands, subcommands and options__: operations in Git are performed by *commands* like ``git commit``, ``git push``. ``git`` (is the command). ``push`` ``commit`` (is the subcommand). *Subcommand* is the operation you want Git to do. *Options* accompany commands which use hyphens (-) or double hyphens (--) e.g ``git reset --hard``

### Git command line
You can use GUI available for Git like GitHub Desktop or programming editors like Microsoft Visual Studio Code but they have different limitations hence the use of Git command line which enables one tap to all of Git's functionality without being confronted with error messages.

### Git and GitHub
Git is DVCS to give access to multiple developer and other contributors to work on a project. GitHub is a cloud platform that uses Git as its core technologies.</br>
Features in GitHub include issues, discussions, notifications, pull requests, labels, actions, folks, projects.

### Git commands
Some of the git commands commonly used are:
- ``git status:`` this command lets one see which changes are currently being tracked by Git so one can decide whether to ask Git to take another snapshot.
- ``git add:`` this command is used to let Git know it needs to start keeping track of changes in certain files. </br>
Use ``git add`` is used to track all changes on files listed Git when you run the ``git status`` command in both the untracked and the modified section.
*Staging* is the technical term for these changes. Files added but not commited yet are stored in the staging area.
- ``git commit:`` the command is invoked to save work to a snapshot ``git commit -am`` to commit modified files.
- ``git log:`` this command allows one to see into previous commit. It prints information about the recent commit e.g. authors, commit message anfd their time stamp.
- ``git help:`` used to acquire information about all commands. Commands come with a help page e.g. to find the help page for the ``git commit`` command type ``git commit --help.``
- ``git push:`` this command is used to upload git commits to a remote repository e.g. Github.
- ``git pull:`` this command is used to download changes from remote repository to local machine. It is the opposite ``git push.``
- ``git clone:`` this command is used bring a repository that is hosted somewhere e.g. GitHub into a folder on local machine.
- ``git innit:`` this command is used to create a new Git repository.
- ``git remote:`` this command lets one create, view and delete connection to other repositories.
*Git branching* allows developers to diverge from production version f the code to fix a bug or add a feature.
- ``git branch:`` this command lists the branch you are on.</br>
Use the ``git branch -d`` command to delete branches especially after merging.
- ``git checkout:`` this command is used to switch between branches. </br>
To create a new branch use ``git checkout -b`` command followed by the name of the branch you want to create. 
- ``git diff:`` this command is used to show what changes havebeen made.
- ``git merge:`` this command merge changes made,
*Pull request* a request to have a code pulled into another branch.
- ``git pull:`` this command is used to fetch and download content from a remote repository and update on local repository to match the content.
- ``git reset:`` this command is used to undo a staging.
- ``git log:`` this command is used to see a log of all commits.



