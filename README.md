<h1 align="center">Git Commands</h1>

<h4>1. Setup user name and user email</h4>

- User name  : `git config --global user.name "user name"`<br>
- User email : `git config --global user.email "userEmailID"`

<h2></h2>

<h4>2. View user name and user email</h4>

- User name  : `git config --global user.name`<br>
- User email : `git config --global user.email`

<h2></h2>

<h4>3. Cache login credentials (It helps to avoid re-typing the username and password everytime you perform a commit)</h4>

- `git config --global credential.helper cache`

<h2></h2>

<h4>4. Obtain a repository from an existing URL</h4>

- `git clone URLofRepository`

<h2></h2>

<h4>5. Initialize an empty git repository</h4>

- Initialize git in existing folder : `git init`
- Initialize git with new folder : `git init folderName`

<h2></h2>

<h4>6. Adding files to staging area</h4>

- Adding a single file : `git add fileName`
- Adding all files : `git add .` 

<h2></h2>

<h4>7. Check repository status</h4>

- `git status` 

<h2></h2>

<h4>8. Commit changes with commit message</h4>

- Single line message : `git commit -m "Short summery about commit"`
- Complete commit message : `git commit` 

<h2></h2>

<h4>9. View commit history with changes</h4>

- List of newest commits : `git log`
- Detailed changes of each file : `git log -p` 

<h2></h2>

<h4>10. View a particular commit</h4>

- `git show commitID`
- `git show commitHash`

<h2></h2>

<h4>11. View changes before commiting</h4>

- Unstaged changes : `git diff`
- Staged changes : `git diff --staged`
- Changes of a specific file : `git diff fileName`

<h2></h2>

<h4>12. Remove tracked files from the current working tree</h4>

- Remove a single file : `git rm fileName` or `git rm directoryName/fileName`
- Remove files with a particular extension : `git rm *.extensionName` or `git rm directoryName/*.extensionName`
- Remove file only from VCS : `git rm --cached fileName` or `git rm directoryName/fileName`

> <i>Note : First two commands will also remove the files from the local system.</i>

<h2></h2>

<h4>13. Rename files</h4>

- `git mv oldFileName newFileName`

<h2></h2>

<h4>14. Move files</h4>

- `git mv sourceDirectoryName/fileName destinationDirectoryName`

> <i>Note : Executing the above command will move the source into the destination directory. The source must exists and can be a file, or a directory and the destination must be an existing directory.</i>

<h2></h2>

<h4>15. Revert unstaged changes staged changes</h4>

- Restore a unstaged working tree files : `git checkout fileName`
- Restore a staged working tree file : `git reset HEAD fileName`
- Restore all staged files : `git reset HEAD`

<h2></h2>

<h4>16. Amend the most recent commit</h4>

- Update the most recent commit : `git commit --amend -m "Updated message for the most recent commit."`
- Commit more files to most recent commit : `git add fileName` then `git commit --amend --no-edit`

<h2></h2>

<h4>17. Rollback last commit</h4>

- `git revert HEAD`

<h2></h2>

<h4>18. Rollback a particular commit</h4>

- `git revert commitID`
- `git revert commitHash`

<h2></h2>

<h4>19. Creat and switch to a new branch</h4>

- Only create a new branch : `git branch newbranchName`
- Create and switch to a new branch : `git branch -b newBrachName`

<h2></h2>

<h4>20. View list of all branches</h4>

- List all branch : `git branch`
- List all remote branches : `git branch -a`

<h2></h2>

<h4>21. Delete branch</h4>

- Normally delete a branch : `git branch -d branchName`
- Forcibly delete a branch : `git branch -D branchName`
- Delete a remote branch : `git push origin --delete branchName`

<h2></h2>

<h4>22. Merge two branches</h4>

- Normally merge a branch : `git merge -d branchName`
- Merge a branch with a merge commit : `git merge --no-ff branchName`

<h2></h2>

<h4>23. Show commit log as graph for current or all branches</h4>

- Commit log of current branch : `git log --graph --oneline --decorate`
- Commit log of all branches : `git log --all --graph --oneline --decorate`

> <i>Note : The `--graph` option will draw an ASCII graph, which represents the branch structure of the commit history. When it used in association with the `--oneline` and
> `--decorate` flags, it makes it easier to identify which commit belongs to which branch.</i>

<h2></h2>

<h4>24. Abort a conflicting merge</h4>

- `git merge --abort`

<h2></h2>

<h4>25. Add a remote repository</h4>

- Origin repositories : `git remote add origin URLofRepository`
- Upstream repositories : `git remote add upstream URLofRepository`

<h2></h2>

<h4>26. View remote URLs</h4>

- `git remote -v`

<h2></h2>

<h4>27. Get additional information about a remote repository</h4>

- Origin repositories : `git remote show origin`
- Upstream repositories : `git remote show upstream`

<h2></h2>

<h4>28. Push changes to a remote repository</h4>

- `git push origin branchNametobePushed`

<h2></h2>

<h4>29. Pull changes from a remote repository</h4>

- `git pull`
- `git pull --verbose`

<h2></h2>

<h4>30. Merge remote repository with local repository</h4>

- `git merge origin`

<h2></h2>

<h4>31. Push a new branch to remote repository</h4>

- `git push -u origin newBranchName`

<h2></h2>

<h4>32. Remove a remote branch</h4>

- `git push --delete origin branchName`

<h2></h2>

<h4>33. Use rebase</h4>

- `git rebase branchName`

> <i>Note : The above command will change the base of your branch from one commit to another, which will make it appear as if you have created your branch from a different commit.</i>

<h2></h2>
