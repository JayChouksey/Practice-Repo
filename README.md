# Practice-Repo
This repo is for practice purpose. 

`Learnings:`

*Date : 14 July*
- What is git?
- Git vs Github
- Creating a new repo
- Some commands : 
    - git --version
    - git config --global user.name <user name>
    - git config --global user.email <user email>
    - git config list
    - git clone <repo url>
    - git status 
    - git add 

*Date : 16 July*
- Revised last class concepts
- What is staging? 
- Learnt command *git commit* 
- Learnt about *git reset* to undo staged files 
- Learnt about *git push* and *git pull*
- Learnt command *git show <commit id>* to see the changes of specific commits 

*Date : 18 July*
- Revised last class concepts
- How to create new branches
- How to commit from different branches
- git switch <branch name> : to switch to different branch
- git switch -c <new-branch-name> : for creating and switching simoltaneously 
- git branch -m <new-name-of-the-branch> : to rename the branch

*Date : 21 July*
- Revised last class concepts 
- What are merge conflicts?
- How to resolve conflicts 
- git pull origin <branch name> : to fetch the new changes from remote to local
- git fetch : to retrieves changes without modifying local branches
- git diff : to check the differece between different codes 
    - Viewing unstaged changes : *git diff*
    - Viewing staged changes : *git diff --staged* or *git diff --cached*
    - Viewing all uncommitted changes : *git diff HEAD*
    - Comparing two specific commits : *git diff <commit1> <commit2>*
    - Comparing branches : *git diff <branch1> <branch2>*
    - Comparing a specific file : 
        - git diff <file_path>
        - git diff <commit1> <commit2> -- <file_path>
        - git diff --staged <file_path>
- How to create a Pull Request?
- git remote : shows the list of remotes
- git remote add <remote-name> <remote-link> : to add new remote
- git remote remove <remote-name> 
- git remote rename <remote-name> <new-remote-name>

*Date : 22 July*
- git reset --<flag> HEAD~1 : to undo previous changes and *it removes completely the last head* 
    - soft : will undo all the changes and put them in staged area 
    - mixed(default) : will undo all the changes them in unstaged area
    - hard : will undo but remove all the changes
    - hard origin/<branch> : want to undo your resets and match the remote 
- git push --force origin <branch> : when head is behind but you are sure to merge code to remote 
- git revert <commit-hash> : to undo all previous changes in form of new commit
    - -n or --no-commit: Applies the changes to your working directory and index, but does not create a new commit.
    - -e or --edit(default) : Opens the configured editor to allow you to modify the default commit message for the revert commit.
    - --no-edit : Creates the revert commit with the default commit message without opening the editor.
    - -m <parent-number> : Used when reverting a merge commit.
    - Eg : 
        - git revert HEAD : Revert the most recent commit.
        - git revert a1b2c3d : Revert a specific commit by its hash
        - git revert a1b2c3d --no-commit : Revert the changes of a commit without creating a new commit immediately
        - git revert HEAD~3..HEAD : Revert a range of commits (from oldest to newest). This reverts the changes introduced by the last three commits.
        - git revert -m 1 <merge-commit-hash> : Reverting a merge commit, specifying the parent to revert from
- git checkout <file-name> : 
    - discards all local changes to the provided file.
    - works only for unstaged changes
- type *:qa* : to come out of editor window in terminal  

*Date : 05 August*
- git stash :
    - git stash -m <message>
    - git stash pop
    - git stash apply
    - git stash list 
- .gitignore file : it tells Git which files or directories to ignore 

*Date : 07 August*
- Tagging and Releases : tag is a Git reference to a specific commit, often used to mark important milestones like releases.
    - Lightweight Tag : git tag v1.0.0 
    - Annotated Tag : git tag -a v1.0.0 -m <msg>
    - Creating, deleting, pushing tags
    - Versionin projects with tags
    - git tag, git show, git push origin<tag>

- Cherry-Pick : git cherry-pick <commit-hash>
