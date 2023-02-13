
##Начало работы


Configure Git
To start using Git from your computer, you must enter your credentials to identify yourself as the author of your work. The username and email address should match the ones you use in GitLab.

In your shell, add your user name:

git config --global user.name "your_username"

Add your email address:

git config --global user.email "your_email_address@example.com"

To check the configuration, run:

git config --global --list




echo "# gitComands" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M master
git remote add origin https://github.com/yarov475/gitComands.git
git push -u origin master


##Продолжение
git remote add origin https://github.com/yarov475/gitComands.git
git branch -M master
git push -u origin master

обновить проект
git pull <REMOTE> <name-of-branch>
git checkout -b <name-of-branch>
git status
git reset
git checkout <default-branch>
git merge <feature-branch>
лог
