# My global GIT Hooks

These are helper hooks that are intended to be installed by git whenever I initialize a git repo

## How to install:
1. Clone repository into your home path with the directory name `.git-templates`
```
  git clone [repo url] ~/.git-templates
```

2. run the following git init command
```
  git config --global init.templatedir '~/.git-templates'
```
  - This will tell your global git that you have a config directory with templates for the git hooks. Whenever you initialize a repo, or reinitialize a repo with `git init` then it will copy these hooks if they do not already exist into your repo's `.git/hooks` directory
  - If there is already a hook in that directory, then the git hook will not be copied

## What to do if you already have git repos but you want to copy the new hooks

Simple. Just cd into the repo and reinitialize the repo with `git init`
