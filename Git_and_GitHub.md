# Git and GitHub



### What is Git?

It is the most popular system implemented for version control to date. It is available on most operating systems and can operated either via command line or by a GUI. 

![The stages of a git repository.](https://git-scm.com/images/about/index1@2x.png)



### What is GitHub?

GitHub is a web-based repository service. It is used integrally in many businesses and projects today, as besides remote storage and version-control, it also allows for collaboration between multiple users towards a single project.



### Popular Git Commands

##### *git init*

This command initialises a new repository. This involves creating a *.git* folder with metadata regarding the new local repository.

##### *git clone [path to repository]*

This command is used to copy a repository locally. It checks out a local or remote repository as specified and creates a local copy. Remote repositories may be copied in two ways, by HTTPS or SSH.

##### *git config*

This command lets you configure your Git installation (or an individual repository) from the command line.

##### *git add*

This allows us to move files from the working directory to the staging area so that changes to these files may be committed. However, changes are not actually made to the repository until the actual commit.

##### *git commit {-m "Message Body"}*

This command commits the contents of the staging area onto the branch specified. The `-m "Message Body"`  may be avoided if a text editor is configured to accept the messages. This is done via the `git config` command.

##### *git status*

Lists and gives details on which files are staged, unstaged, modified and newly created.

##### *git log {-n [limit]}/{--graph}* 

The command `git log` displays a log of previous commits within the branch specified. Various versions of `git log` achieve different things. The use of `-n` can restrict the number of items in `git log` to a specified limit. The use of `--graph` displays the log in a graphical manner.

##### *git diff* {[filename1]} {[filename2]}

This command is used to check differences between the working directory and staging area, staging area and repository, or two versions of a file.

##### *git checkout [branch]/[file]/[commit]*

The `git checkout` command performs three distinct functions: checking out files, checking out commits, and checking out branches. Checking out something is the git equivalent of selecting that something to work on.

##### *git branch {[name]}*

This command is used to create a branch at the existing section or to see the branches that exist. Branches are useful entities that allow us to work on the project without affecting the main or *master* branch. They are often used to test experimental features or to change certain aspects of code before introducing it to the stable master.

##### *git merge [branch1] {[branch2]}*

This method merges two branches together. It checks for conflicts within the code, and if there are none, commits the merge.

##### *git revert [commit]*

The `git revert` command undoes a commit or several commits. Instead of removing the commit from the project history though, it appends a new commit with the corrected file.

##### *git reset*

A `git reset` will permanently undo changes made by you to a repository or file.

##### *git remote*

This command lets you create, view, and delete connections to other repositories. Usually, these repositories are not stored locally.

##### *git fetch [remote]*

This command imports commits from a remote repository into your local repository. These are stored as remote branches instead of the normal local branches. A `git merge` command is used to bring changes into the local repository.

##### *git pull [remote\] \[branch]*

This command combines `git fetch` and `git merge` into one command, and brings the remote changes into your local repository.

##### *git push [remote\] \[branch]* 

Pushing shifts your local commits onto your remote repository.

**git comm