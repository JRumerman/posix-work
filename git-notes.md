## GIT

### .git folder
* contains logs under logs folder
* config contains information about branches, origins, and remotes


### git init
* git init
	- initialize .git folder
* git init --bare
	- initialize folder as a repository (a place where pushes can be sent)

### git remote
* git remote add origin ssh/http
	- adds a remote origin the existing repo
* git remote -v
	- lists the fetch/push remotes for the current repo

### git revert <i>commit number</i>
	- reverts the commit listed in the commit number by committing the files necessary to revert it. 

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

### git branch
* git branches
	- shows all local branches, colorizing the current branch
* git branch -a
	- shows all local and remote branches, colorizing the current branch
* git branch -d 
	- deletes local branch, if no commits pending
* git branch -D
	- force deletes local branch
* git branch --set-upstream-to=origin/master master
	- assigns the upstream (remote repo) origin master to the local master branch 
 

### git push
* git push
	- pushes the committed changes on the current branch to the remote repository. uses default values for upstream and repo since none were specified
* git push origin HEAD
	- push the current branch to the remote of the same name
* git push origin <i>branchname</i>
	- push the committed changes on branch <i>branchname</i> and creates it on the remote if the branch doesn't exist.