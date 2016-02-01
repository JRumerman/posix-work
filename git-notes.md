## GIT

### .git folder
* contains logs under logs folder
* config contains information about branches, origins, and remotes


### git init
* git init
	- initialize .git folder
* git init --bare
	- initialize folder as a repository (a place where pushes can be sent)


### git diff
* git diff
	- differences that have not been staged
* git diff HEAD
	- differences including those that have been staged
* git diff --cached
	- what will be committed next time commit is run
* git diff HEAD^ HEAD
	- the version before the last commit and the last commit
* git diff --name-status
	- just show the filenames


### git add
* git add .
	- stages all unstaged files
* git add filename1, filename2
	- stages filename1, filename2

### git reset
* git reset || git reset HEAD
	- unstages all staged files
* git reset HEAD filename1
	- unstages filename1

### git checkout
* git checkout <i>branchname</i>
	- switch branch to <i>branchname</i>
* git checkout -b <i>branchname</i>
	- create and switch to branch <i>branchname</i>
* git checkout --filename1
	- undoes all local changes on filename1

### git push
* git push
	- pushes the committed changes on the current branch to the remote repository. uses default values for upstream and repo since none were specified
* git push origin HEAD
	- push the current branch to the remote of the same name
* git push 