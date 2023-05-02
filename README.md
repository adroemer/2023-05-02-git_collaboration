# 2023-05-02-git_collaboration

## Exercise 1

## Creating local repositories
- 'git clone <URL>' : "downloads the repository to the current directory
- 'git init' : initializes the current directory for Git

## Creating local branches

- 'git branch<name>' : creates a branch where HEAD is
- 'git branch -a':  list all the branches
- 'git switch <NAME>' : moves HEAD / switches your branch to <NAME>
- 'git checkout <NAME>': older way to switch branches

## Exercise #2
-create a branch 'branch_defs'
- edit README
    - 'git log --oneline --graph --all'
    - 'git push'
    - pull request
- add/commit changes
- push branch
- create the PR
-merge the PR
- sync our local 'main' with 'origin/main'
- 'fetch --prune'
- delete local branch

## Merging branches via PR

- 'git log --oneline --graph --all' : show you a decorated history
- 'git push  <REMOTE> <BRANCH': push a brnach to the remote, par attention to what branch you're working on

## cleaning up branches and saving history

- 'git fetch' updates the lit log / history
    - 'git fetch --prune': deletes any remote branches that were deleted
- 'git branch -d <NAME>': delete branch on your local machine

- pull request will auto update when you push the branch again

## Rebase

- 'git fetch --prune'
- 'git switch main'
- git pull origina main'
-'git switch <BRANCH>
- 'git rebase main':command to incorporate main into current branch

Code to simulate conflicts:

git checkout -b conflict_branch_1
echo "Changes to b1 commit 1" >> README.md
git status
git add README.md
git commit -m "b1 c1"
echo "Changes to b1 commit 2" >> README.md
git add README.md
git commit -m "b1 c2"

git checkout main

git checkout -b conflict_branch_2
echo "Changes to b2 commit 1" >> README.md
git add README.md
git commit -m "b2 c1"
echo "Changes to b2 commit 2" >> README.md
git add README.md
git commit -m "b2 c2"

git push origin conflict_branch_2
git push origin conflict_branch_1










Changes to b2 commit 1
Changes to b2 commit 2
