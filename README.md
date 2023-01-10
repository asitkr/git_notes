# git_notes

###   25-06-2022 class
-----------------
## We have to create Git respository from github.com

GIT Repo URL : https://github.com/asitkr/Java-Jdbc.git

GIT Bash Commands
-----------------
git help --> It provides frequently used several git commands

git help <cmd-name> -->It opens documentation of that paticular commmand

git init --> It is used to create empty repository or re-instilize existing repository

git status --> This command will Display status of current repository

git clone --> This command is used to copy of any project which are already present in github respository to local
machine
syntax : git clone https://github.com/asitkr/git_notes.git

Staged Files --> Files which are added and they are ready to commit
------------ -->These files name will be displayed in green color

Un-Staged Files --> Modified files will be displayed here, we need to stage these files to commit
--------------- --> These files name will be dispalyed in red color

Un-Tracked Files --> Newly Created files, we need to stage them to commit
---------------- --> These files name will be displayed in red color

git add -->This command is used to add file to staging area

syntax : git add <file-name>
syntax : git add --a or git add .   ====> To add all files at a time

git restore --> to discard changes in working or current directory
syntax : git restore --staged <file-name>

git rm --> This command is used to un-staged newely created files

syntax : git rm --cached <file-name> ====> This command is used to Un-Tracked Files for single file at a time
syntax : git rm --cached * ===> This command is used to Un-Tracked Files for all files at a time

How to configure Email and Username
--> By using this command


syntax : git config --global user.email "you@example.com" ===> This command is used for setting the email which are on github
syntax : git config --global user.name "username" ===> This command is used for setting the username which are on github


git commit --> This command is used to commit our chnages to git local repository
syntax : git commit -m 'commit-msg'


git log --> It shows the whole commit history.
syntax : git log


git branch --> List all of the branches in your repository which is already present.
syntax :  git branch


git branch <branch_name> --> This command is used to create a new branch which having some name
syntax : git branch <branch_name>
i.e : git branch branch_name(dev)


git branch -d <branch_name> --> Delete the specified branch. This is a “safe” operation in that Git prevents you from deleting the 
        branch if it has unmerged changes.
syntax :  git branch -d <branch_name>


git branch -D <branch_name> --> Force delete the specified branch, even if it has unmerged changes. This is the command to use if you want to 
        permanently throw away all of the commits associated with a particular line of development.
syntax : git branch -D <branch_name>


git branch -m <branch_name> --> Rename the current branch to new branch_name.
syntax : git branch -m <branch_name>


git checkout --> This command is use for changing the branch.
syntax : git checkout


git checkout -b ＜new-branch_name＞ --> This command create the new branch and immediately switch to it
syntax : git checkout -b ＜new-branch_name＞

Note : When we execute commit command it will consider all files which are in staging area

Note : Git local repository will be available in our machine only

To commit our files to remote repository we should execute below commands :--
1. git remote add <repo-url> ===> This required only first time only
2. git branch -M main ===> This is required for changing the baranch Master to Main(Default Master barnch is Avilable)
3. git push -u origin main ===> If it branch is selected as main then we used this command to move changes from local to central respository
4. git push -u origin master ===> If it branch is selected as master then we used this command to move changes from local to central respository

git reset --> It is used to unstaged a file
syntax : git reset HEAD <file-name>
