
##  git command line
1. git add<file> =>specified single file
2. git add .  =>to add all file
3. git commit -m "your message"  =>commit with message
4. git commit -a-m "your message"  => the '-a' symbol only add modified or deleted tracked file,modifed or deleted file is no need more to use "git add"
5. git commit --amend  =>change the messge you have commited
6. git status  ==> file status
7. git diff  ==>difference
8. git log ==>check history version
9. git log --pretty=oneline  ==>pretty show
10. git reset --hard<version id>  ==>reset to specified version,even is desprecated version if you still know the version id
11.git reflog   ==>to show every command you have write (to find the version you have lost )

## notice    the difference between the check out branch
12.git checkout --<file> ==> give up the change of the specific file at the workspace, and if you have delete some file wrong ,you can replace the workspace contents with the local repository contents

13. git checkout .  ==>give up all the changes at the workspace

14.git reset HEAD file  ==> to reset the stage content to workspace
15. git rm  ==>delete the file  at the local repository

16 git remote add origin https://github.com/xxx/xxx.git  ==> connect local  repository to remote
17.git push -u origin master  ==> push local to remote first time
18.git push origin master  ==>push local to remote after first time

## the branch is only to check your daily work

19.git checkout -b dev   ==> create and switch to dev branch
20.git branch ==> check all the branch
21.git checkout<brachName> ==> switch to current branch
22.git merge dev  ==>merge the dev to master
23.git branch -d dev  ==>delete the dev branch

24 git clone xxx.git "filepath"  ==>specify the filepath where you want to clone
25.git log --graph  ==>see graphical of the branch merging


