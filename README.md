# Learning-Git-and-GitHub

### Window’s commands

<hr width="400px" align="left">

- To change directory to somewhere in current driver `cd {directory name}`

- To change directory to somewhere in another driver `cd /d {d:\programming\html}`

- To display everything in current directory `dir`

- To make a directory `mkdir`

- To display hidden files in directory `dir /a:h`

- To create a new file `cd . > file.txt`

- To delete a file `rm -rf {file_name}`

### Git commands:

<hr width="400px" align="left">

- To initialize a git repository `git init`

- To display all changes in the repository `git status`

- To stage the changes of all files(to save any changes they must be staged first) `git add .`

  > You know what it is for a particular file

- To save the changes `git commit -m “your text”`

  > -m here refers to message a commit can only happen with a message.

- To check whether the commits are successful try running `git status` again.

- If you staged a change and want to restore previous version `git restore –staged {file_name}`

- To see all modifications made ever `git log`

- If you committed a change and want to move to a previous version, use `git reset {sha code}`

  > You can get the sha code in GitHub or by git log

- If you don’t want to change your files but want to store the changes somewhere else `git stash`

- If you want the changes in stash to come to live `git stash pop`

- If you want to clear all the changes in stash `git stash clear`

- `git remote add {origin} {URL}`

> here `git` means a git command
> `remote` means you are working with URL’s
> `add` means you are adding the URL
> `origin` is used to tell what the name of URL is going to be

- To see all the URL’s attached to your folder `git remote -v`

- To push the repository to GitHub `git push origin master`

> Here `master` is the branch you are pushing and `origin` is the URL you are referring to. It `also commit’s` all changes.

- To create a new empty branch `git branch {branch_name}`

- To move your default branch to some others `git checkout {branch_name}`

- To get commits of other branch after merging `git fetch –all –prune`

> All the `commits` that are made will be done on the `default branch`. The `head` will point to the `default branch.`

> _**Note:**_ Commit after checkout.

- To merge a branch to the default branch `git merge {other_branch}`

- To clone a repository `git clone {URL}`

> After cloning a repository, the original repository URL is known as upstream URL

> **If a branch already has a pull request you cant create another pull requests hence the commit’s will be pushed**

- To force push something `git push origin {brach_name} -f`

> Force commits are done if a reset is made to a previous version.

> _**Note:**_ a proposal to merge a set of changes from one branch into another in a software development project

- Reset main branch of my origin to main branch of upstream `git reset –hard upstream/main`

- Brings modifications in remote repository to local repository with commits `git pull upsteam/main`

- Bring modifications in remote repository to local repository with out commits `git fetch upstream/main`

- To squash multiple commits into one (use pick to show and s to squash) `git rebase -i {sha}`

**_A merge conflict occurs when multiple contributor’s change same line or something similar_**
