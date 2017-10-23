# GitHub Tutorial

_by Rahat Mazhar_

---
## Git vs. GitHub
Git is a version control system and GitHub is a web-page on which you can publish your Git repositories and collaborate with other people.  

* **Git:**   
  * Git is taking snapshots of code   
  * doesn't require Github  
* **GitHub:**   
  * requires git   
  * store code in the cloud  
  * visually track changes   
  * easily collaborate on files  


---
## Initial Setup

* **Making a Github account:**
1. Go to [github.com](github.com)
2. Click sign up
3. Enter username, email, password
4. Continue
5. Enter your experience
6. Submit
7. Account is made

* **Making a repo:**  
1. `cd ~/workspace`
2. `mkdir filename`: Make a directory 
3. `cd filename`: change into your new file from workspace
4. `git init`: intializes git in the directory

**SSH key:** SSH keys statnds for secure shell and establishs a secure connection between your computer and GitHub

---
## Repository Setup

**Init:** Initializes git in the repository     

**First add & commit:** 
1. `touch README.md` (crete README.md)  
2. Open README.md
3. Add text
4. `git add.` (This is to add the file to the stage)   

**New repo:** 
1. Go to [github.com](github.com)
2. Create repository

**Remote:** Now your remote is on github

---
## Workflow & Commands

`git status`: command to see which files have been edited since the last commit  
`git add`: add the file to the stage to be committed  
`git commit`: take a ‘snapshot’ of the files on the stage.  The message should be present-tense and describe what was modified in this snapshot  
`git push`: push the commited file back up to the remote

---
## Rolling Back Changes

undo edit: After you've made an edit undo it using `git checkout -- filename`  
undo add: After you've added a change undo it using `git reset HEAD filename`  
undo commit: After you've made a commit undo it using `git reset --soft HEAD~1` or `git reset HEAD~1`  
undo push:After you've pushed to the remote undo it using `git reset --hard HEAD~1`