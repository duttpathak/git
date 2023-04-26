1 What is Git? Explain it in as much detail as possible.

Git is a version control system used for tracking changes in computer files. It is generally used for source code management in software development. 

The Git workflow is divided into three states:

```
Working directory - Modify files in your working directory

Staging area (Index) - Stage the files and add snapshots of them to your staging area

Git directory (Repository) - Perform a commit that stores the snapshots permanently to your Git directory. Checkout any existing version, make changes, stage them and commit.
```

Branch in Git is used to keep your changes until they are ready. You can do your work on a branch while the main branch (master) remains stable. After you are done with your work, you can merge it with the main office.

 
2 What programming language is Git written in?

Primarily wirtten in C and programming scripts written in shell script, perl, and python. 

3 Provide five examples of a platform which uses Git?

```
Bitbucket 
GitLab
Perforce
Beanstalk
Codebase

```


4 Explain five common Git commands and their usage. 

```
Create Repositories
git init #initialized empty git repository under user

Make Changes
$ git add 
$ git commit #commit to the changes made. 
$ git status 

Sync Repositories
$ git push #push changes made
$ git pull #pull repository from github 
$ git add origin #add the url of the repository created to push changes. 


used to add a new remote:
$ git remote add origin git@github.com:User/UserRepo.git

used to change the url of an existing remote repository:
$ git remote set-url origin git@github.com:User/UserRepo.git

A power user shortcut command that combines the -a and -m options. This combination immediately creates a commit of all the staged changes and takes an inline commit message.
$ git commit -am "commit message"


```


5 What is the difference between a git merge and a git rebase?

Git merge and Git rebase commands are used to combine the work of multiple developers in one code. 

To understand git merge, the git branch needs to be understood first. There is a main branch and featured branch. Let's say that you want your code in a new place and not visible on the master branch. You put it in feature branch. On the main branch the commit changes of the feature branch are not there, so git merge is used to see the commited changes of the feature branch on the master branch. 

Git rebase is similar to git merge, except the featured branches will not be merged, but they will be rebased as seprate commits. Git rebase is eaiser to see, because the logs are linear and it's easy to move through the project.   

6 What command would you use to fix a broken commit?

```
$ git commit --amend
then use 
$ git rebasse --continue #lets git continue with the rebase operation
```

7 How do you revert a commit that has been pushed and made public?

```
$ git revert 
```


8 What is Git squash?

Git squash is a way to rewrite your commit history; this action helps to clean up and simplify your commit history before sharing your work with a team. 

9  What are the two steps performed by a git pull?

Git pull will fetch and replay the changes from the remote maain branch since it diverged from the local master until its current commit on top of master and record the result in a new commit along with the names of the two parent commits and a log message from the user describing the changes. 

10  What is the difference between a git pull and a git fetch?

Git pull command downloads the changes directly and then applies those changes to the current working files. The git fetch command does not change or manipulate or spoil the data of the remote repository. 

Git pull pulls all the changes from the remote repository to corresponding branch of the local repository. The git fetch changes from the remote repository and then stores the changes in a separate branch in local repository. 

Git pull updates the current HEAD of teh current branch with the latest changes of the remote branch and the git fetch downloads the new changes from remote server. 

11  How do you remove a file from Git w/o removing it from your filesystem?

```
$ git rm --cached

```

12  What is a merge conflict? How can you resolve it?

When there are two commits, merge conflict is where git is unable to automatically resolve differences in code. Git only merges the changes automatically only if the commits are on different lines or branches. 

```
The easiest way to resolve a conflicted file is to open it and make any necessary changes
After editing the file, we can use the git add a command to stage the new merged content
The final step is to create a new commit with the help of the git commit command
Git will create a new merge commit to finalize the merge

```