# Git-and-GitHub
## Git Commands
This project provides basic and advanced concepts of Git and GitHub. Git is the version control system allows us to monitor and work together with our team members at the same workspace.

#### Features of Git
* **Scalable**
Git is scalable, which means when the number of users increases, the Git can easily handle such situations.
* **Distributed**
One of Git's great features is that it is distributed, we can create a "clone" of the entire repository rather switching the project to another machine
* **Security**
Files and commits are checked and retrieved by its checksum at the time of checkout. It stores its history in such a way that the ID of particular commits depends upon the complete development history leading up to that commit. So Git is secure. 
* **Speed**
Git is very fast, It has a centralized version control system continually communicates with a server somewhere.Fetching version history from a locally stored repository is much faster than fetching it from the remote server.
* **Supports non-linear development**
Git supports seamless branching and merging, which helps in visualizing and navigating a non-linear development. A branch in Git represents a single commit. We can construct the full branch structure with the help of its parental commit.
* **Branching and Merging**
Git allows the creation of multiple branches without affecting each other. We can perform tasks like creation, deletion, and merging on branches.
* **Data Assurance**
The Git data model ensures the cryptographic integrity of every unit of our project. It provides a unique commit ID to every commit through a SHA algorithm. We can retrieve and update the commit by commit ID. Most of the centralized version control systems do not provide such integrity by default.

#### Git Terminology
* **Branch**
A branch is a version of the repository that diverges from the main working project.A Git project can have more than one branch.
* **Checkout**
Checkout is used for the act of switching between different versions of a target entity.
* **Cherry-Picking**
To apply some commit from one branch into another branch.
* **Clone**
It is used to make a copy of the target repository or clone it.
* **Fetch**
It is used to fetch branches and tags from one or more other repositories, along with the objects necessary to complete their histories.
* **HEAD**
HEAD is the representation of the last commit in the current checkout branch. We can think of the head like a current branch. When you switch branches with git checkout, the HEAD revision changes, and points the new branch.
* **Index**
The Git index is a staging area between the working directory and repository.
* **Master**
Master is a naming convention for Git branch.After cloning a project from a remote server, the resulting local repository contains only a single local branch. This branch is called a "master" branch. It means that "master" is a repository's "default" branch.

* **Merge**
Merging is a process to put a forked history back together. It takes the data created by git branch and integrate them into a single branch.

* **Origin**
It is a reference to the remote repository from a project was initially cloned. 

* **Pull**
The term Pull is used to receive data from GitHub. It fetches and merges changes on the remote server to your working directory.

* **Pull requests**
Pull requests are a process for a developer to notify team members that they have completed a feature. Once their feature branch is ready, the developer files a pull request via their remote server account. Pull request announces all the team members that they need to review the code and merge it into the master branch.

* **Push**
The push term refers to upload local repository content to a remote repository. Pushing is capable of overwriting changes; caution should be taken when pushing.

* **Rebase**
Rebase is referred to as the process of moving or combining a sequence of commits to a new base commit.

* **Remote**
Remote is concerned with the remote repository. It is a shared repository that all team members use to exchange their changes. 

* **Repository**
It contains the collection of the file as well as the history of changes made to those files. Repositories in Git is considered as your project folder. A repository has all the project-related data.

* **Stashing**
The git stash command enables you to switch branch without committing the current branch.

* **Tag**
Tags make a point as a specific point in Git history. It is used to mark a commit stage as important. 

* **Git Revert**
Revert is used to revert some commit. To revert a commit, git revert command is used. It is an undo type command. 

* **Git Reset**
Reset stands for undoing changes. The git reset command is used to reset the changes. The git reset command has three core forms of invocation. These forms are as follows.
  * Soft
  * Mixed
  * Hard

* **Git Ignore**
Ignore used to specify intentionally untracked files that Git should ignore. It doesn't affect the Files that already tracked by Git.

* **Git Diff**
It runs a diff function on Git data sources. These data sources can be files, branches, commits, and more. It is used to show changes between commits, commit, and working tree, etc.

* **Git Squash**
Squash is used to squash previous commits into one. It is technique to group-specific changes before forwarding them to others. You can merge several commits into a single commit with the powerful interactive rebase command.

* **Git Rm**
In Git, the term rm stands for remove. It is used to remove individual files or a collection of files. The key function of git rm is to remove tracked files from the Git index. 

#### GitHub
GitHub is a Git repository hosting service. GitHub also facilitates with many of its features, such as access control and collaboration. It provides a Web-based graphical interface. GitHub is a place where programmers and designers work together. They collaborate, contribute, and fix bugs together.

#### Git config command
| Command    |Description               | Example / Syntax|
| ------------   | ------------               |---- |
|  git config   | The Git config command is the first and necessary command used on the Git command line. This command sets the author name and email address to be used with your commits. | ```$ git config --global user.name "user_name"  ``` <br />  ``` $ git config --global user.email "someuser@gmail.com" ```  |

#### Getting & Creating Projects
| Command    |Description               | Example /Syntax|
| ------------   | ------------               | ---|
| git init	 |Initialize/create a local repository. The init command will initialize an empty repository | ```$ git init Sample_Repo ```   |
| git clone | Create a local copy of a remote repository. It used to make a copy of a repository from an existing URL |``` $ git clone URL ``` |

#### Basic Snapshotting
| Command    |Description               | Example /Syntax|
| ------------   | ------------               | ----|
| git status	 | Check status |  ```$ git status  ```|
| git add  | [file-name.txt]	Add a file to the staging area |``` $ git add Filename   ``` OR <br />  ``` $ git add all  ``` |
| git add-A |  	Add all new and changed files to the staging area |```  $ git add -A ```  |
| git commit -m  |"[commit message]"	Commit changes |```  $ git commit -m " Commit Message"  ```  |
| git rm -r  |[file-name.txt]	Remove a file (or folder) | ```  $ git rm <file Name>  ``` |

#### Branching & Merging
| Command    |Description               | |
| ------------   | ------------               |------ |
| git branch	List branches (the asterisk denotes the current branch) |``` $ git branch  ```  |
| git branch -a	List all branches (local and remote) | | 
| git branch [branch name]	Create a new branch | |
| git branch -d [branch name]	Delete a branch |```  git branch -d ``` |
| git checkout -b [branch name]	Create a new branch and switch to it | |
| git checkout -b [branch name] origin/[branch name]	Clone a remote branch and switch to it | |
| git branch -m [old branch name] [new branch name]	Rename a local branch | ``` git branch -m ``` |
| git checkout [branch name]	Switch to a branch | |
| git checkout -	Switch to the branch last checked out | |
| git checkout -- [file-name.txt]	Discard changes to a file | |
| git merge [branch name]	Merge a branch into the active branch | ``` $ git merge BranchName ```  |
| git merge [source branch] [target branch]	Merge a branch into a target branch | |
| git stash	Stash changes in a dirty working directory | |
| git stash clear	Remove all stashed entries | |

#### Sharing & Updating Projects
| Command    |Description               | |
| ------------   | ------------               |----- |
| git push origin [branch name]	Push a branch to your remote repository |```$ git push [variable name] master ```  |
| git push -u origin [branch name]	Push changes to remote repository (and remember the branch) | |
| git push	Push changes to remote repository (remembered branch) | |
| git push origin --delete [branch name]	Delete a remote branch | |
| git pull	Update local repository to the newest commit |``` $ git pull URL ``` |
| git pull origin [branch name]	Pull changes from remote repository | |
| git remote add origin ssh://| git@github.com/[username]/[repository-name].git	Add a remote repository
| git remote set-url origin ssh://git@| github.com/[username]/[repository-name].git	Set a repository's origin branch to SSH | |

#### Inspection & Comparison
| Command    |Description               | |
| ------------   | ------------               | ----|
| git log	View changes  |```$ git log ``` |
| git log --summary	View changes (detailed) | |
| git log --oneline	View changes (briefly) | |
| git diff [source branch] [target branch]	Preview changes before merging |```  $ git diff [source branch] [target branch]``` |
