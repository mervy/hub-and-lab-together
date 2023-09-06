# Usando o github e gitlab ao mesmo tempo

** Comandos do github **
```
echo "# hub-and-lab-together" >> README.md //Não precisa
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/mervy/hub-and-lab-together.git 
git push -u origin main
```

** Command line instructions - Gitlab **

You can also upload existing files from your computer using the instructions below.

** Git global setup **
```
git config --global user.name "Rogério Soares"
git config --global user.email "rgrsoares@yahoo.com.br"
```

**Create a new repository **
```
git clone git@gitlab.com:m3rvy/hub-and-lab-together.git
cd hub-and-lab-together
git switch --create main
touch README.md
git add README.md
git commit -m "add README"
git push --set-upstream origin main
```

** Push an existing folder **
```
cd existing_folder
git init --initial-branch=main
git remote add origin git@gitlab.com:m3rvy/hub-and-lab-together.git
git add .
git commit -m "Initial commit"
git push --set-upstream origin main
```

**Push an existing Git repository**
```
cd existing_repo
git remote rename origin old-origin
git remote add origin git@gitlab.com:m3rvy/hub-and-lab-together.git
git push --set-upstream origin --all
git push --set-upstream origin --tags
```

**Outros comandos úteis**
```
git remote rename origin origin-gitlab
git remote remove origin
```
https://gitlab.com/m3rvy/hub-and-lab-together.git

teste