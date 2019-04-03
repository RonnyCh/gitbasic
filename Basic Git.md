


# 1. Some Git Commands

#### Go to the directory you want to track and do the following 

git init

git add README.md

git commit -m "first commit"

git remote add origin https://github.com/RonnyCh/test.git

git push -u origin master  (i think you only need to this once, next time just git push)

#### to change the url just in case you mistype

git remote set-url origin https://github.com/RonnyCh/test.git



# 2. Branching

#### You can't delete a file in local directory and expect remote will delete. You need to create a branch in local file and make the changes and do the following. The same applies for other changes... so make sure do branches first if you already have the same files in github. If the file is new is fine since Github does not know anything about it.

1. create a branch ---> git branch test
2. go to that branch ----> git checout test
3. make some amendments..... e.g delete a file.
4. commit ----> git commit -m "delete a file"
5. move to master branch ---> git checkout master
6. merge the branch to master ---> git merge test   (this will show a file has been deleted)
7. you can delete that branch tooo ---> git branch -d test
8. now you can push your master to github online ---> git push
9. your online will be the same with local now.

# notes on using branches logic

1. once you create a branch, you need to do the usual >> add, commit, push the branch to origin.
So if the name of the branch is test >>>> git push origin test

2. by doing so.... when you use RMD and switching branch, your codes automatically updated to correct version. 

# reset the local files. e.g you delete some files from github web and want to force overwrite to local file
1. git fetch --all
2. git reset --hard origin/master  (for master branch) or
3. git reset --hard origin/<branch_name>    >>> for specific branch name


# Notes on command to read text file 
1. use command cat readme.md





