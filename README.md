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
	
	
	


