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
# Git - login to GitHub via SSH Key
````
# SSH key generation
ssh-keygen
cat ~/.ssh/id_rsa.pub 

#In case of https and ssh 
git remote -v
origin	git@github.com:anpavlovsk/Git-GitHub-crib.git (fetch)
origin	git@github.com:anpavlovsk/Git-GitHub-crib.git (push)

git remote set-url origin git@github.com:anpavlovsk/Git-GitHub-crib.git  
````
