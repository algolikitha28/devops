GIT:s
step1- instal git 
step2- then check weather it is installed using    "git --version"
step3- create a folder in vs code
step4- initialise git "git init"
step5- check project status "git status"
step6- add files to git  "git add" . - . means everything in a present file 
step7- ssh-keygen -t ed25519 -C "emailid"
step8- $env:USERPROFILE\.ssh\id_ed25519.pub (copy this link)
github account- profile- settings- ssh and gpu keys-new ssh key- "my commit"-paste the link in key - add verify 
step9- commit files "git commit -m "Initial commit - folder name"
step10- create repository on github
step11 - git remote -v
step12- connect local project to git "git remote add origin https://github.com/yourusername/epitope-prediction.git" [this link you get in git hub]
step13- push code to github "git branch -M main"
step14- "git push -u origin main"


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

BRANCHES IN GIT:
to create - git checkout -b feature-branch
to delete the branch- git branch -d feature-branch
git checkout main


DOCKER:
1. docker --version

2. create a new file named Dockerfile(exactly same word)

3. then type this command in Dockerfile 
              FROM nginx:alpine
              COPY . /usr/share/nginx/html

4. docker build -t devops .

5. docker run -p 8080:80 devops
it will run then press ctrl+c , then open localhost  8080 in googlt tab and click on http and check the index.html changes

6. then agin make some changes in index.html and save it and then again run docker build and docker run 

5. Then in yml file enter this command
             - name: Build docker image
        run: docker build -t devops .

6. git add .

7. git commit -m "Docker support added"

8. git push

9. docker run -d -p 8080:80 -v ${PWD}:/usr/share/nginx/html --name webdev devops

10. docker exec -it webdev sh

11. ls

NOTE: if you get error stating"you are not currently on a branch" when git push then enter git checkout main 
and then whole Dockerfile will be deleted and do from starting