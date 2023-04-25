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

```



5 What is the difference between a git merge and a git rebase?

6 What command would you use to fix a broken commit?

7 How do you revert a commit that has been pushed and made public?

8 What is Git squash?

9  What are the two steps performed by a git pull?

10  What is the difference between a git pull and a get fetch?

11  How do you remove a file from Git w/o removing it from your filesystem?

12  What is a merge conflict? How can you resolve it?