## GIT

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
* git checkout --filename1
	- undoes all local changes on filename1
	D