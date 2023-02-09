Scenario 1: 
How to clone Cydeo project from github ? 

1.go to spring project url (cydeo repo)
	https://github.com/Cydeo-JD-A3/spring
2.Intellij- File - New - Project from version control
3.Paste the https link
4.clone 
	If it asks login, please choose login via Github and proceed.

The main point of cloning project from github is getting the update during the class. you have 2 intellij project open during classes, one you will be coding, other one (this) only get the updates.

During the classes, wheneverf ozzy push the code click blue arrow to get updates. you will NOT code anything in this repo

====================
Scenario 2: how to create project from intellij and push to github (individual)
	1.Create a maven project 
	2.Top menu, VCS
	3.Click Enable Version Control 
	4.Click OK

	To add files 
	1.Right click, git, add file 
	2.Commit button on right top to commit changes

	to create remote repo on github
	1.Git (on the top menu)
	2.Github
	3.Share project on github

	once we shared our project for the first time, we can commit and push our changes. 

	these are the basics of github with intellij 

========================

Scneario 3: Global Git Ignore file 
for mac
	1.open sublime 
	2.copy paste gitignore content form jamal-only channel gitignore file. 
	3.save file under users/your username as .gitignore
	4.you might see some pop up, click use "."
	5.open terminal
	6.execute following command
		git config --global core.excludesFile '~/.gitignore'
for windows
    1.open Powershell
    2.execute following command
           cd ~
    3.execute following command
           new-item "$Env:USERPROFILE\.gitignore"
    4.execute following command
           notepad "$Env:USERPROFILE\.gitignore"
    5.copy paste gitignore content form jamal-only channel gitignore file, and save it.
    6.execute following command
        git config --global core.excludesFile "$Env:USERPROFILE\.gitignore"

=========================
Scenario 4: Module Structure
	This is will be your own, and you will code what ozzy do in class.It will be module structure like ozzy's spring repo.

	1.File-New Project
	2.select empty project and name it spring-framework
	3.Enable VCS
	how to create module ? 
	1.New -> Module
	Name: demo
	Next, and finish

	after you add each module, you need to git, add pom.xml and src folder

	***to create remote repo for the first time, git, github, share project on github***

	How to remove module ?
	1.right click module folder
	2.remove module
	3.then right click again 
	4.delete

	commit and push changes to make sure remote repo is also updated. 

	This spring-framework repository is the second repo you will be using during the class. for each part of development, you will be coding with ozzy and commiting you changes. it will be your profile besides the project that tou will be working on. 

============================================================
Scenario 5: working together 

To work together as a team we can follow github flow. it is a branch based work flow, whenever you want code you follow these steps;
	
	1.Create a branch from master/main(default branch)
		-branch allow us to have same environment with master and not affect the code. we will be working on the branch that we created. 
	2.commit your changes
		-do your work and commit 
	3.open a pull request 
		-we open a pull request to merge our work with master branch. most of the time it will requre some review, approval to merge. 
	4.review and approve 
		-someone from the team, based on structure and rules will review and approve your changes or ask for changes. after approval someone can merge the code or whoever assigned.

Scenario 6: Master updated while working - conflict 
	
	we created branch for feature and working on it but before we create PR, we need to make sure we have updated version of the master branch to avoid merge conflicts. so after our work done, we need to checkout master , get the updates, pull, checout the our branch and merge. if there is a conflict we can update the code. 



Save your changes to switch between branches without commits
Git -> Uncommitted changes -> Stash changes

checkout bracnh and comeback

Git -> Uncommitted changes -> Unstash changes

=========================
