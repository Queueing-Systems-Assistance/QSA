# Configuration

Perform the following commands in Windows:
```sh
git config --global user.name "your name"
git config --global user.email "your_email@epam.com"
```

Check if all was set correctly with:
```sh
git config --global -l
```

# Daily routine for feature branch

* May branch off from: __develop__
* Must create a merge request to the __develop__ branch
* Branch naming convention: `feature/QSA#****` (using the issue id)
* All branches should have an ISSUE ID

**Merge the upstream (usually the master) branch into your feature branch on a daily basis.** When the feature is done, merge the latest upstream branch into your branch before ask for a merge request. NEVER PUSH to the master branch.

### 1. Make your local master branch up to date
Note: you must not commit directly to master, so this must be a fast-forward
```sh
git checkout master
git pull
```

### 2. Create a new feature or bug branch and switch to there with one command
```sh
git checkout -b __branch-name-here__
```

Avoid various names/typos, capitalization. The ISSUE ID is starting with `(QSA: #***)` and a number found under the issue ticket, like [#1](https://github.com/Queueing-Systems-Assistance/qsa-application/issues/1). In this case the full id look like this: `(QSA: #1)`

### 3. Add new files to stage
```sh
git add .
```

### 4. See changes you're going to commit
```sh
git status
git diff --staged
```

### 5.Commit including issue feature/bug/... id
```sh
git commit -m "<meaingful comment> (QSA: #1)"
```
- Matches regex (if you're using commit-msg git hook): `\(QSA:[[:blank:]]#[0-9]{1,}\)`
- If you already made a commit, but you want to add more files to the commit:
  - Add the files to staging: `git add .`
  - Issue the following command:`git commit --amend --no-edit`
  - This will add the files to your last commit without modifying the message

### 6. If you want, push your changes to the feature branch to let others see/continue your work
```sh
git push -u origin
```

## When you are ready to merge your feature branch back to master

### 7. Make your feature branch up to date regarding master
```sh
git pull origin master
```

### 8. Push your feature branch to the remote repository when you have finished it
```sh
git push -u origin
```

### 9. Ask a pull request on the website into the master
After your request approved by Travis and there is no merge conflicts you can merge your branch 

### 10. Remove your local feature branch if it is not needed anymore
```sh
git branch -d __branch-name-here__
```
If you want to delete remote branch: 
```sh
git push origin --delete __branch-name-here__
```
