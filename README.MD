#Intro to Git and Github Pages
All commands and reference from git documentation.  
https://git-scm.com/docs

Atlassian also has a good tutorial and documentation for getting started with git.  
https://www.atlassian.com/git/tutorials/what-is-version-control

Git cheat sheet.  
https://education.github.com/git-cheat-sheet-education.pdf

Github pages has all the information for hosting a static site using a git repository on Github.  
https://pages.github.com/ 

##Dependencies
#### Git
Install git from https://git-scm.com/ or using your OS package manager.

Check installation with `git --version`

####Github account
Setup an account with a Github by signing up.


##Git Commands
####One time, first time git setup
Set your name and email.
```
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```
https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup

####Creating a git reposoitory
Initialize directory as Git Repository.
```
git init
```
Add changes to staging with different options.
```
git add . 		#Adds current directory
git add file 	#Adds file
git add -A		#Adds all changes
```
Check the status of your files on the stage waiting for commit.
```
git status
```
Commit changes staged to a version with different options.
```
git commit
git commit -m "Message header"
git commit -m "Message header" "Message body"
```
Push changes to remote repositories.
```
git push				#Pushes to default remote
git push origin			#Pushes to origin remote
git push origin master	#Pushes the master branch to the origin remote repository
```
If you haven't added a remote add one.
```
git remote add origin https://github.com/csulbacm/github-pages-example.git
```
####Branching and merging
Branching and mergind documentation
https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging

Use branches to seperate different features and code.
```
git branch					#Check current branch and list of branches
git branch newBranchName	#Creates new branch from current one
git branch -d branchName	#Deletes branch
```
Checkout branches to switch current work in directory to branch.
```
git checkout branchName		#Switch branches to branchName
git checkout -b newBranch 	#Create a newBranch and switch to it
```
Merge two branches.
```
git merge otherBranch	#Merges other branch to current one
```
If you run into a merge conflict, a case where there is two different versions of the history, you will need to fix it. There are existing tools to handle this for you or you can handle it manually.
```
git mergetool
```
Many options for merge tools refer to internet for different options and use what works for you.
####Cloning a repository
Copy an existing repository to your computer.
```
git clone https://github.com/csulbacm/github-pages-example.git
```
##Github pages
Insinde a github repository go to settings and go to the github pages section. Select master or gh-pages branch to build website. URL and content is generated <username>.github.io/projectname. 
https://pages.github.com/ 

##Git Workflows
Many different types of workflows for working on Git with teams. Here is a good description.

https://www.atlassian.com/git/tutorials/comparing-workflows