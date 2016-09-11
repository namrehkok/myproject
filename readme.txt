@AA

https://www.digitalocean.com/community/tutorials/how-to-use-git-branches

viewing branches:
git branch -a

To create a new branch, named develop, type the following:
git checkout -b develop

Changing branch
git checkout branch

Adding files
git add filename

Commiting changes
git commit -am "whatever"

merging code
Run this in the branch you want to merge with
git merge develop

Pushing changes to git:
git push -u origin development

Getting up to date with the stuff on git:
git stash --include-untracked
git pull
Later you can clean the stash history.
Manually, one-by-one:

$ git stash list
stash@{0}: WIP on <branch>: ...
stash@{1}: WIP on <branch>: ...

$ git stash drop stash@{0}
$ git stash drop stash@{1}
Brutally, all-at-once:

$ git stash clear
Of course if you want to go back to what you stashed:

$ git stash list
...
$ git stash apply stash@{5}

editing the URL:
git remote set-url origin https://github.com/namrehkok/notes.git
