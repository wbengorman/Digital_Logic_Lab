# Digital Logic Lab Fall 2017
# Lab 01
-----------------------------------------------------------

## Description

In this lab, we will get ourselves familiar with git and github classroom tools.
All the details will be discussed in the lab session.

Some useful resources:
  - [Git manual](https://git-scm.com/doc)
  - [Git cheatsheet](http://ndpsoftware.com/git-cheatsheet.html)
  - [Git koans](http://stevelosh.com/blog/2013/04/git-koans/)
  - [Github markdown](https://guides.github.com/features/mastering-markdown/)
  
-----------------------------------------------------------

## Basic Bash Commands

  - Create directory
  ```Shell
  mkdir <dirname>
  ```

  - Show current location
  ```Shell
  pwd
  ```

  - Change directory
  ```Shell
  cd
  cd <dirname>
  cd ..
  cd -
  ```
  
  - Show all the files in current directory
  ```Shell
  ls
  ls -l
  ls -plsha
  ```
  
### Change 

## Git

![git](pics/git.2.14.1.png)

## Git commands
  - Obtaining the repository
  ```Bash
  git clone '<repository url>'
  ```
  
  - Set User information
  ```Bash
  git -global user.name “your name”
  git -global user.email your.email@email.com
  ```

  - Checking the status of the repository
  ```Bash
  git status
  ```

  - Adding changes
  ```Bash
  git add <file name>
  ```

  - Committing changes to local repository
  ```Bash
  git commit
  ```

  - Push local changes to remote
  ```Bash
  git push
  ```

  - Getting update from remote
  ```Bash
  git pull
  ```

  - Checking the logs
  ```Bash
  git log
  git log --oneline --graph --decorate=auto --color
  ```

## Assignment

  1. All members of the group must commit, i.e. I want to see all the members making meaningful changes

  2. Answer the following questions:

  - What is git? what does it do?
  	- Git is a distributed version control system. It is used as a server and adds 		access control, displays the contents of a git repository and helps to manage 		multiple repositories.

  - Why is user information important?
	- User information assigns changes made to a repository to a specific user so that 	changes to a repository can be tracked back to an individual. If the user 		information isn’t given in the commit then the user responsible for the changes 	cannot be identified.

  - What is the difference between https and git url?
  	git:
	- no user authentication or security
	- very fast and can handle large amounts of traffic
	- more difficult to set up
	- mostly read-only access
	https:
	- easier for users
	- good security with user authentication
	- fast and efficient

  - After you made a change to a file, in order to push that change to the remote repository what the steps you must perform? (List all the steps in order)
	- git add <file_name>
	- git commit <file_name>
	- git push
  - After you are informed that there are some changes have been made, what are the steps you must follow in order get those changes? (List all the steps in order)
	- git pull
