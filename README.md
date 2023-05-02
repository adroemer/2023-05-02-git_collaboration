# 2023-05-02-git_collaboration

##
- 'git clone <URL>' : "downloads the repository to the current directory
- 'git init' : initializes the current directory for Git

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











