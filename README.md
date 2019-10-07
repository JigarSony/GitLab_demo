#GITLAB

* What is GitLab
* Create an account on GitLab
* Create a new project on GitLab

##Git
* Global Information Tracker
* Gastro Intestinal Tract

Git is a version control system
to locally track changes in your project/folder and push & pull changes from remote repositories like GitHub, BitBucket, GitLab

GitLab, GitHub, BitBucket
Services that allow to host your project on a remote repo & have additional features to help in SDLC and CI, CD
e.g: Managing, Sharing, Wiki, Bug tracking, CI & CD

Step 1: Go to GitLab.com and create an account
Step 2: Sign in to GitLab
Step 3: Create a new project on GitLab

## GitLab Accounts
* [RaghavPal](https://gitlab.com/RaghavPal/)
* [JigarSony](https://gitlab.com/sonijigar94/)


## Learn GIT

* Download and install Git
* Add a project/folder to git
* Commit and Push project to GitLab

Step 1: Download git from https://git-scm.com/ and install git 

Step 2: Check git is installed on your system
   git --version

Step 3: Run following git commands
   git config --global user.name “xxxx”
   git config --global user.name

   git config --global user.email “xxxx”
   git config --global user.email

   git config --global --list

Step 4: Create a demo project/folder & add to git
   
Step 5: Goto cmd OR terminal OR git bash 
     CD to the location of the folder and run the following commands
   git init
   git status
   git add .
   git commit -m “msg”
   git push -u “url” master

Step 6: Check project (files) added on GitLab

[Git PlayList]
(https://www.youtube.com/playlist?list...)

##Learn Fork

* What is fork
* How to fork a project

A fork is a copy of a project.
Forking a pro/repo allows you to make changes without affecting the original project

Step 1: Login to GitLab and goto your project

Step 2: Click on Fork button

If you get a message
No available namespaces to fork the project.           

After making changes to the fork project you can merge the changes to the original project using Merge Request

##SSH Key


>What is SSH key

>How to setup SSH key in GitLab

SSH - Secure Shell

- Used for authentication
- By setting ssh key you can connect to GitLab server without using username and password each time

Step 1: Run command 
   ssh-keygen

On Mac - run command on terminal
On Windows - use putty or git bash

Step 2: Login to GitLab 
   Goto account ＞ Settings ＞ SSH Keys

Step 3: Copy contents of id_rsa.pub and Add Key

Step 4: Verify SSH key is added


##GitLab Runner

- What is GitLab Runner
- How to install GitLab runner
- How to register GitLab runner
- How to start GitLab runner

- used in GitLab CI
    - Open-source continuous integration service  included with GitLab
- used to run jobs & send results back to GitLab

Step 1: Install GitLab Runner
https://docs.gitlab.com/runner/
https://docs.gitlab.com/runner/instal...

brew install gitlab-runner
gitlab-runner --version

Step 2: Register GitLab Runner
https://docs.gitlab.com/runner/regist...
gitlab-runner register

Step 3: Start GitLab Runner

brew services start gitlab-runner
brew services stopgitlab-runner

Step 4: Check runner is activated in the project

##GitLab CI/CD

1. What is GitLab CI/CD
2. Create .gitlab-ci.yml
3. Run CI/CD pipeline

GitLab CI is an open-source CI service included with GitLab
Since ver 8.0
GitLab CI is an open-source Continuous Integration service included with GitLab
Only project maintainers & Admin can access the Settings

Step 1: Add .gitlab-ci.yml in the root folder of your project/repo

- GitLab CI/CD pipeline is configured using YAML file called .gitlab-ci.yml in each project
- .gitlab-ci.yml file defines the structure and order of the pipeline & determines
- 
Mac - TextEdit, TextWrangler
Windows - Notepad, notepad++

demo_job_1:
     tags:
       - ci
     script:
       - echo Hello World

[YML FIle validator](http://www.yamllint.com/)

Step 2: Commit and push the file to gitlab repo

Step 3: Create GitLab runner for the project
Video - https://www.youtube.com/watch?v=R8rru...

Step 4: Start the runner

Step 5: Make any change in the project  ＞ commit ＞ push

#References:

https://gitlab.com/help/ci/quick_star...

https://docs.gitlab.com/ee/ci/

https://docs.gitlab.com/ee/ci/yaml/

https://docs.gitlab.com/runner/instal...


* [autodevops](https://gitlab.com/help/topics/autodevops/index.md)

https://docs.gitlab.com/runner/register/index.html

https://docs.gitlab.com/runner/install/osx.html

http://www.yamllint.com/

https://docs.gitlab.com/runner/

After set/start the runner when any push commit changes happen automatically runner started 
Check that in the CI/CD Jobs

