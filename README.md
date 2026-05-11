# This is my local repo

#1. here we used git init command to initialise a git repo.
#2.1 git remote add origin <-URL of github repo: for this a new github repo needs to be created->.
#2.2 git remote -v : to access the above url
#2.3 we used git branch command to fetch the name of the  branch.
#3. Git branch -M "branch to be renamed" : this is to rename any branch
#4. Git Push -u origin main : -u (it is used to set upstream): so now onwards we can just write "git push" to push any further changes to the same branch as mentioned in upstream.
#5. CREATE NEW BRANCH : Git checkout -b <-new branch name here-> eg. Git checkout -b Feature1
#6. Navigate branch : Git checkout <-branch name> eg. Git checkout main (to navigate back to main branch)
#7. DELETE branch : Git branch -d <-branch name->

#MERGE BRANCH : 
METHOD 1:

#1. Git diff <-branch name-> : Check the differences btw the branches & compare the changes.
#2. Git MERGE <-branch name-> : Merge the 2 branches. 

METHOD 2: Pull request on github
But here if you successfully merged the branches, to see your changes in your code also in local system you'll need to pull the contents from remote repo, immediately Update your local repo & match the content.
: Git pull origin main

Undoing changes:
Case 1: Staged changes
#1. git reset <-file_name> eg. git reset <-file name like index.html>
#2. git reset

Case 2 : Commited changes (need to go back one step)
#1. Git reset HEAD~1

Case 3 : Commited changes (need to go back many steps)
#1. Git reset <-commit hash-> 
: i.e every commit has a nique hash associated with it , identify the hash & paste it in the command ( git log : command to find out the hash)

#2. git reset --hard <-commit hash-> 
(after using the command #1 , we can check git status : observed that the changes post the provided hash are still present in vs code as it shows the modified status, so to hard reset to the provided hash use this , now you would no longer have a modified status for this code & you can continue coding as if nothing happened after that point)
