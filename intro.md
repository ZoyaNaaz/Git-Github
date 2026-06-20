# GIT

-> version control system to keep track of the changes in software.
-> Git is a software for tracking

## Github

-> Service or a cloud service.

## repo

-> github repo

## git init(one time per project)

-> only initialize git the repo which you want to track
-> creates .git (hidden) folder

## branch

-> you will always be on some branch (master, main, anyother)

## git log

-> commit history
-> use 'q' to end terminal current command

## git commit

-> it will open vim if opened without -m msg.
-> opens in terminal.
-> to close -> use esc+:+q or q! to forcefully quit

## Atomic commit

-> one thing at a time
-> present tense, imperative
-> means give order to your codebase

## .gitignore file

-> use to ignore sensitive files

## .gitignore generator

-> use .gitignore generator to generate .gitignore file for respective environment.

## branch

-> like an alternative timeline

## create branch

git branch <branch-name>
git switch -c <branch-name> -> create a branch & move there
git checkout -b <branch-name> -> create a branch & move there

## branch switch

git checkout <branch-name>
git switch <branch-name>

## branch work

-> branches are independent.
-> changes made in one branch will not be visible in the main until merged

## merging of branch

-> make sure you're on the branch where you have to make other branch merge.
-> fast forward(no conflict)
git merge <branch-name>
-> not fast forward(conflicts)
-> main branch is working along with some other branches on same code files
-> git tries best to resolve these conflicts
-> git merge <branch-name>
```
<<<<<<< HEAD
    Looks good as a project footer added
=======
    Looks good as a project

    footer was added successfully
>>>>>>> footer
```
-> keep the only part 
## delete branch

git branch -d <branch-name>

## conflict

changes on same file/folder on different branch, conflict happens while merging

## git diff

-> informative command
-> shows difference in 'x' time and 'y' time in the same file.
-> compare working with staging

-> reading git diff
```
a -> file1 & b -> file2(same file over time)
--- => file1 (indicate changes in file)
+++ => file2 (indicate changes in file)
changes in lines & little preview of it.
```
-> git diff requires other info (--staged, <commit>)
```
git  diff --staged
git diff <commit> <commit>
git diff <commit>..<commit>
```
## git stash

-> temp area to store your unstaged changes.
-> you have to bring those changes as well.
```
git stash
git stash pop
git stash list
git stash apply
```
## more commands
```
git checkout <hash> (detach head): new branch
git switch main (reattach hash)
git checkout HEAD~2 (look at 2 commits prior)
git restore filename (get back to last commit version)
```

## git reflog

-> moves back head to its previous position
