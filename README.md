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