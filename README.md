# Git-GitHub-crib
Git and GitHub basics

### Git - configuration .gitconfig
````
git config --global user.name "Andriy Pavlovskyi"
git config --global user.email "anpavlovsk@gmail.com"
git config -l
````
Output
````
user.name=Andriy Pavlovskyi
user.email=anpavlovsk@gmail.com
````
### Git - work with local repository
````
git init
git add .
git status 
git commit -m "Comments"
````
### Git - change history, .gitignore, file restoring
````
git log
git log -p
git log -p -1
git diff --staged
git checkout -- file.txt
````
### Git - upload project to GitHub
````
git clone
git push origin
````
### Git - login to GitHub via SSH Key
````
# SSH key generation
ssh-keygen
cat ~/.ssh/id_rsa.pub 

#To change https on ssh for access (Code)
git remote -v
origin	https://github.com/anpavlovsk/Git-GitHub-crib.git (fetch)
origin	https://github.com/anpavlovsk/Git-GitHub-crib.git (push)

git remote set-url origin git@github.com:anpavlovsk/Git-GitHub-crib.git  
````
### Git - Branch
````
git branch
git branch test
git checkout test
#or
git checkout -b test

#Merge 
git checkout main
get megre test

#Delete branch
git branch -d test
#If branch is not merged
git branch -D test

````
### Git - return to previous version
````
git log
git log checkout 1ba4
git chechout main

#Delete commits
git reset --hard HEAD~2

#Delete commit logs
git reset --soft HEAD~3

#To change last commit 
git commit --amend
````
### Git and GitHub - full working cycle
````
git clone git@github.com:anpavlovsk/Git-GitHub-crib.git
git checkout -b anpavlovsk_Ticket0897
git push origin
git push --set-upstream origin anpavlovsk_Ticket0897

git checkout main
git branch -d anpavlovsk_Ticket0897
git push origin --delete anpavlovsk_Ticket0897

````
### Git - tags on GitHub
````
git tag
git tag v1.0.0
git tag -a v1.2.0 7h54f
git push origin v1.0.0

git chechout v2.0.0

git tag -d v1.1.1
git push origin --delete v1.1.1

git log --pretyy=online
````
