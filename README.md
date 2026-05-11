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
