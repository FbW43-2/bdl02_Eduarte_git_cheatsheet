# Git commands cheat-sheet: the most useful git commands
## 1. Navigate to your git project folder
Use `cd` to move between folders. For example:
```
cd workspace
cd bdl02_markopacak_git_cheatsheet
```
## 2. Check the status of the project
I can use these commands **anytime** to inspect my project.
- `git status`
    With `git status` I can see if some changes have happened and if some files are ready to be committed. 
    It gives me an overview of the project at that specific moment in time.
    Messages given by `git status`:
    - > working tree clean
    This means that no change has happened in our project since our last `git commit`
    - > nothing to commit
    
    This means that no `git add .` has happened yet, so there is no change to commit
    - > changes to be committed
    This means that we have staged some changes with `git add .`, and we now need to commit 
    - > changes not staged for commit
    This means that we need to use `git add .` to prepare some changes to be committed.
- `git log` 
    This command shows the commit logs.
- `git diff`
    Shows what changes have happened in our project since the last `git add .`.
    - Lines marked in **red** are lines that were removed.
    - Lines marked in **green** are lines that were added.
## 3. Initialize a git project 
If any `git` command that we run gives the following output:
> fatal: not a git repository (or any of the parent directories): .git
it means that **we are not inside a git project**.
In this case we can:
1. Make sure that we are inside the right folder (and navigate to it, if necessary)
2. Initialize a git project
To initialize git, run 
```
git init
``` 
This command creates an empty Git repository. From now on, we can make changes to our files and permanently save those changes.
## 4. Save changes to files
1. `git add .` (or `git add -A`)
    `git add` tells Git that you want to include the latest changes in the next commit. However, changes are not actually recorded until you run `git commit`.
2. `git commit -m "Meaningful message here"`
    A commit is the Git equivalent of a "save". Commits can be thought of as snapshots of our project at a given point in time.
    You can also *quick-commit* by running `git commit -am "Message here"`
3. `git push`
    This command sends the committed changes to a server. It is used to upload local repository content to a remote repository. 