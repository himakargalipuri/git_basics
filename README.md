
# Everything about GIT a software developer needs to know!

  

### git clone

  

To clone the git with existing name

    git clone URL_HERE
To clone from a specific branch

    git clone -b BRANCH_NAME URL_HERE
To clone to a specific folder

    git clone URL_HERE PROJECT_NAME

If working with multiple git accounts remotely 

    `git clone https://username:password@github.com/username/repository.git`  

### add remote to git folder

      git remote add origin LINK_TO_GIT

  

### get remote details

  
    git remote -v

or

    git remote show origin

  

### change git remote

  

    git remote set-url origin URL_HERE

  

### remote delete

  

    git remote rm destination/origin

### basics
check git status

    git status

add files to git

    git add .

    git add SPECIFIC_NAME  

    git add \*.FILE_EXTENSION
commit with a message

    git commit -m "YOUR MESSAGE HERE"

push to remote

    git push -u origin BRANCH_NAME

### Remove already indexed files from git

  
For all files and folders

    git rm -r -cached .

or for a specific file

    git rm -cached FILE_NAME

or for a specific folder

    git rm -r -cached FOLDER_NAME

  

### Hard pull

Force pull from remtoe  

    git fetch --all
    git reset --hard origin/BRANCH_NAME

  

### Pull all remote branches at once

  

    git pull -all

  

### Reset one commit

  

    git reset --hard HEAD~1

  

### Revert specific file to specific commit

  

    git checkout c5f567 -- file1/to/restore file2/to/restore

  

### create branch and update

  

    git checkout -b BRANCH_NAME
    git push -u origin BRANCH_NAME

  

### list/update git branches

  

    git fetch

  

### match local and remote

  
This method will reset all uncommitted/saved changes

    git fetch origin
    git reset --hard origin/master

  

### view change history of a file

  

    gitk FILE_NAME

  

### restore a deleted file

  

    git log --diff-filter=D --summary
    
    git checkout COMMIT_HASH~1 PATH_TO_FILE

  

### merge branch to master

  

    git checkout master
    
    git pull origin master
    
    git merge BRANCH_NAME
    
    git push origin master

