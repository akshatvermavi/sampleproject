# sampleproject
## 0.To make a local Clone

  git branch -m mainnew main
  
  git fetch origin
  
  git branch -u origin/main main
  
  git remote set-head origin -a

# learn git/ guthub

https://www.w3schools.com/git/default.asp?remote=github
  
# set Proxy

npm config set proxy http://edcguest:edcguest@172.31.102.29:3128

npm config set https-proxy http://edcguest:edcguest@172.31.102.29:3128

# to clone branch from anyn repo

git clone -b new --single-branch https://github.com/MauryaRitesh/Softdart

here new = name of the new branch

# To push new project in old repo

git remote add origin https://github.com/akshatvermavi/sampleproject

git add .

git commit -m "Message you want to give after making any commit"

git branch -M dev

git push origin dev

# sampleproject

#Adding an existing project to GitHub using the command line

Simple steps to add existing project to Github.

## 1. Create a new repository on GitHub.
In Terminal, change the current working directory to your local project.

##2. Initialize the local directory as a Git repository.

  git init
	
Add the files in your new local repository. This stages them for the first commit.

	git add .

or:
	
	git add --all

Commit the files that you've staged in your local repository.

	git commit -m 'First commit'


Copy remote repository URL field from your GitHub repository, in the right sidebar, copy the remote repository URL.

In Terminal, add the URL for the remote repository where your local repostory will be pushed.

	git remote add origin <remote repository URL>
	
Sets the new remote:
	
	git remote -v

Push the changes in your local repository to GitHub.

	git push origin master

Pushes the changes in your local repository up to the remote repository you specified as the origin

# To push new file in exixting github repo.

	cd foldername

	git status
	
	git add .

	git status
	
	git commit -m "message you want to send"

	git status
	
	git push

# Create repository

	# to create an empty local repo
	git init
	
	# to create a local copy from from an existing repo
	git clone https://github.com/sampleproject
	
# update 

	# get updates but dont apply them
	git fetch
	
	# get updates and apply them
	git pull

# Commit

	# Add a file to the nnext commit (Stagging area)
	git add path/to/file
	
	# Get update
	git commit 
	# then, an editor should open and ask you to give a commit message
	
	# add all modified filess, commit them and give a commit message
	git commit -am "first commit by me"
	
	# update last commit
	git commit --amend
	
	# to see the current status of file 
	git status

# hacktoberFest Git Cheatsheet

# Commiting

## Recording changes made to the repo.

### Commits staged files with a meaningful commit message so that you and others can track commits.
	git commit -m "Commit message"

### Condenses all tracked files by committing them in one step.
	git commit -am "Commit message"

### Modifies your commit message.
	git commit --amend -m "New commit message"
 
## INITIALIZING ( Starting up Git within a project and getting it connected.)

## Initializes (or starts) your current working directory (folder) as a Git repository (repo). Initializing Creating files staged after modifying a file and marking it ready to go in the next commit. STAGing
	git init

### Copies an existing Git repo hosted remotely.
	git clone https://www.github.com/username/repo-name

### Shows your current Git directory’s remote repo. Use the -v flag for more info.
	git remote or git remote -v
 
### Adds the Git upstream to a URL.
	git remote add upstream https://www.github.com/username/repo-name



# STGING

### Checks the status of your Git repo, including files added that are not staged.
	git status

### Stages modified files. If you make changes that you want included in the next commit, you can run add again. Use for all files to be staged, or specify For specific files by name.
	git add . or git add my_script.js

### Removes a file from staging while retaining changes within your working directory.
	git reset my_script.js

## BRANCHING (Isolating work and developing work and features in one place)

### List all the current branchs An asterisk (*) will appear next to your currently active branch.
	git checkout -b new-branch

## Consolidates the creation and checkout of a new branch.
	git branch -d branch-name
 
# do it later from here

## Deletes a branch.
	git branch new-branch

## Creates a new branch. You will remain on your currently active branch until you switch to the new one.
	git checkout another-branch

## Switches to any existing branch and checks it out into your current working directory. Isolating work and managing feature development in oneplace. BRANCHing
	git branch

## Lists all current branches. An asterisk (*) will appear next to your currently active branch.
	git pull

## Fetches and merges any commits from the tracking remote branch.
	git merge upstream/main

## Merges the fetched commits. Downloading changes from another repository or sharing changes with the larger codebase. COLLABORATING AND SHARING
	git push origin main

## Pushes or sends your local branch commits to the remote repo. 
### Note: some repos use master instead of main in their commands. See changes between commits, branches, and more.
	git diff a-branch..b-branch

## Displays the diff of what is in `a-branch` but is not in `b-branch`.
	git diff 61ce3e6..e221d9c
### Uses commit id to show the diff between two specific commits.


