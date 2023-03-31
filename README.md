# Github-Practice
This project is nothing but practicing all the commands to upload the data from our local repo (folder) to the remote repo (folder).

## Steps to follow while using the git.

Step 1 :

Inorder to push your code into the Github 
First you have to do few things which are :

Initially the code is in your local folder (repo)
we should keep track of the changes happening in your code 

so in order to keep track of changes in your code 
you should do : `git init`

This will create a .git in your folder and look after the changes.

Step 2 :

Now we need to select which are changes we need to make 

`git add <file_name>`

If you want to send all the files `git add .`

Step 3 : 

`git status`

you can see which are the tracked items and which are untracked items.

Step 4 :

now that you have seleccted all the files you wanted to add
now all the files will be added with one command 

`git commit -m "first"`

Step 5 :

These these will be stored in a master repo by default.
You can check where our files are stored by using command 

`git branch`

you can see that they are present in *master

Step 6 :

By default when we create remote repository its origin is in main
so we need to change our branch to main by using 

`git branch -M main`

Step 7 :

if you check the git branch it shows as *main

Step 8 :

Now we should add the local repo to the remote repo
for that we should create a remote repo in github 
we get the address from the <code> https://
copy the address and put it in the command 

`git remote origin add <https://>`

This will set the address as a remote origin.

Step 9 :

Now we should push the local repo into the remote repo

This is the first time we are pushing so we should specify the location

`git push -u origin main`

if you didnt change the repo from master to main use 

`git push -u origin master`

From the second time on you can just use `git push` and it will work fine

If there is a error in pushing try

`git push --set-upstream origin master`

There might be a case that while creating a remote repo in github and you might add addMe 
which means you have made changes to the remote and now it becomes someothers repo so 
we should pull the code 

`git pull`

this will save the code in the remote to your repo 

Now we can push the data 

`git push`

if there is a case where pull also doesnt work 

do a force push 

`git push -f --set-upstream origin main

remember that all the existing code in the remote repo will be gone if you do a force push.






