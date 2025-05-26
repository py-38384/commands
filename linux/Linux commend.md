```
pwd - current path.
ls - list path.
mkdir new folder - folder creation
ls -R - recursive listing
ls -a - show hidden folder
history - show all executed command
mv /home/c/myfile/text.txt /home/f/ (file move example)
cp /home/c/myfile/text.txt /home/f/ (file copy example)
top (show most consuming possessing)
ps (show all possessing)
ps -a (show all possessing in details)
kill 2557 (kill a possessing with Possess ID)
sudo su (be regular user to root user)
apt install vim (example of installing a software)
Commend To Refresh Application Menu list: update-desktop-database ~/.local/share/applications
Giveing A File Executeing Permission: chmod +x your_file_name.run
Run The Executeable file: sudo ./your_file_name.run
Xampp Commands: sudo /opt/lampp/lampp start, stop, restart, startapache, startmysql
Recursively delete a directory and its files: rm -rf directory/

Generating ssh key

     ssh-keygen -t rsa -b 4096 -C "piyal13133@gmail.com"

Activeing agent

    eval "$(ssh-agent -s)"

Creating agent file

    touch ~/.ssh/config

Creating agent file (for windows)

    ssh-add C:\Users\[Your-Username]\.ssh\id_rsa

Opening agent file

    nano ~/.ssh/config

Adding key to agent

    ssh-add ~/.ssh/id_rsa

See private key

    cat ~/.ssh/id_rsa

See public key

    cat ~/.ssh/id_rsa.pub

Connect key to github

    ssh -T git@github.com

Check git remote path

    git remote -v

Remove remote path

    git remote remove origin

File Hard reset

    git reset --hard

File recover

    git checkout filename

Update local
    
    git pull origin master

Update remote 

    git push origin master

Commit

    git commit -m "commit message"

git show different between working tree vs staging area

    git diff

git show different between previous commit vs staging area

    git diff --staged

Direct Commit

    git commit -a -m "Direct commit message"

Git delete

    git rm file.name

Git rename

    git mv currentFile.name renamedFile.name

Git Untrack

    git rm --cached <file_name>

Git repository delete

    rm -rf .git

Git alias

    git config --global alias.st "status"

Git new Branch
 
    git checkout -b branchName

Git switching Branch

    git checkout branchName 

Git show all Branch

    git branch

Git merge

    git merge branchName

Git show branch with small detail

    git branch -v

Git show merged branch

    git branch --merged

Git show unmerged branch

    git branch --no-merged

Git safe branch delete

    git branch -d branchName

Git unsafe branch delete

    git branch -D branchName

Git delete remote branch

    git push -d origin branchName

Git create a remote branch

    git push origin <branch-name>

Git create a branch from a commit

    git checkout -b <new-branch-name> <commit-id>


### Replaceing master branch with another branch

```
git checkout master
git pull
git checkout ""another branch name""
git merge --allow-unrelated-histories -s ours master
git checkout master
git merge ""another branch name""
```

