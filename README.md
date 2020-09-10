# Git commands cheat-sheet: the most useful git commands
## 1. Navigate to your git project folder
Use `cd` to move between folders.

```
## 2. Check the status of the project
I can use these commands **anytime** to inspect my project.
- `git status`
    With `git status` I can see if some changes have happened and if some files are ready to be committed. 
    It gives me an overview of the project at that specific moment in time.
- `git log`
- `git diff`

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
3. `git push`
    This command sends the committed changes to a server. It is used to upload local repository content to a remote repository.