# tesla- Git and SCM 
============
Landmark-SS -                 Paypal:
===========                   =======
    Develops, Tests, Builds, deploys & monitors applications 
    Applications are the output from Softwares  

paypal:
  Releases:
   Releasing an application is taking/deploying it to the client
   In realtime we have multiple Releases.     

release1 = version1   = 1000lines of code  
   echo 'Welcome to LandmarkTech'

release2 = version2  = 2000lines of code  
   echo 'Welcome to Paypal'
   echo "Your convenient payment gateway"

Release3  = version3  = 1000 lines of code  
echo "Paypal the best payment gateway"

Rollout   --> version1 --> version2 ---> version3  
RollBack  --> version3 --> version2

The client is not happy with the latest version of the application.   
What can be done??? RollBack

Versioning in Software Development:
===================================
Version control systems = VCS:
  Local = version1, 
          version2,[5000LINES ] 
          version3 [2000LINES ] 
   cons: Single point of failure
         lacks collaboration
         in-efficient use of resources including time  
         can't RollBack

   cons: 1. Single point of failure
         2. lacks collaboration
         3. in-efficient use of resources including time  
         4. can't RollBack
  pros:  
  
  Centralised:
    cons: can't RollBack
          The central server can fail 

Distributed VCS:
===============
GIT: DVCs 
  Distributed Version Control system 
  - Git manage data as snapshots. 0 / 10 / 20 / 30 / 40 / 50 / 60 / 
  - It takes a picture of what all your files look like 
     at that moment and stores 
    a reference to that snapshot.

  Benefits: Nearly every operation is local
            git has data intergrity
            Git generally only adds data
            Rollout and RollBack  
other DVCs:
SVN --> Sub Version
CVS --> Concurrent Version system
TFS --> Team Foundation Server
Git --> 95% plus of companies are using GIT   

Git is a Distributed Version Control systems. DVCS
In our environments (Landmark) we use Git for Versioning.  

SCM = Source Code management
=======================-====  
SCM service plaforms :
  GitHub - MS
  GitLab
  BitBucket (Stash) - A
  awsCodeCommit 

IQ: As a DevOps Engineer, what are your roles & responsilities
    in Versioning with Git?
Answer:
  1. We ensure that Developers environments are configured and secured 
     We create an enabling environment for Developers to code/Develop
       DevelopmentServers are created in AWS/GCP.  
       share login details with Developers/Team [ userName/password ]  
       Ensure that git package/Software is installed 

2. Project Onboarding: 
   1. create a github account for your organisation or self  
   2. Create organisations where applicable in a SCM ['GitHub']  
       url =  https://github.com/landmarkss
   3. Create teams in SCM/github and assign members[Developers, etc.] 
       Team url = https://github.com/orgs/landmarkss/teams/paypalteam
        assigning members to teams using GitHub account userName/email
           oogunbiyi22
           amambua
           pride22
           Anyong87
           Ngohtez
           angeltemmy
       Grant permissions/roles to team members and collaborators:
           read  -- you can view codes   
           write -- you can view codes and make changes  
           admin/maintainer - ownership  
   4. Create repositories in SCM [GitHub] 
      repo url = https://github.com/landmarkss/paypal

   5. login into github
       website = https://github.com/
            name      = Amambua Ivoline Nkimih
            email     = amamivoy@gmail.com
            userName  = amambua
            password  = Admin@123.. 
            https://github.com/landmarka  

       website = https://github.com/
       login url = https://github.com/login
            userName  = amambua
            password  = Admin@123.. 


login url = https://github.com/login
url =  https://github.com/landmarkss
Team url = https://github.com/orgs/landmarkss/teams/paypalteam
repo url = https://github.com/landmarkss/paypal

  6. Ensure that Git and relevant IDEs are installed by Developers 


Git Installations
-----------------
Git Installations differs depending on your operating system:
Pre Requisite Software Download/ Registration :
Install git in Windows   :  
  Install gitbash @ https://git-scm.com/downloads [git.exe]
  $ git -v
    git version 2.38.1.windows.1

Install in RedHAT Linux servers:
    sudo yum install git  -y 

Install in ubuntu Linux servers:
    sudo apt install git  -y 
=============================
remote repository in github 
https://github.com/landmarkss/paypal
mkdir paypal && cd paypal

Assume the role of a Developer
We are developing for our paypal FinTech client. 
1. create a directory for Development   
   mkdir paypal && cd paypal  
2. Initialise this directory to keep track of 
   any change or changes in the files/codes  

[obim@demo22 paypal]$ git --version
   git version 2.39.2

Git Commands:
  git status 
  git init 
    create a Local repository [.git]  
    initialises the git repository
  git add 
  git init  

 touch list  
 echo simon >> list 

 workingArea  stagingArea LocalRepo RemoteRepo  :
   git add *   
              git commit  
                           git push 

  git add fileName  
  git add .   
  git add *  

[obim@demo22 paypal]$ 
 git config --global user.email "legah2000@gmail.com"
 git config --global user.name "Simon Legah"

with THE "git commit command -m " a version is created with a version number[commitID]  

git init          = to initialised a git empty repository
                    create the default branch[master, main]
git status        = to track files location
git log           = list all commits  
git add           = move files to staging area from working area
git commit -m     = move files to the local repository FROM STAGING AREA
                    good commit message for tracking changes created by authors are recommended

remote repository in github 
https://github.com/landmarkss/paypal

  git remote -v 
  git remote add aliasName repoURL  
  git remote add paypal https://github.com/landmarkss/paypal

  git push aliasName branchName  
  git push paypal master  
  [obim@demo22 paypal]$ git push paypal master
Username for 'https://github.com': legah2045
Password for 'https://\legah2045@github.com': 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

Class32Teams:
Project:
  1a. Create your GitHub account 
  1b. Onboard a new project for a FinTech Client
        organisation / teams / repository
  2. Managers and assistant
       Create a Team in your created organisation for paypal and add members of your 
       your group with write access 

