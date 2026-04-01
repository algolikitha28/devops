step1- instal git 
step2- then check weather it is installed using    "git --version"
step3- create a folder in vs code
step4- initialise git "git init"
step5- check project status "git status"
step6- add files to git  "git add" . - . means everything in a present file 
step7- ssh-keygen -t ed25519 -C "emailid"
step8- commit files "git commit -m "Initial commit - folder name"
step9- create repository on github
step10- connect local project to git "git remote add origin https://github.com/yourusername/epitope-prediction.git" [this link you get in git hub]
step11- push code to github "git branch -M main"
step12- "git push -u origin main"


To update-
       git status 
step1- "git add readme.md"
step2- "git commit -m "create read"  "   
step3- git add .
step4- git push
step5- git log 
commit a243627c06dda3e362450323672e0c42dc8ccf3c - it is called hash code helps in restoring files when once deleted

to create other branch- " git checkout -b feature-branch"

if we get fatal error-  git push --set-upstream origin main

Senario:
if we change the repo name - git remote set-url 
in this we will set origin

git remote set-url origin git@github.com:algolikitha/devops.git

completely reset the connections- git remote add origin git@github.com:algolikith/devops.git
after this we have to git push origin

if we want to completely remove everything
Remove-Item -Recurse -force .git

merge conflict:



 