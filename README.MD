# Git

- Git is a version control system
- Git is used to collaborate on project.

# Version control system

`version control system` generally allow users to revisit earlier versions of the files, compare changes between versions, undo changes and a whole lot more.

<div style="height:200px; width: 200px; >

![Remote Image](https://git-scm.com/book/en/v2/images/local.png)

</div>

# Why To Use Git ?

1. Back to old versions.
2. Compare Versions of a project.
3. Collaborate and share changes.
4. Combine changes.
5. Tracking changes across multiple files.
6. Revert to previous versions.

# Difference between Git and Github

1. ### Git
   - Git is the version control software, that runs locally on your machine.
   - You don't need to register for an account.
   - you don't need the internet connection to use it.
   - you can use git without ever touching Github.
2. ### GitHub
   - GitHub is a service that hosts Git repositories in the cloud.
   - You need to register for an account.
   - You need the internet connection to use it.
   - It's an online place to share work that is done using git.

# Setting User Name and Email

```javascript
git config --global user.name "Your_Name"
git config --global user.email "Your_Email"
```

# Accessing User Name and Email

```javascript
git config user.name
git config user.email
```

# Basic Terminal command

- cd desktop/ : Change directory to desktop
- cd .. : get out from folder
- mkdir dirName : make new directory
- ls : content inside folder
- ls -a : show hidden file
- clear : clear terminal
- pwd : present working directory
- q : to quit
- cat fileName : show content inside file

# Repository

A Git Repository is a workspace which tracks, and manages files within a folder.

# Git Status

give us information on the current status, of a git repository and it's content.

```javascript
git status
```

# Git init

Creates an empty git repository or reinitalize an existing one and gives us .git folder which is hidden by default.

```javascript
git init
```

# touch command

It is used to create file.
`touch index.html`

# Git Commit

every time you save file it creates a unique ID that allows you to keep record of what changes were made when and by who.

<div style="background-color: white;">

![Remote Image](https://miro.medium.com/v2/resize:fit:686/1*diRLm1S5hkVoh5qeArND0Q.png)

</div>

# Git Add

The Git add command adds a change in the working directory to the staging area.  
It is a way of telling Git (please include this changes in our next commit)

```javascript
git add fileName // add one file
git add . // add all remaining file
```

-

# -m flag

The -m flag, which stands for message, is used to add a commit message to a commit.

```javascript
git commit -m "Write your message"
```

# Git log

git log show status of file after commit such as (name, email, date, message).

```javascript
git log
```

# Git branch

Git branches are effectively a pointer to a snapshot of your changes

![remote image](https://www.nobledesktop.com/image/gitresources/git-branches-merge.png)

Git branch command list all the branches we currently have in our project.

```javascript
git branch
```

- ### making a new branch

```javascript
git branch branchName
```

# Switching branch

```javascript
git switch branchName
```

# creating and switching branch

```javascript
git switch -c branchName
```

# HEAD -> main

It tells about current branch which is main. `main` is the default branch created when you initialized a git repository.

# Deleting Branch

`git branch -d <branch-name>` will delete the branch, but we cannot delete the branch in which we're currently in.

# Renaming Branch

`git branch -m <new-branch>` allows us to rename the branch, but in this case we have to be inside the branch.

# Merge command

`git merge <branch-name>` It allows us to merge two branches.

- we merge banches, not specific commits.
- we always merge to the current Head branch

# Remote

Before we can push anything up to the Github, we need to tell git about our remote reop on GitHub. We need to setup a destination to push up to.

# show Remotes

Git remote -v just display a list of remotes. if you haven't added any remotes, you won't see anything.

```javascript
git remote add origin<url> //creating remote origin
git remote -v // show url
```

# Git push

we use git push command to push our work to GitHub.

```javascript
git push origin branchName
```

# Git clone

it is used to copy repo.

```javascript
git clone url
```

# Fetch

The git fetch command downloads your work from a remote repository into your local repo but those changes will not be automatically integrated into our working files.

```javascript
git fetch remote branchName
```

# pulling

git pull is another command we can use to retrieve changes from a remote repository. Unlike fetch, pull actually updates our Head branch with whatever changes are retrieved from the remote.

```javascript
git pull remote branchName
```

# Steps to fetch and pull

1. git fetch origin
2. git pull origin main

   ### fetch and pull (branch)

   1. git fetch
   2. git switch newBranch
   3. cat fileName

# checkout

```javascript
git checkout origin/main
```
