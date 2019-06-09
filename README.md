# Git
- [Git Complex Tutorial](https://githowto.com/ru)
- [Resources to learn Git](http://try.github.io/)
- [Learn Git (branching)](https://learngitbranching.js.org/)
- [Git FAQ](https://github.com/k88hudson/git-flight-rules/blob/master/README_ru.md)
- [Git CheatSheet](https://services.github.com/on-demand/downloads/github-git-cheat-sheet/)
- [Git-flow cheatsheet](http://danielkummer.github.io/git-flow-cheatsheet/index.ru_RU.html)
- [Git-merge vs git-rebase](https://webdevkin.ru/posts/raznoe/izuchaem-git-merge-vs-rebase-dlya-nachinayushhix)
- [Git rebase and cherry-pick](https://toster.ru/q/28207)


# Git tweeks
- [Connecting to GitHub with SSH](https://help.github.com/en/articles/connecting-to-github-with-ssh)
- [Oh-my-git](https://github.com/arialdomartini/oh-my-git) - Awesome shell-theme for better git-cli experience (only for bash/zsh)
- [Git aliases for Bash terminal](https://github.com/sdcorp/dotfiles)
- [Git aliases for Fish terminal](https://github.com/jhillyerd/plugin-git)



## GitKraken
- [GitKraken Documentation](https://support.gitkraken.com)
- [GitKraken Cheat sheet](https://www.gitkraken.com/downloads/gitkraken-cheat-sheet-219.pdf)
- [GitKraken for GitHub Users Cheat Sheet](https://www.gitkraken.com/downloads/gitkraken-for-github-cheat-sheet-28sept2017.pdf)

## Commands

### Clone

#### Https

```
sh
git clone https://github.com/ashwanikumar04/git-cheatsheet.git
```

#### SSH

```
sh
git clone git@github.com:ashwanikumar04/git-cheatsheet.git

```
#### Single branch
Sometimes when the repository is very large, we only want to clone a single branch. Use below command to clone a single branch
```
sh
git clone git@github.com:ashwanikumar04/git-cheatsheet.git -b master --single-branch

```

### Config

The following command makes the output of git commands colorful.
```
sh
git config --global color.ui true
```

#### Local

```
sh
git config user.name "Ashwani Kumar"
git config user.email "ashwanikumar@test.com"
```

#### Global


```
sh
git config --global user.name "Ashwani Kumar"
git config --global user.email "ashwanikumar@test.com"
```

### Status

`git status` Shows the status with tracked and un-tracked files

### Add

```git add .``` Adds all the files in the current directory to staging.

```git add -A``` Adds all files in the current repository (even new files that are not yet tracked)

```git add -u```  Add all files that are already being tracked (ignore new files)

### Commit

`git commit -m "Add file to repository"` Commit staged files to the repository

`git commit --amend -m "New Message"` Changes the commit message for the last commit

`git commit -am "New Message"` Lets us add and commit all tracked, modified files in one step.

### Checkout

`git checkout -b <name_of_branch>` Create a branch and check it out in one step

`git branch <name_of_branch>` Create a branch, but stay in the current branch.

`git checkout <name_of_branch>` Check out an already created branch

`git branch` See a list of all branches, highlights the currently checked out branch

`git checkout master` Checkout master branch

`git branch -d <name_of_branch>` Remove branch locally, but only if we have merged branch.

`git branch -D <name_of_branch>` Remove branch even if we haven't merged changes.

### Stash

`git stash` Use this to stash all the changes to the current repository

`git stash apply` Use this to apply the last stash

### Push

`git push --set-upstream origin <branch>`
`git push`

### Pull

`git pull origin/master`
