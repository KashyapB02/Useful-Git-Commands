<h1 align="center">Git Commands</h1>

<h5>

```
1. git config

Usage: git config –global user.name “[name]”  
Usage: git config –global user.email “[email address]”

This command sets the author name and email address respectively to be used with your commits.
```
 
```
2. git init

Usage: git init [repository name]
This command is used to start a new repository.
```

```
3. git clone

Usage: git clone [url]  
This command is used to obtain a repository from an existing URL.
```

```
4. git add

Usage: git add [file]  
This command adds a file to the staging area.
 
Usage: git add *  
This command adds one or more to the staging areas.
```

```
5. git commit

Usage: git commit -m “[ Type in the commit message]”  
This command records or snapshots the file permanently in the version history.

Usage: git commit -a  
This command commits any files you’ve added with the git add command and also commits any files you’ve changed since then.
``` 

```
6. git diff

Usage: git diff  
This command shows the file differences which are not yet staged.
 
Usage: git diff –staged 
This command shows the differences between the files in the staging area and the latest version present.

Usage: git diff [first branch] [second branch]  
This command shows the differences between the two branches mentioned.
```

```
7. git reset

Usage: git reset [file]  
This command unstages the file, but it preserves the file contents.

Usage: git reset [commit]  
This command undoes all the commits after the specified commit and preserves the changes locally.

Usage: git reset –hard [commit]
This command discards all history and goes back to the specified commit.
```

```
8. git status

Usage: git status  
This command lists all the files that have to be committed.
``` 

```
9. git rm

Usage: git rm [file]  
This command deletes the file from your working directory and stages the deletion.
```

```
10. git log

Usage: git log  
This command is used to list the version history for the current branch.

Usage: git log –follow[file]  
This command lists version history for a file, including the renaming of files also.
```

```
11. git show

Usage: git show [commit]  
This command shows the metadata and content changes of the specified commit.
``` 

```
12. git tag

Usage: git tag [commitID]  
This command is used to give tags to the specified commit.
```

```
13. git branch

Usage: git branch  
This command lists all the local branches in the current repository.
 
Usage: git branch [branch name]  
This command creates a new branch.

Usage: git branch -d [branch name]  
This command deletes the feature branch.
```

```
14. git checkout

Usage: git checkout [branch name]  
This command is used to switch from one branch to another.

Usage: git checkout -b [branch name]  
This command creates a new branch and also switches to it.
```

```
15. git merge

Usage: git merge [branch name]  
This command merges the specified branch’s history into the current branch.
```

```
16. git remote

Usage: git remote add [variable name] [Remote Server Link]  
This command is used to connect your local repository to the remote server.
```

```
17. git push

Usage: git push [variable name] master  
This command sends the committed changes of master branch to your remote repository.

Usage: git push [variable name] [branch]  
This command sends the branch commits to your remote repository.

Usage: git push –all [variable name]  
This command pushes all branches to your remote repository.

Usage: git push [variable name] :[branch name]  
This command deletes a branch on your remote repository.
```


```
18. git fetch

Usage: git fetch [remote]  
Fetch all of the branches from the repository & downloads all of the required commits and files from the other repository.

Usage: git fetch [remote] [branch] 
Fetch the specified branch from the repository.

Usage: git fetch --all
usage: git fetch --all --prune

Fetches all registered remotes and all their branches.
```

```
19. git pull

Usage: git pull [Repository Link]  
This command fetches and merges changes on the remote server to your working directory.
```

```
20. git stash

Usage: git stash save  
This command temporarily stores all the modified tracked files.

Usage: git stash pop  
This command restores the most recently stashed files.

Usage: git stash list  
This command lists all stashed changesets.

Usage: git stash drop  
This command discards the most recently stashed changeset.
``` 

```
21. git reset

usage: git reset [file]
Remove the specified file from the staging area, but leave the working directory unchanged.

usage: git reset
Reset the staging area to match the most recent commit, but leave the working directory unchanged.

usage: git reset [remote/branch]
Reset the working directory exactly the same as remote/branch.

usage: git reset --hard
Reset the staging area and the working directory to match the most recent commit.
```

</h5><hr>
