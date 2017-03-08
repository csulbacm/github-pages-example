#Intro to Git with Github Pages
##Dependencies
#### Git
Install git from https://git-scm.com/ or using your OS package manager.

Check installation with `git --version`

####Github account
Setup an account with a Github by signing up 


##Git Commands
All commands and reference from git documentation.
https://git-scm.com/docs

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
Check the status of your files on the stage waiting for commit
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
git push origin master	#Pushes the master branch to the origin remote repository
```

####Cloning a repository
Copy an existing repository to your computer.
```
git clone https://github.com/csulbacm/github-pages-example.git
```



##Git Workflows
Many different types of workflows for working on Git with teams. Here is a good description.

https://www.atlassian.com/git/tutorials/comparing-workflows