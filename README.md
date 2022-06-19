# Git-and-Github-Cheatsheet

# Git and Github Cheat Sheet
### Git Commands
To get the version:
```
git --version
```
Configuration:
```
git config --global user.name "usama440-coder"
git config --global user.email "usamamian440@gmail.com"
```
Initialize Git:
```
git init
```
Check git status:
```
git status
```
Stage the files
```
git add index.html
//to stage all the files:
git add --all
// OR
gir add --A
```
Commit
```
git commit -m "some message"
```
Get status of repo.

| Flag  | Meaning |
| ------------- | ------------- |
| ??  | Untracked Files  |
| M  | Modified  |
| A  | Added to stage  |
| D  | Deleted  |

```
git status --short
```
Get history
```
git log
```
Help:
```
git help --all
```
Creating a new branch:
```
git branch <new_branch_name>
```
Show all the branches
```
git branch
```
Switch to another branch
```
git checkout <branch_name>
```
Creating and switching to a branch simultanously
```
git checkout -b <some_branch>
```
Merge a branch
```
git merge <branch_name>
```
Deleting a branch
```
git branch -d <branch_name> 
```
---

### Authors

- [@usamashaukat](https://github.com/usama440-coder)

