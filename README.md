
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
11. git reflog   ==>to show every command you have write (to find the version you have lost )

## notice    the difference between the check out branch
12. git checkout --<file> ==> give up the change of the specific file at the workspace, and if you have delete some file wrong ,you can replace the workspace contents with the local repository contents

13. git checkout .  ==>give up all the changes at the workspace

14. git reset HEAD file  ==> to reset the stage content to workspace
15. git rm  ==>delete the file  at the local repository

16. git remote add origin https://github.com/xxx/xxx.git  ==> connect local  repository to remote
17. git push -u origin master  ==> push local master branch to remote first time
18. git push origin master  ==>push local master branch to remote after first time, need to connect local branch to remote ,see 32

## the branch is only to check your daily work

19. git checkout -b dev   ==> create and switch to dev branch
20. git branch ==> check all the branch
21. git branch -a ==> check local and remote branch
21. git checkout `brachName` ==> switch to `brachName` branch, when switch branch please commit your change first
22. git merge dev  ==>merge the dev to current branch
22. git merge --no-commit `branchName` ==> merge brachName to current brach
23. git branch -d dev  ==>delete the dev branch,you’d better delete it after you merge to master
23. git branch -D `branchName` ==>delete forced

24. git push origin dev:dev_remote  ==>create remote new branch(dev is your local branch)
24. git push origin test:master    ==> push test to remote master(as master)
25. git push origin :test  ==>delete remote test branch 
25. git push origin --delete test  ==>delete remote test branch 

24. git clone xxx.git "filepath"  ==>specify the filepath where you want to clone
25. git pull origin <origin branchName>:<local branchName> ==> if local branchName is nil,default to be local current branch
26. git pull is equal to git fetch + git merge origin branch to current
27. git merge --no-ff -m "merge with no-ff" dev   ===>merge dev to current branch and forbid "fast forward"mode  add will commit with a new message

28. git stash  ==>save current branch working space and the work space will be clean,function to create a new branch to fix some bug,and not to commit the workspace work that not finished


## branch remote and local

30. git remote -v  ==>check remote branch link info
30. git branch –r  ==> check remote branch info
32. git branch --set-upstream branch-name origin/branch-name  ==> if pull failed ,this command will connect local branch with remote appropriate branch

## git tag:replace commit id with tag will be much more easy
33. git tag<name> ==> add a tag name
34.  git tag <name> <commit id>  default tag at latest commit,this will tag at specific commit
35. git tag -a <tag name> -m "message" <commit id>
36. git tag  ==>show all tag

37. git show <tag name> ==>see the tag info,tag is not ordered by time but charactors
38. git tag -d <tag name> ==>delete a tag local,tag default not push to remote
39. git push origin :refs/tags/<tagname>  ==> if tag name is push to remote ,delete local first,then delete remote
40. git push origin <tag name>
41. git push origin --tags ==>push all tags once

42. git log --graph  ==>see graphical of the branch merging



