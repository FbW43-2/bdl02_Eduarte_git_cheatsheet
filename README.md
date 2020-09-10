# Git commands cheat-sheet: the most useful git commands

I can use these commands anytime to inspect the progress in my project.

## 1. Navigate to your git project folder.

use 'cd' to move between folders.

## 2. Check the status of the project

- 'git Status:
With *git status* I can see if some changes have happened and if some files are ready to be committed.
It gives me an overview of the project at that specific moment in time.
- 'git log':

## 3. Initializing a git project

if any 'git' commant that we run gives the following ouput:
> fatal: not a git repository (or any of the parent directories): .git

it means that **we are not inside a git projct**.

in such case we can:

1. Make sure that we are inside the right folder (and navigate to it, if necessary)
2. Initialize a  git Project

to initialize git, run


git Init

This command creates an empty Git repository. From now on,  we can make changes to our files and permanently save those changes.

## 4. Save changes

1. 'git add .' (or 'git add -A'
2. git commit -m "Meaningful message here"

	A commit is the Git equivalent of a "Save"
	
3. git push.

