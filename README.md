# learning about git and github
## Topics
  - # basic git commands
  - # concepts 




# basic git commands
 - git init :   initalize the repository and ready to track changes in it
 - git add filename : our files are ready for commit (we write the feature and then we say we are ready )
 - git commit -m "message : take a snap shot of current version of folder (we save the feature)
 - git status : check status of the repo : it shows files are modified or added or up to date
 - git log    : see all the commits(snapshots)

# concepts
 -  github
 -  branches
 - upstream and origin
 - push
 - pull
 - fetch
 - fork and clone
 - merging
 - stash

# Advance concepts
 - rebase : make all commits into a single commits by squashing



# github 
 lol you are reading this in github :) hehehe
 - online hosting account where you can host your code and connect with local repo and easily track changes and update changes .. etc

# branches 
 Think of tree(folder which you are working on project and committing to it)

 main tree is  a repositores 
 
 branches are like sandboxes where you can take the copy of the tree and add some features it with out damaging the main tree if everything is workly rightly with features then merge the feature with the Tree
 when you are creating an repo it automatically creates a branch for you called main
 ## commands related to branches
  - git branch : to see all the branches
  - git branch name: to create a new branch (copies of main branch)
  - git checkout name : to change in to the branch speicified
  - git branch -d name : to delete the branch




## about upstream and origin

 - upstream : The project which is orginal repository which you are forked from 
 - origin   : The repository in our local github account which you are forked that is present in your github account

 - ## commands about upstream and origin
 - git remote add origin our-own-github-repo
 - git remote add upstream original-project-link

# push
 when you needed to push the changes or commits to the remote repo 
 # commands related to push
  git push origin branchName : origin is remote that is connected to this local repo and which branch are you pusing

# pull 
 when you needed to pull the changes to the local repository

 git pull origin branchname : get all the changes from the remote local repo in your github  merge it automatically

 git pull : get all the changes from main remote repo you needed to add it as upstream before  as mentioned above


# fetch

when you fetch all the changes to local repo but not merge it and make it

series of commands that needed to make repos equal locally from upstream repo

 git fetch  --all -prunge : get all the data from main repo all branches and even del ones
 
 git reset --hard upstream/main : make the local main repo branch equal to the upstream branch main

 git push origin main : send all the changes


# fork and clone
 fork : make a local copy of other repo to the your github account and add featues to it locally(github)

 clone : copy entire code into your computer either by zip or by clone command
 
 git clone urlink


# Merge
 merging is when you add the branches together (mainly some brach which you are working is a feature)

 you tested it and then merged it to the main branch and release into the proudctoin
 
  git branch feature-branch : creating a branch called feature-branch
   
  added some commits

  git checkout main    : moving into the main branch
  
  git merge feature-branch : merging feature-branch into the main branch

# stash
  make work hold for now all the work we done
  
 The files must be in staging area
 
  git stash : go back to last commit with out loosing all the work we done basically storing them some where with out taking snapshot
  
  git stash pop : get all the details back

  git stash clean : remove all the changes 



## links for learning more about git and github topics for future references
  - [upstream-info-link](https://stackoverflow.com/questions/9257533/what-is-the-difference-between-origin-and-upstream-on-github)
  - [git-fetch](https://www.atlassian.com/git/tutorials/syncing/git-fetch#:~:text=The%20git%20fetch%20command%20downloads,else%20has%20been%20working%20on.)
  - [git-fetch vs git-pull](https://phoenixnap.com/kb/git-pull-all-branches)

