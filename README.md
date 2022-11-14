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
git config --global core.editor "code --wait"
git config --global core.autocrlf true (for windows)
git config --global core.autocrlf input (for Mac)
```
Open git settings in Vs Code
```
git config --global -e
```
Initialize Git:
```
git init
```
Check for all files
```
git ls -a
```
Remove git
```
rm -rf .git
```
Check git status:
```
git status
```
Suppose you have ```file1``` and ```file2``` in a working directory. You stage both files and then commit. After that you have deleted for some reason ```file2``` but it is still in the staging area. You must have to add that file to remove it from staging.
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
Skipping the staging area
```
git commit -a -m 'message'
```
To delete file in project and in staging area at the same time:
```
git rm file2.txt
```
Add a .gitignore file
```
echo logs/ > .gitignore
git add .gitignore
git commit -m 'adding an ignore file'
```
If a file is already in working directory and committed and then you add it in .gitignore, it will show a message to be committed each time you change in that file. That should not happen. So, we want that file in working directory and in .gitignore but not in staging area(that file is important to us to make the code run)
```
git rm --cached -r bin/
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
### Github Commands
After creatting a repo, copy HTTPS link
To add a remote repository,
```
git remote add origin <copied_link>
```
Push master branch to remote URL
```
git push --set-upstream origin master
```
or
```
git push -u origin master
```
Fetch updates to see what has changed
```
git fetch origin
```
If recent changes, on branch behind, to better verify
```
git log origin/master
```
```
git diff origin/master
```
Now if no difference, merge
```
git merge origin/master
```
Pulling all the changes from romote to local repo (combination of fetch and merge)
```
git pull origin
```
If made any changes in local repo, check status first
Commit the changes
```
git commit -a -m 'updating'
```
Push to the origin
```
git push origin
```
If added a new branch to local repo, check the list
```
git branch -a
```
Now checkout to the new branch
```
git checkout <branch_name>
```
Check if its all up to date
```
git pull
```
Push a new branch to Github
```
git push origin <branch_name>
```
To clone a project:
```
git clone <url-of-project>
```
Check if you have a full copy
```
git log
```
We have full copy, origin is not allowed to make changes to
See the remote configuration
```
git remote -v
```
Rename the origin
```
git remote rename origin upstream
git remove -v
```
After fetching, add origin to remote
```
git remote add origin <url_of_project>
```
Now you have 2 origins
* origin (read-write)
* upstream (read)
### Authors

- [@usamashaukat](https://github.com/usama440-coder)

