# Git - GitHub

## Most useful git commands
> `git init` - to initialize git

> `git add .` - add all files to staging
>
> `git add <fileName>` - To add specific Files

> `git status` - Get to know status of all files

> `git commit -m "message" ` - commit all staged code with "Message"

> `git push` - push commited code to GitHub
>
> `git push <origin> <branch>` - to push into specific branch
>
> `git push <origin> <branch> -f` - When remote has more commit than local repo, we have to fours push

> `git pull` - get latest code from remote repo

> `git clone <url>` - get all files from remote to your empty folder <url of repo>

> `git log` - Shows history of the project.

> `git stash` - save code without a commit
>
> `git stash pop` - to get all changes we saved
>
> `git stash clear` - to delete all those changes which are stashed

> `git fetch --all --prune` - This will fetch data of all Branches(--all) and even get deleted files (--prune)

> `git pull <upstream> <branch>` - This will also do the same as fetch

## Initialize username and password in Git
> `git config --global user.name <your_username>` - use it to set username
>
> `git config --global user.email <your_email>` - used to set email

## Remote Repository in Git
> `git remote add <origin> <url>` - This will connect local repo to GitHub, here you can name anything <anythingYouWant> to point to that specific URL
>
> `git remote add <upstream> <url>` - To add an upstream url (Url of original repo from which we have forked to our own account)
>
> `git remote -v` - show all repo connected to the folder

## Branch Commands in git
> `git branch <b-name>` - create branches

> `git checkout <b-name>` - switch branch
>
> `git checkout -b <b-name>` - To create and checkout branch at the same time

> `git merge <b-name>` - merge branches

> `git remote` - display all remote repo

> `git remote add <origin> <url>` - connect remote repo to local git

## Reset branch in Git
> [!CAUTION]
> `git reset` command are dangerous they can modify code base in suck a way you can undo it!

> `git reset <hasCode>` - Past the HasCode of the commit we want to restore
>
> `git reset --hard <hasCode>` - This will remove all changes and move to branch you put code of
>
> `git reset HEAD --hard` This will undo any changes you've made to track files and restore deleted files
>
> `git reset --hard <upstream> <branch>` This will reset head to match with the provided URL

> `git clean -fd` - This will delete any new files added since the last commit

> `git restore .` - Remove all changes you did after commit
>
> `git restore --staged <fileName>` - remove file from staged

## Rebase in Git
> `git rebase -i <hash of commit>` - This will open a window where we can pick a commit and squash(s) other commits into one single commit (Merge multiple commit into single commit). Check the description for more information

## Merge conflict in Git
> Merge conflict happens when two separate branches made change in the same file and also in the same lines... Then Git will get confused like which line changes should be taken... and we have to manually select whose(which branch) changes should stay...

## Git Ignore files
> `.ignore` - files & folders that should be ignored are named here
