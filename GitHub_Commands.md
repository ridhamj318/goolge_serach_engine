# Common Git Commands.

-----------

### Make directory a Git repository

* This is the first step in creating a repository. After running git init,
  adding and committing files/directories is possible.

* It will create a hidden .git file.

* Command : **git init**

### To add files in the to the staging area for Git.

* Command : **git add <file name>**

### Git Commit Record the changes made to the files to a local repository.

* Command : **git commit -m <comment in quotos>**

### Git Status

*  If a file is in the staging area, but not committed, it shows with git status.

* Command : **git status**

### Git Config

* It is used to see the configurations of GitHub.

* Command : **git config**

### Git Branch

* To determine what branch the local repository is on, add a new branch, or delete a branch.

**Create a new branch**

* Command : **git branch <branch_name>**

**List all remote or local branches**

* Command : **git branch -a**

**Delete a branch**

* Command : **git branch -d <branch_name>**

### Git Checkout

* To start working in a different branch, use git checkout to switch branches.

**To see branch**

* Command : **git checkout**

**Checkout an existing branch**

* Command : **git checkout <branch_name>**

**Checkout and create a new branch with that name**

* Command : **git checkout -b <new_branch>**

### Git Merge

* git merge combines the changes from one branch to another branch.

**Merge changes into current branch**

* Command : **git merge <branch_name>**

### Git Remote 

* To connect a local repository with a remote repository.

* A remote repository can have a name set to avoid having to remember the URL of the repository.

**Add remote repository**

* Command :  **git remote <command> <remote_name> <remote_URL>**

**List named remote repositories**

* Command : **git remote -v**

### Git Clone

* To create a local working copy of an existing remote repository, use git clone to copy and download the repository to a computer. 

* Git will create a directory locally with all files and repository history.

* Command : **git clone <remote_URL>**

### Git Push 

* Sends local commits to the remote repository. 

* git push requires two parameters: the remote repository and the branch that the push is for.

* Command : **git push <remote_URL/remote_name> <branch>**

**Push all local branches to remote repository**

* Command : **git push —all**

### Git Pull

* To get the latest version of a repository run git pull. 

*  This pulls the changes from the remote repository to the local computer.

* Command : **git pull <branch_name>**

### Git Diff

* Diffing is a function that takes two input datasets and outputs the changes between them. 

* Command : **git diff<file name>**

### Git restore

* Use this command For resort file.

* Command : **git restore <file name>**

### Git Fetch

* When we use the command git fetch, Git gathers any commit from the target branch that does not exist in our current branch and stores it in our local repository. 

* However, it does not merge it with our current branch.

* Command : **git fetch**

### Git Reset

* We use this command to return the entire working tree to the last committed state.

* This will discard commits in a private branch or throw away the uncommitted changes.

* Command : **git reset –hard**

### Git Stash

* To save changes made when they’re not in a state to commit them to a repository.

* This will store the work and give a clean working directory.

* For instance, when working on a new feature that’s not complete, but an urgent bug needs attention.

**Store current work with untracked files**

* Command : **git stash -u**

**Bring stashed work back to the working directory**

* Command :  **git stash pop**

### Git Log

* To show the chronological commit history for a repository. 

* This helps give context and history for a repository. 

 **Show entire git log**

* Command : **git log**

 **Show git log with date pameters**

* command : **git log --<after/before/since/until>=<date>**

 **Show git log based on commit author**

* Command : **git log --<author>="Author Name"**

### Git rm

* Remove files or directories from the working index (staging area).

* Running the command with force deletes the file

* The cached command removes the file from the working index.

 **To remove a file from the working index (cached)**

* Command : **git rm --cached <file name>**

 **To delete a file (force)**

* Command : **git rm -f <file name>**

 **To remove an entire directory from the working index (cached)**

* Command : **git rm -r --cached <directory name>**

 **To delete an entire directory (force)**

* Command : **git rm -r -f <file name>**

