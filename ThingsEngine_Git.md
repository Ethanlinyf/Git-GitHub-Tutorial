
# Table of Contents

1.  [Primer](#orgbc622ae)
    1.  [What is Version Control](#org296f8cd)
    2.  [Team Work](#org482e0c7)
        1.  [centralized & distributed](#org90046fd)
2.  [Git Introduction](#org4601817)
    1.  [What is Git](#orgfe1ba30)
        1.  [Performance](#org18e8443)
        2.  [Security](#org691dd8f)
        3.  [Flexibility](#orgad57dce)
    2.  [History](#orgab54d9a)
    3.  [Culture](#orgcd1a436)
    4.  [Installation of Git](#orgeb8e2b0)
        1.  [Install Git on Mac OS X](#orge6729e8)
        2.  [Install Git on Windows](#orgf7bfdcb)
        3.  [Install Git on Linux](#org139c6e1)
        4.  [Configure your Git username and email](#org056b858)
3.  [Getting Started](#org2420ac0)
    1.  [Basic settings](#orgbd50196)
    2.  [Initialize a repository](#org60dadcd)
4.  [Remote Repository at GitHub](#org4164d22)
5.  [Advanced Topic](#orgb1ef77a)
    1.  [Branch Management](#orgdfaf64c)
        1.  [What is a branch](#org023a798)
        2.  [Common operations of branches](#org0db3995)
        3.  [Git Flow, teamwork based on branches](#org6a70ba2)
    2.  [Bookmark Management](#org1392ad8)
    3.  [Customization](#org2e3543e)
6.  [Magit Tutorial](#org5dcec22)
    1.  [Basic magit](#orgc0e74e6)
        1.  [Create a git repo](#org7cad0a3)
        2.  [Clone a repo](#org7e375b0)
        3.  [Check the status of your repo](#orgf48368c)
        4.  [Stage a file](#orgcb5d751)
        5.  [Commit a file](#org748325f)
        6.  [Diffs](#org709ed5e)
        7.  [See the log](#orgff0beb6)
        8.  [Push](#orgd83ca2a)
        9.  [Pull](#org53afa0f)
        10. [Run a command-line git command manually](#org157b9de)
        11. [Check the output of the git command](#org71f1875)
        12. [Keybindings](#orgf68ab5f)
    2.  [Intermediate concepts](#orga33c943)
        1.  [Checkout an older version of a file](#orgb8378a0)
        2.  [Search the commit messages for a pattern](#orgb6f2a45)
        3.  [Revert a commit](#org462c89f)
        4.  [Tag a version](#org686c873)
        5.  [Checkout an existing branch.](#orgb0332c4)
        6.  [Merge two branches](#org542818d)
        7.  [Resolving conflicts](#orgc6db71a)
        8.  [Fetching](#org93b76fd)
        9.  [Add a remote](#orgecf9064)
        10. [Stashing](#orgc0366dc)
        11. [Git blame](#org8fa58b8)
    3.  [Advanced concepts](#org67eaeb9)
        1.  [Resetting](#orga48082a)
        2.  [Rebasing](#orgc40f7c4)
        3.  [Create patches](#org38f7120)
        4.  [Cherry-picking](#org5d2740f)
        5.  [Apply patches](#orge7f5e22)
        6.  [Notes about commits](#org79a8f79)
        7.  [Cherry-picking](#org076f025)
7.  [Test](#orgec06ce5)



<a id="orgbc622ae"></a>

# Primer


<a id="org296f8cd"></a>

## What is Version Control

Version control systems are a category of software tools that help a software team manage changes to source code over time. Version control software keeps track of every modification to the code in a special kind of database. If a mistake is made, developers can turn back the clock and compare earlier versions of the code to help fix the mistake while minimizing disruption to all team members.

For almost all software projects, the source code is like the crown jewels - a precious asset whose value must be protected. For most software teams, the source code is a repository of the invaluable knowledge and understanding about the problem domain that the developers have collected and refined through careful effort. Version control protects source code from both catastrophe and the casual degradation of human error and unintended consequences.

Software developers working in teams are continually writing new source code and changing existing source code. The code for a project, app or software component is typically organized in a folder structure or "file tree". One developer on the team may be working on a new feature while another developer fixes an unrelated bug by changing code, each developer may make their changes in several parts of the file tree.

Version control helps teams solve these kinds of problems, tracking every individual change by each contributor and helping prevent concurrent work from conflicting. Changes made in one part of the software can be incompatible with those made by another developer working at the same time. This problem should be discovered and solved in an orderly manner without blocking the work of the rest of the team. Further, in all software development, any change can introduce new bugs on its own and new software can't be trusted until it's tested. So testing and development proceed together until a new version is ready.

Good version control software supports a developer's preferred workflow without imposing one particular way of working. Ideally it also works on any platform, rather than dictate what operating system or tool chain developers must use. Great version control systems facilitate a smooth and continuous flow of changes to the code rather than the frustrating and clumsy mechanism of file locking - giving the green light to one developer at the expense of blocking the progress of others.

Software teams that do not use any form of version control often run into problems like not knowing which changes that have been made are available to users or the creation of incompatible changes between two unrelated pieces of work that must then be painstakingly untangled and reworked. If you're a developer who has never used version control you may have added versions to your files, perhaps with suffixes like "final" or "latest" and then had to later deal with a new final version. Perhaps you've commented out code blocks because you want to disable certain functionality without deleting the code, fearing that there may be a use for it later. Version control is a way out of these problems.

Version control software is an essential part of the every-day of the modern software team's professional practices. Individual software developers who are accustomed to working with a capable version control system in their teams typically recognize the incredible value version control also gives them even on small solo projects. Once accustomed to the powerful benefits of version control systems, many developers wouldn't consider working without it even for non-software projects.


<a id="org482e0c7"></a>

## Team Work


<a id="org90046fd"></a>

### centralized & distributed


<a id="org4601817"></a>

# Git Introduction


<a id="orgfe1ba30"></a>

## What is Git

[Git](https:/en.wikipedia.org) is a distributed version-control system for tracking changes in source code during software development. 
It is designed for coordinating work among programmers, but it can be used to track changes in any set of files. 
Its goals include speed, data integrity, and support for distributed, non-linear workflows.
Git is free and open-source software distributed under the terms of the GNU General Public License version 2.


<a id="org18e8443"></a>

### Performance


<a id="org691dd8f"></a>

### Security


<a id="orgad57dce"></a>

### Flexibility


<a id="orgab54d9a"></a>

## History

Git was created by Linus Torvalds in 2005 for development of the Linux kernel, with other kernel developers contributing to its initial development. Its current maintainer since 2005 is Junio Hamano.


<a id="orgcd1a436"></a>

## Culture


<a id="orgeb8e2b0"></a>

## Installation of Git


<a id="orge6729e8"></a>

### Install Git on Mac OS X

There are several ways to install Git on a Mac. In fact, if you've installed XCode (or it's Command Line Tools), Git may already be installed. To find out, open a terminal and enter git &#x2013;version.

    git --version

-   Git for Mac Installer
    the latest [Git for Mac installer](https://sourceforge.net/projects/git-osx-installer/files/).
-   Install Git with Homebrew

    brew install git


<a id="orgf7bfdcb"></a>

### Install Git on Windows

The latest Git for [Windows installe](https://gitforwindows.org/).


<a id="org139c6e1"></a>

### Install Git on Linux

-   Debian / Ubuntu

    sudo apt-get update
    sudo apt-get install git


<a id="org056b858"></a>

### Configure your Git username and email

Configure your Git username and email using the following commands, replacing "Your name" with your own. These details will be associated with any commits that you create:

    git config --global user.name "Your name"
    git config --global user.email "Your email address"


<a id="org2420ac0"></a>

# Getting Started


<a id="orgbd50196"></a>

## Basic settings

$ git config &#x2013;global user.name "Your Name"
$ git config &#x2013;global user.email "youremail@example.com"


<a id="org60dadcd"></a>

## Initialize a repository

-   create a folder for testing

    mkdir learngit
    cd learngit
    pwd 

-   initialize a repository

    git init

Initialized empty Git repository in *Users/ethanlin/Documents/ThingsEngine/ThingsEngine-Git*.git/

-   add a file name readme.md

"Git is a version control system.
Git is free software." in readme.md

-   add and commit

    git add readme.txt
    
    git commit -m "create a readme file"

[master (root-commit) eaadf4e] wrote a readme file
 1 file changed, 2 insertions(+)
 create mode 123456 readme.md

-   add more files

    touch file1.txt file2.txt file3.txt

    git add file1.txt
    git add file2.txt file3.txt

    git commit -m "add 3 files"

-   adjustment for readme.md

"Git is a distributed version control system.
Git is free software."

-   git status

    git status

On branch master
Changes not staged for commit:
  (use "git add <file>&#x2026;" to update what will be committed)
  (use "git checkout &#x2013; <file>&#x2026;" to discard changes in working directory)
 
	modified:   readme.txt
 
no changes added to commit (use "git add" and/or "git commit -a")

-   git diff

    git diff readme.md

diff &#x2013;git a/readme.md b/readme.md
index 46d49bf..9247db6 100644
&#x2014; a/readme.md
<del>+</del> b/readme.md
@@ -1,2 +1,2 @@
-Git **is** a version control system.
+Git **is** a distributed version control system.
 Git **is** free software.

-   update readme.md, new version

    git add readme.md

    git status

On branch master
Changes to be committed:
  (use "git reset HEAD <file>&#x2026;" to unstage)
 
    modified:   readme.md

    git commit -m "add distributed"

[master e475afc] add distributed
 1 file changed, 1 insertion(+), 1 deletion(-)

    $ git status

On branch master
nothing to commit, working tree clean


<a id="org4164d22"></a>

# Remote Repository at GitHub

    ssh-keygen -t rsa -C "youremail@example.com"

You could find a directory .ssh in your home folder. id<sub>rsa</sub> and **id<sub>rsa.pub</sub>**


<a id="orgb1ef77a"></a>

# Advanced Topic


<a id="orgdfaf64c"></a>

## Branch Management

Compared with SVN, one of the specific features Git has is about branch. 

Teamwork in the real project development will benifit from the feature of branch. In this tutorial, the followings will be introduced:

-   what is a branch
-   The main branch operations
-   how to achieve effective teamwork by through branch management


<a id="org023a798"></a>

### What is a branch

“A branch in Git is simply a lightweight movable pointer to one of these commits. The default branch name in Git is master. As you initially make commits, you're given a master branch that points to the last commit you made. Every time you commit, it moves forward automatically.”


<a id="org0db3995"></a>

### Common operations of branches

-   Creat a new branch based on the current branch

    git branch develop

-   Swith to the new branch

    git checkout develop

-   one step to create and switch to a new branch develop

    git checkout -b develop

-   Push the created branch to github

    git push origin develop

-   Check the local branches

    git branch

-   Check the remot branches

    git branch -r

-   Delete a local branch named develop

    git branch -d develop

-   Delete a remote branch named develop

    git push origin :develop

-   Fetch a remote branch to local

    git checkout develop origin/develop

-   Fetch a remote branch to local and switch to this branch

    git checkout -b develop origin/develop


<a id="org6a70ba2"></a>

### TODO Git Flow, teamwork based on branches

[A successful Git branching model](git-model.png)


<a id="org1392ad8"></a>

## Bookmark Management


<a id="org2e3543e"></a>

## Customization


<a id="org5dcec22"></a>

# Magit Tutorial


<a id="orgc0e74e6"></a>

## Basic magit


<a id="org7cad0a3"></a>

### Create a git repo

[info:magit#Repository setup](magit#Repository%20setup)
You can create a git repo with M-x magit-init. This will create a git-repo in the current directory.

    (magit-init)

<magit-init>


<a id="org7e375b0"></a>

### Clone a repo

[info:magit#Repository setup](magit#Repository%20setup)

M-x magit-clone

This will prompt you for a repo, which is either a url, or a path, and a path to clone it to.

<magit-clone>


<a id="orgf48368c"></a>

### Check the status of your repo

[info:magit#Status buffer](magit#Status%20buffer)

Run M-x magit-status to see the status of your repo.

Press "g" in the window to refresh it.

press "n" (next) or "p" (previous) to navigate in this window.

<magit-status>


<a id="orgcb5d751"></a>

### Stage a file

[info:magit#Staging and unstaging](magit#Staging%20and%20unstaging)

In the magit-status window, put your cursor on an unstaged file and press "s".

If you press TAB on the file, it will expand to show the changes that are unstaged. Deletions show in red, and additions in green. The changes are in "hunks".

You can unstage a file with "u"


<a id="org748325f"></a>

### Commit a file

[info:magit#Initiating a commit](magit#Initiating%20a%20commit)

[info:magit#Editing commit messages](magit#Editing%20commit%20messages)

In the magit-status window with some files that are staged, press "c", review the options, and probably press "c" again. Enter a commit message and type "C-c C-c" to commit it, or "C-c C-k" to cancel it.


<a id="org709ed5e"></a>

### Diffs

[info:magit#Diffing](magit#Diffing)

From the magit-status window, press "d" then "d" to see what has changed.


<a id="orgff0beb6"></a>

### See the log

[info:magit#Logging](magit#Logging)

In the magit-status window press "l", review the options, and press "l" again.

If you want to see only the commits that affected a file, in the magit-status window press "l" then "=f", enter the filename, and then press "l" again.


<a id="orgd83ca2a"></a>

### Push

[info:magit#Pushing](magit#Pushing)

In the magit-status window press "P" then "p".

Note that tags don't normally get pushed, but there are options ("T" to push a tag, and "t" to push all tags).


<a id="org53afa0f"></a>

### Pull

[info:magit#Pulling](magit#Pulling)
In the magit-status window press "F" then "p".


<a id="org157b9de"></a>

### Run a command-line git command manually

[info:magit#Running Git manually](magit#Running%20Git%20manually)
In the magit-status window, type "!" to get the popup and choose what you want to do (e.g. where to run the command, etc&#x2026; You do not need to type "git" in the command. Note you can also run a shell command from this interface.


<a id="org71f1875"></a>

### Check the output of the git command

Press "$"


<a id="orgf68ab5f"></a>

### Keybindings

[info:magit#Keystroke Index](magit#Keystroke%20Index)


<a id="orga33c943"></a>

## Intermediate concepts


<a id="orgb8378a0"></a>

### Checkout an older version of a file

Use M-x magit-checkout-file select the branch, or enter a revision, and then choose a file.

<magit-checkout-file> 

<magit-find-file>
<magit-find-file-other-window>


<a id="orgb6f2a45"></a>

### Search the commit messages for a pattern

In a magit-status window press "l =g" enter a pattern to grep for, and then press "l".


<a id="org462c89f"></a>

### Revert a commit

[info:magit#Reverting](magit#Reverting)

Got to the log, select the commit and type "V" then "V".


<a id="org686c873"></a>

### Tag a version

[info:magit#Tagging](magit#Tagging)

press "t" in the magit-status window. You can then create a tag, annotate it, delete tags, and prune them.


<a id="orgb0332c4"></a>

### Checkout an existing branch.

[info:magit#The branch popup](magit#The%20branch%20popup)

In the magit-status window press "b" then "b" and choose the branch.

To checkout a new branch, in the magit-status window press "b" then "c". Choose the branch to start from then a name for the new branch.


<a id="org542818d"></a>

### Merge two branches

[info:magit#Merging](magit#Merging)

In the magit-status window press "m", then "m" and select the branch to merge into the current one.


<a id="orgc6db71a"></a>

### TODO Resolving conflicts

[info:magit#Resolving conflicts](magit#Resolving%20conflicts)

You will probably also want to get familiar with [info:ediff#Top](ediff#Top).

On a file in a magit-status window, press "e" to enter the 3-window ediff view. The A window is the version at HEAD, the B window is what is in the index, and the C window is the current version.


<a id="org93b76fd"></a>

### Fetching

[info:magit#Fetching](magit#Fetching)

In the magit-status window press "f".


<a id="orgecf9064"></a>

### Add a remote

[info:magit#Remotes](magit#Remotes)

M-x magit-remote-add
then enter an alias, and the url.


<a id="orgc0366dc"></a>

### Stashing

[info:magit#Stashing](magit#Stashing)

Press "z" in the magit-status window


<a id="org8fa58b8"></a>

### Git blame


<a id="org67eaeb9"></a>

## Advanced concepts


<a id="orga48082a"></a>

### Resetting

[info:magit#Resetting](magit#Resetting)


<a id="orgc40f7c4"></a>

### Rebasing

[info:magit#Rebasing](magit#Rebasing)

1.  Interactve rebasing

    Open the log, select the oldest commit you want to rebase on then press "r" and then "i". Use M-p and M-n to move commits around. Press "s" on any commits you want to squash into the commit above it. C-c C-c will start the commands.
    
    From the magit-status on unpushed commits, you can also press "r" to get the rebase popup.

2.  Reword a commit message

    "r w" allows you to reword the commit message.


<a id="org38f7120"></a>

### Create patches

[info:magit#Creating and sending patches](magit#Creating%20and%20sending%20patches)

In magit-status window, press "W"

"W p" creates patches
"W r" makes a pull request. This just creates an email with information in it. It is not a GitHUB request, and it is only useful if there is a public, external copy of the repo.


<a id="org5d2740f"></a>

### Cherry-picking

[info:magit#Cherry picking](magit#Cherry%20picking)

Press "A"


<a id="orge7f5e22"></a>

### Apply patches

[info:magit#Applying patches](magit#Applying%20patches)


<a id="org79a8f79"></a>

### Notes about commits

[info:magit#Notes](magit#Notes)

Press "T" to attach a note.

A typical use of notes is to supplement a commit message without changing the
	commit itself. Notes can be shown by git log along with the original
	commit message. To distinguish these notes from the message stored in
	the commit object, the notes are indented like the message, after an
	unindented line saying "Notes (<refname>):" (or "Notes:" for
	refs/notes/commits).


<a id="org076f025"></a>

### Cherry-picking

[info:magit#Cherry picking](magit#Cherry%20picking)


<a id="orgec06ce5"></a>

# TODO Test

<span class="timestamp-wrapper"><span class="timestamp">&lt;2019-08-13 Tue 18:00&gt;</span></span>

This is a test

This is a test drawer

This is a test two

