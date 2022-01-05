
# Git and GitHub course with notes- OceanProgrammer

Git and GitHub are used a lot in software developement. So it gets much important for you to have its knowledge.
**Here are some git commands:**


## A diagram explaining the 3 stage architecture of Git
![App Screenshot](https://miro.medium.com/max/500/1*9hNsHV22lsi03i9Ah92KmQ.png)

```bash
$ git config --global user.name "User_name" #providing our username to git
```
```bash
$ git config --global user.email "youremail@test.com" #providing our email to git
```
```bash
$ git config --list #displays a list of information you have provided to git
```
---
```bash
$ git status #shows the status of current repository
```
```bash
$ git init #initialize current repository with git
```
```bash
$ git add -A #add all files to staging area
```
```bash
$ git restore --staged myFile.py #Unstage this file
```
```bash
$ git commit -m "<commit message>" #files get commited
```
```bash
$ git commit --amend -m "Changed latest commit" #Rename your commit
```
```bash
$ git log #display a list of commits
```
```bash
$ git tag -a v1.1 -m "<tag message>" #add a tag with the name
```
```bash
$ git tag #display a list of tags made
```
```bash
$ rm -rf .git #this command deletes the .git/ folder
```
---
```bash
$ git clone https://github.com/OceanProgrammer/git-tutorial-with-notes.git #gives a copy of this repository
```
# To push file(s) to GitHub, follow the given steps:  
```bash
$ git remote add origin git@github.com/UserName/repo.git
```
```bash
$ ssh-keygen -t ed25519 -C "your_email@example.com"
```
```bash
$ eval "$(ssh-agent -s)"
```
```bash
$ ssh-add ~/.ssh/id_ed25519
```
```bash
$ clip < ~/.ssh/id_ed25519.pub #Now copy your SSH key using this command & add it into your GitHub
```
```bash
$ git branch -M main
```
```bash
$ git push -u origin main #Final command to push into github
```
---
```bash
$ git log --pretty=oneline #All commits are displayed in one line
```
```bash
$ git log --stat #All commits are displayed with some additional information
```
```bash
$ git log --p -1 #Shows one latest commit
```
---
```bash
$ touch .gitignore #Creates a .gitignore file
```
```bash
$ git rm --cached something.txt #Unstage this file which was previously in working tree
```
```bash
$ git commit --amend -m "Changed latest commit" #Rename your commit
```
```bash
$ git checkout myMainFile.py #Match this file with latest commit
```
```bash
$ git checkout -f #Match all files with latest commit
```
```bash
$ git checkout <commit_hash> #Match all files with the commit of this hash.
```
```bash
$ git diff #Compares working tree with staging area
```
```bash
$ git diff --staged #Compares staging area with recent commit
```
```bash
$ git config --local alias.sts status #Instead of *git status* you can now use *git sts*
```
---
```bash
git branch <branch_name> #Create a new branch
```
```bash
git checkout master #Come back to master 
```
```bash
git branch -d new #Delete this branch
```
```bash
git -m test test2 #Rename this branch
```
```bash
git merge test2 #Merge this branch with master
```
```bash
git branch --merged #Shows merged branches
```
```bash
git branch --no-merged #Shows unmerged branches
```
```bash
git push -u origin main #Push this branch to github
```
```bash
git push -d origin main #Delete this branch from github
```