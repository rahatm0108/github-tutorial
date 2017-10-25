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
1. Go to the [Github](github.com) website.
2. Click sign up.
3. Type a your desired username and password 
4. Verify this account through the email you used to sign up
5. Go to [cloud9](c9.io) and sign in using your Github account.
6. After signing into cloud9, press the gear icon and then go to Connected Service.
7. Press the green connect button to connect your cloud9 and github
![](account.png)
* **SSH Key**:   
**SSH Key** stands for secure shell and establishs a secure connection between your computer and GitHub
1. Go to GitHub, and go to your profile settings.
2. Next, click on SSH and GPG Keys.
3. Then, click on New SSH key to make a new SSH key.
3. Title it cloud9. 
4. Then go to c9.io and press the gear icon > SSH keys tab > copy(from cloud9) and paste the SSH key in GitHub and add the SSH key.  

---
## Repository Setup

1. `mkdir filename`: Create a folder or repository through the command line
2. `cd filename`: Change into that folder 
3. `git init`: Then, initialize git in the new repository 
4. `touch README.md`: Make a README file in the folder 
5. `c9 README.md`: Open the README.md file and type something, and save the file.
6. `git status`: Type git status to check the changes made in the file.
7. `git add`: Type git add README.md to add the file to the stage
8. `git commit -m`: Type git commit -m "" and add a message about the changes made.
* **Setup a remote repo**. 
  * Go to GitHub and select the + button and press the New Repository button. 
  * Name the repository on GitHub the same name as the repository on cloud9
  * Make sure to click SSH, copy and paste into cloud9 the one that says git remote add origin git@github.com : yourgithubusername/repo-name.git. Then, copy and paste into cloud9 : git push -u origin master.
---
## Workflow & Commands
###### General commands
`mkdir`: Creates a new directory in the working directory.  
`touch`: Creates a new file  
`cd`: Changes directory  
`~`: is used to go back to root directory  
`ls`: Lists all files and directories
---
###### Important commands

`git status`: command to see which files have been edited since the last commit  
`git add`: add the file to the stage to be committed  
`git add .` 
`git add --all`: add all files including deleted or removed to the stage to be committed 
`git commit -m`: take a ‘snapshot’ of the files on the stage.  The message should be present-tense and describe what was modified in this snapshot  
`git push`: push the commited file back up to the remote


---
## Rolling Back Changes

undo edit: After you've made an edit undo it using `git checkout -- filename`  
undo add: After you've added a change undo it using `git reset HEAD filename`  
undo commit: After you've made a commit undo it using `git reset --soft HEAD~1` or `git reset HEAD~1`  
undo push:After you've pushed to the remote undo it using `git reset --hard HEAD~1`


---
## Error Handling
* If you type git init in the wrong dicrtory and intialize git type rm -rf.git to unintialize git from the current direcctroy that you are in
* If in any case you want to delete your repo(local and remote) 
  * Go to your IDE and in your repo type in rm -rf.git and this will delete your local
Go to github and click your repo. Click setting and go all they way down till you see Delete this Repository and go ahead and press delete and type the name of your repo. You have delted your remote.

---
## Collaboration

**Fork**

A fork is a copy of a repository. Forking a repository allows you to make changes without affecting the original project, and push those changes to the forked remote repository.

**Clone**

When you create a repository on GitHub, it exists as a remote repository. You can clone your repository to create a local copy on your computer and sync between the two locations. Make sure to clone the SSH url

**Pull Requests**

Pull requests are made from people who have forked a repository and made changes to it. After changes are made a pull request is submitted and the owner chooses whether or not to add those changes.
