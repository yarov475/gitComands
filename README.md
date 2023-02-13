
##Начало работы


Configure Git
To start using Git from your computer, you must enter your credentials to identify yourself as the author of your work. The username and email address should match the ones you use in GitLab.

In your shell, add your user name:

git config --global user.name "your_username"

Add your email address:

git config --global user.email "your_email_address@example.com"

To check the configuration, run:

git config --global --list

## разлогиниться
git config --global unset -all

залогиниться с нуля
https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
## FIND FOLDER WITH SSH
cd ~
cd .ssh
# Start the ssh-agent in the background.
## Sheck if there are ssh keys
 ls -al ~/.ssh
# Lists the files in your .ssh directory, if they exist
# the ssh ar like:
id_rsa.pub
id_ecdsa.pub
id_ed25519.pub

### if there no SSH
### Generating a new SSH key and adding it to the ssh-agent
$ eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519

# Then select and copy the contents of the id_ed25519.pub file
  # displayed in the terminal to your clipboard

 cat ~/.ssh/id_ed25519.pub

 githyb.com>profile>settingd>keys (https://github.com/settings/keys)> ssh keys> new ssh keys


сделать SSH
добавить SSH на сайте 
## поменять оригин на ssh с https
удалить старый оригин
сделать новый(на сайте над папкой)
An HTTPS URL like https://github.com/user/repo.git
An SSH URL, like git@github.com:user/repo.git

git remote -v (покажет адреса ремоут)
git remote rm origin (удалит оригин)
git remote add origin <REMOTE_URL>(задаст оригин. копируем его с сайта. важно чтобы он был вида  ssh как An SSH URL, like git@github.com:user/repo.git )

можем начинать работу


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
git checkout <default-branch>
git merge <feature-branch>
